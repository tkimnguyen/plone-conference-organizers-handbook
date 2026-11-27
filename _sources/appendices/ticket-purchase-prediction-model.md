---
steward: unassigned
deputy: unassigned
review-by: 2028-11-01
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "A rerunnable method for forecasting attendance when a community buys tickets late, with inputs, scenarios and a code sketch built on synthetic numbers."
    "keywords": "Plone, Plone Conference, ticket sales, forecast, attendance prediction, late buying"
---

# Ticket-purchase prediction model

The Plone community buys tickets late.
Sales that look weak six weeks out can still end well above break-even, and sales that look healthy can hide a real shortfall.
Organizers who cannot tell the two apart either panic and cut what they should keep, or relax and miss a real gap.
This page describes a method that helps a treasurer tell a late-buying pattern from a demand problem, using the conference's own sales data.

The method comes from the forecast that the 2026 team reran each time the sales export changed (S108, L-5066).
That implementation carried edition-specific configuration and identity-bearing output, so this page describes the method and gives a sketch built on synthetic numbers.
Future organizers supply their own protected sales data and keep it out of the handbook (L-5029).

## Why a forecast and not a feeling

Late buying is a pattern, not an exception.
One conference saw sales below break-even four weeks out and a late rush that carried the total well past it (L-2084).
Cash-flow planning for a community that buys late needs sales evidence, so that normal late purchasing is separated from a revenue shortfall before commitments increase (L-5008).
A low-sales warning is assessed against the expected late-purchase pattern and a dated forecast, because anxiety alone does not show a collapse of demand (L-5009).

The first-hour response to a real gap is in the playbook [Playbook: low ticket sales](../risk/playbooks/low-ticket-sales.md).
This page supplies the numbers that the playbook's second step needs, which is the decision whether the gap is timing or demand.

## What the model does

The model estimates physical attendance on the principal conference days at a checkpoint date, in three scenarios.
It does so with two independent views and takes the larger.

1. **Pace view.** Take the tickets sold so far and project them to the checkpoint with the measured sales velocity. Then divide by the share of final sales that earlier conferences had reached by that checkpoint. Blend the result with a straight-line continuation of the current velocity, so a single historical curve does not dominate.
1. **Named view.** Take the projected tickets and add the people the team knows are coming but have not yet bought: speakers without a ticket, weighted by the chance that each buys, and unclaimed sponsor seats, weighted by the chance that each is named.
1. **Attendance.** Add the people who attend without any ticket, such as organizers and keynote speakers. Take the larger of the two views for ticket holders and subtract an expected no-show rate.

The 2026 implementation also separated daytime attendance from other ticket categories, such as party-only tickets, and compared scenario estimates using sales velocity and reviewed judgment inputs (L-5066).
Keep the separation: a ticket for an evening event does not fill a conference room.

## Inputs a future team needs

| Input | Where it comes from | Who reviews it |
|---|---|---|
| Tickets sold by category, with dates | The ticket platform export, one per run | Treasurer |
| Previous export | The last run, for the measured sales velocity | Treasurer |
| Past sales curves | Earlier conferences, cumulative tickets by days before the event | Treasurer, with the handbook's [conference data table](../evidence/conference-data-table.md) as a starting point |
| Checkpoint dates | The venue and supplier deadlines, such as the headcount freeze | Conference chair |
| Speakers without a ticket | The program list matched against the ticket list | Program lead |
| Unclaimed sponsor seats | The sponsor benefits list | Sponsor lead |
| People attending without a ticket | The team list | Conference chair |

Four of these are judgment inputs: the speaker count, the sponsor seat probabilities, the people without a ticket, and the scenario parameters.
The script prints the raw material for each, a person adjusts the numbers, and the script runs again.
Do not bump the judgment inputs mechanically from one run to the next.

## Panic or pattern

The question the model answers is whether today's number is behind the usual curve or behind the plan.
Use three checks, in this order.

1. **Compare with the curve.** What share of final sales did earlier conferences have at this many days before the event? If your number is at or above the low end of that range, you are inside the late-buying pattern.
1. **Compare with the checkpoint.** Do the three scenarios cross break-even at the date the next cost cannot be reduced? If the low scenario already does, the gap is not a timing issue for that cost.
1. **Compare with velocity.** Has the weekly rate dropped, or only the total? A falling rate with a fixed total is a stronger signal than a low total on its own.

Write the verdict and the date of the next check down.
A record that says "inside the pattern, check again at the headcount freeze" ends a week of worry.

## A sketch

The code below is a sketch, not a tool.
Every number is a synthetic placeholder.
Replace the scenario parameters with values from your own past curves where you have them, and keep a dated snapshot of each run.

