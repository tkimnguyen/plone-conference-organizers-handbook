---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How the handbook scores, places and reviews conference risks, and how an organizing team builds its own risk register at kickoff."
    "keywords": "Plone, Plone Conference, risk register, risk management, incident playbooks"
---

# The risk register method

A Plone conference fails in a small number of familiar ways.
Money is committed before it arrives, a key person drops out, the network collapses on the first morning, or the community turns out smaller than the plan assumed.
Each of these has happened at least once in the archive, and most of them happened more than once.

This page explains how the handbook records those risks, how a team scores them, and how a team turns the handbook's risks into its own register.
It does not repeat the advice of the chapters.
The advice lives in each chapter's "Risks" section and in the playbooks listed below.

## What the method covers

The handbook keeps risk advice in three places, and nowhere else.

- **Chapter risks.** Each chapter ends its advice with a "Risks" section.
  A risk there belongs to one workstream, for example a venue contract without a cancellation clause in `venue` or a missing insurance check in `contracts-legal-insurance`.
- **Cross-cutting risks.** Some risks span several workstreams and have no single home.
  They live on [Cross-cutting risks](cross-cutting-risks.md).
- **Incident playbooks.** When a risk turns into an event, the team needs a short first-hour script, not a chapter.
  The eight playbooks hold those scripts and link back to the chapters for the full advice.

The [Risk register](../generated/risk-register.md) collects every risk block from all three places into one table.
A script generates it from the pages, so nobody edits it by hand and it cannot drift from the chapters.

## How a risk is written

A risk is one thing that can go wrong, phrased as an event and not as a worry.
"The venue cancels ten weeks before the conference" is a risk.
"Venue problems" is not, because nobody can say whether it happened or what reduces it.

Every risk in the handbook carries the same fields:

| Field | Meaning |
|---|---|
| Likelihood | How probable the event is for a typical mid-size conference: low, medium or high. |
| Impact | How much damage it does to money, time or trust if it happens: low, medium or high. |
| Mitigation | One sentence that names an action, not an attitude. |
| Owner role | The role that watches the risk. A role, never a person. |
| Playbook | The incident playbook to open when the risk becomes an event, if one exists. |

The format, as a chapter author writes it:

````markdown
```{warning} Venue contract lacks a cancellation clause
:class: hb-risk hb-likelihood-low hb-impact-high
risk | likelihood: low | impact: high | mitigation: Negotiate cancellation and relocation terms before signing and keep one backup venue shortlisted | owner-role: treasurer | playbook: venue-loss

If the venue cancels late, the team carries the cost of rebooking.
```
````

The example is illustrative and is not one of the handbook's recorded risks.

## How a risk is scored

Likelihood and impact each map to a number: low is 1, medium is 2 and high is 3.
The score is their product, from 1 to 9.

| Score | Reading | What the team does |
|---|---|---|
| 6 or 9 | Severe | Name an owner at kickoff, act on the mitigation before the first contract, and review the risk at every planning meeting. |
| 3 or 4 | Material | Name an owner, set a date for the mitigation, and review the risk at each freeze. |
| 1 or 2 | Minor | Record it and review it at the monthly risk review. |

The scale is deliberately coarse.
Past conferences recorded what went wrong, not how often it went wrong across many editions, so a finer scale would claim a precision the evidence does not have.
Judge likelihood for a typical mid-size conference, and write in the risk body when the judgment depends on size, budget model or jurisdiction.

Two judgments deserve a second look.

- **Impact on trust counts as impact.** A Code of Conduct report handled badly can cost the community more than a budget overrun, even though no money changes hands.
- **Likelihood rises with dependence on one person.** A risk with a single owner and no deputy is more likely than the same risk with a named deputy, because illness and exhaustion are common (L-3075, L-5054).

## Building your own register at kickoff

The handbook's register is a starting list, not your register.
Build your own in the first month, so the owners know their risks before the first contract is signed.

1. Open the [Risk register](../generated/risk-register.md) and copy every risk into the team's own tracker, with its score, mitigation and owner role.
   Done looks like one row per risk in a file or board the whole team can see.
2. Delete the risks that cannot apply to your conference, and record the reason in your Tailoring Record.
   The [Tailor](../start/tailor.md) page explains the record.
3. Re-score the remaining risks for your size, budget model, venue and jurisdiction.
   Done looks like every changed score carrying one sentence of reason.
4. Add the risks the handbook does not know, especially those tied to your city, your venue type and your legal entity.
5. Put a person's name next to every owner role in your private tracker.
   The handbook names roles; your tracker names people.
   Done looks like no risk with a score of 3 or more lacking a named owner and a named deputy.
6. Give every mitigation a due date relative to the first conference day, for example T-6m.
7. Mark which risks open a playbook, and check that each playbook's owner roles are filled.
8. Read the [Cross-cutting risks](cross-cutting-risks.md) page with the whole team in one meeting.
   These risks have no single workstream owner, so they need a shared decision about who watches them.

## Review cadence

A register that nobody reads is decoration.
Tie the review to meetings the team already holds.

1. Review the severe risks at every planning meeting.
   The Conference Committee's schedule suggests meeting monthly, then every two weeks from late spring, then weekly in the last month (L-4026).
2. Review the whole register monthly, and at each of the program, headcount, and print-and-order freezes (L-5047).
   A freeze is the moment when a late change acquires a visible cost and owner, which makes it the natural point to ask what could still go wrong.
3. Review the register once more at T-2w with the people who will run the conference on site, and print the playbooks for the information desk.
4. After the conference, record which risks happened, which did not, and which nobody had listed.
   This record is part of the post-mortem.

The handbook's own register is reviewed in the [annual ritual](../running/annual-ritual.md).
When lessons from a finished conference arrive, the incoming team checks each risk that fired against its score and mitigation, and proposes changes by pull request.
A risk that happened at a conference where it was scored low is the strongest signal the handbook can receive.

## From risk to playbook

A risk earns a playbook when three conditions hold.

- It can turn into an event within hours, so there is no time to read a chapter.
- The first hour decides much of the damage.
- It has happened at a Plone conference or at a comparable community conference.

The eight playbooks that meet these conditions:

- [Playbook: Wi-Fi failure](playbooks/wifi-failure.md)
- [Playbook: cash-flow crunch](playbooks/cash-flow-crunch.md)
- [Playbook: low ticket sales](playbooks/low-ticket-sales.md)
- [Playbook: speaker dropout](playbooks/speaker-dropout.md)
- [Playbook: venue loss](playbooks/venue-loss.md)
- [Playbook: force majeure](playbooks/force-majeure.md)
- [Playbook: Code of Conduct incident](playbooks/coc-incident.md)
- [Playbook: key-person loss](playbooks/key-person-loss.md)

Every playbook has the same four parts: triggers, first-hour actions, owner roles, and related chapters.
A playbook never restates its chapters, so it stays short enough to read under pressure.

## Limits of the method

```{warning} No incidence data across conferences
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A per-edition record of which listed risks occurred, collected from post-mortems over several conferences | who-might-know: Conference Committee; past organizing teams; Plone Foundation board

The likelihood judgments rest on recorded incidents, not on counts across editions.
```

The archive tells us what went wrong, but rarely what went right because of a mitigation.
Treat every score as a judgment to revise, not a measurement.

## Sources

- S004 Conference Committee planning schedule.
- S034 Interview with the 2011 lead organizer.
- S100 Maastricht 2026 final-phase countdown plan.
- S101 Maastricht 2026 on-site roles.