```python
import math
import statistics
from dataclasses import dataclass


@dataclass(frozen=True)
class Scenario:
    name: str
    share_at_checkpoint: float  # fraction of final daytime tickets sold by the checkpoint
    velocity_factor: float      # multiplier on the measured sales velocity
    no_show_rate: float
    speaker_weight: float       # chance that a ticketless speaker buys or registers
    sponsor_factor: float       # multiplier on sponsor seat probabilities


SCENARIOS = [
    Scenario("low", 0.80, 0.75, 0.05, 0.50, 0.5),
    Scenario("mid", 0.70, 1.00, 0.03, 0.75, 1.0),
    Scenario("high", 0.60, 1.25, 0.01, 0.90, 1.2),
]


def checkpoint_shares(past_curves, days_before):
    """Past curves: lists of (days_before_event, cumulative_tickets).
    Returns the low, median and high share of final sales reached by the checkpoint.
    A low share means late buying, so it feeds the high scenario."""
    shares = []
    for curve in past_curves:
        final = max(t for _d, t in curve)
        sold = max((t for d, t in curve if d >= days_before), default=0)
        shares.append(sold / final)
    shares.sort()
    return shares[0], statistics.median(shares), shares[-1]


def forecast(daytime_sold, velocity, days_to_checkpoint, gap_days,
             confirmed_without_ticket, speakers_without_ticket,
             sponsor_seats, s):
    """sponsor_seats: list of (seats, probability that the seats get named)."""
    v = velocity * s.velocity_factor
    at_checkpoint = daytime_sold + days_to_checkpoint * v
    scaled = at_checkpoint / s.share_at_checkpoint
    linear = at_checkpoint + gap_days * v
    pace = 0.6 * scaled + 0.4 * linear
    named = (at_checkpoint
             + speakers_without_ticket * s.speaker_weight
             + sum(n * p * s.sponsor_factor for n, p in sponsor_seats))
    attendance = confirmed_without_ticket + (1 - s.no_show_rate) * max(pace, named)
    return pace, named, attendance


results = {}
for s in SCENARIOS:
    pace, named, attendance = forecast(
        daytime_sold=60, velocity=1.5, days_to_checkpoint=30, gap_days=14,
        confirmed_without_ticket=5, speakers_without_ticket=12,
        sponsor_seats=[(8, 0.8), (4, 0.4)], s=s)
    results[s.name] = attendance
    print(f"{s.name}: pace={pace:.0f} named={named:.0f} attendance={attendance:.0f}")

# One venue-style guarantee rule: cover the middle case and most of the high case.
guarantee = math.ceil(max(results["mid"], results["high"] / 1.10))
print("guarantee candidate:", guarantee)
```

The 2026 team set the scenario parameters by hand and kept them fixed from run to run, so that a change in the output came from the data and not from retuning.
The sketch adds a way to take the share at the checkpoint from your own past curves instead.
A scenario such as the guarantee rule at the end is specific to a venue that asks for a headcount band, so write your own rule from your contract.

## How to run it

1. Collect at least three past sales curves, with cumulative tickets by days before the event. Done when each curve has a point near the checkpoint and a final total.
1. Export the current tickets and keep the previous export. Done when the two files carry dates in their names.
1. Fill in the judgment inputs from the printed raw material, and write down what you chose and why.
1. Run the sketch and save the output with the date. Done when a dated snapshot sits next to the previous ones.
1. Read the three scenarios against the next dated cost, and use the panic-or-pattern checks to write the verdict.
1. Rerun whenever another export arrives, and always at each checkpoint date.

## Limits

- The model is only as good as the past curves. With fewer than three, treat the output as a rough range.
- Attendance is counted in tens or low hundreds, so a few large orders move the totals. Look at the orders, not only the sum.
- The model estimates attendance. It does not set prices, and it does not replace a cash view.
- Co-located events and bundled tickets change the curve. Note them beside each past curve.

## Applies when

Use the method when ticket income matters to the budget and when a venue, caterer or supplier asks for a headcount at a fixed date.
A free event with no cost per head does not need it.

## Thin content

```{warning} Only one dataset has been tried
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Sales curves from several earlier conferences, and a rerun of the method by a second team with its own data | who-might-know: Treasurers and ticketing leads of past conferences

The method is generalized from one implementation used at one conference.
The scenario parameters are placeholders, and no historical curve is published in the handbook.
```

## Sources

- S098 Plone Conference 2026 facts and lessons for the handbook.
- S108 Attendance forecast implementation, 2026.
- Related ledger rows: L-2084 (a late rush after a low reading four weeks out), L-5008 and L-5009 (the late-purchase pattern and the low-sales warning).
