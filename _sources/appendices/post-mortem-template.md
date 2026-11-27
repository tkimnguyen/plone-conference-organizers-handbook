---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "A copyable post-mortem skeleton for a Plone conference, based on the Seattle 2006 account, with prompts per section and the handover deadline."
    "keywords": "Plone, Plone Conference, post-mortem, lessons learned, handover, template"
---

# Template: post-mortem

A post-mortem is the first deliverable of the handover contract.
It tells the next team what you did, what happened and what you would advise.
The skeleton follows the Seattle 2006 account "Things We Learned About Running a Plone Conference", the one early conference that wrote its lessons down for its successors.
The worked example is the [2026 case file](../conferences/2026-maastricht/conference-2026-maastricht.md).

## When it is due

The outgoing team owes the post-mortem to the next team by T+60 days, counted from the last conference day (proposed in [Governance](../running/governance.md), decision D8).
It is filed under `conferences/<year>-<city>/` by T+75 days, together with the anonymized survey results.
Write the first draft in the first two weeks after the event, while memory is fresh, and use the remaining time for review and for the numbers.

Seattle published its whole evaluation on one public page: the surveys, the open comments, the detailed budget and a lessons document addressed to future organizers (L-1003).
It also published total staff hours alongside the budget (L-1037).
Bristol published its budget model and final figures so that future hosts would have what the team wished it had had when bidding (L-2031).
The 2015 Foundation hosting call asked bid teams to read past lessons-learned reports before writing their own, which makes yours the de facto handover material (L-4065).

## How to use this template

1. Copy the skeleton below into a fresh file for your conference.
2. Write in first person, as the team, and be candid about money and mistakes.
3. Answer the prompt under each heading.
   Delete the prompt when the section is written.
4. Cite evidence for every claim: a ledger row, a source, a tracker item or a dated message.
5. End every area with the three verdict lists, so the reader gets advice and not only a story.
6. Generalize before filing.
   No personal data, no private amounts, no vendor contacts, no ticket-platform user data.
   The public record carries rules, guidelines, aggregates and pointers only.
7. Mark draft status honestly.
   Facts the team has not confirmed are flagged as reported, hearsay or pending verification.

## The skeleton

```text
# <Conference name and year>: post-mortem

Status: draft | signed off by <team role> on YYYY-MM-DD

## Purpose of this document
Who is this for, and what should the reader be able to do after reading it?
Name the skeleton you followed and what you changed.

## Overview
Dates, city, venue type, format, days and tracks.
Who organized it (organizations and roles, never private contact details).
Who wrote this document and when.
Attendance and result in aggregates only.

## Why this city and this venue
Why you chose them.
What was good, and what were the disadvantages.
What you would check before choosing again.

## Master timeline
Reverse-chronological, from the last conference day back to the day the bid was accepted.
Mark the dates that mattered: freezes, opening of sales, call for proposals, contract signatures.
State when you wish you had started each stream.

## What was planned and what happened
One short block per workstream, in this order:
program, speakers, training, ticketing, sponsors, money, venue, catering,
accommodation, travel and visas, social events, audio and video and internet,
marketing and communications, print and merchandise, volunteers and roles,
code of conduct, accessibility, health and safety, sprints.
For each: what the plan said, what actually happened, what the difference taught you.
Close every block with the three verdict lists below.

## Verdict lists
### Good things to do again
- <one line each, with evidence IDs>
### Things we did not do that you probably should not either
- <one line each, with evidence IDs>
### Things we might do differently next time
- <one line each, with evidence IDs>

## Expected but never written down
Every implicit expectation you ran into.
For each: who expected it, what it cost, and where it should be written down.

## Numbers
Aggregates only: attendees by ticket type, speakers, tracks and sessions,
income and cost by category, result, volunteer and staff hours.
Give each figure a date and a source.
Link the budget sheet and the anonymized survey analysis.

## Survey results
One page of conclusions, linking the anonymized analysis.
State who answered and who is missing.

## What this record feeds
For each handover deliverable: done, pending or not applicable, with the date.
List the handbook chapters your lessons belong to, so the steward can place them.

## Sources and further reading
Evidence IDs and links.

## Thanks
Thank the people and organizations who helped, with their consent.
```

## Prompts per section

### Purpose, overview and city

Say who the record is for in one sentence, then give the facts a successor needs to judge whether your conference resembles theirs: size, venue type, format and organizing body.
Those facts are the same tokens the handbook uses to decide whether a lesson applies (see [Tailor](../start/tailor.md)).
Seattle added a short "why this city" section with good points and disadvantages, and that section is worth copying.

### Master timeline

Write it backwards.
The reader should be able to ask "what should be done by this date?" at any point before their own event.
Add one line per stream saying how much earlier you would start next time.
Seattle's own timeline advised starting about six months out, and your version of that advice is the most reusable line in the section.

### Planned versus what happened

The comparison matters more than either side.
If the plan said one thing and the event showed another, say what you believed and why it was wrong.
Keep each block short, and link to the handbook chapter that holds the general advice instead of repeating it.

### The three verdict lists

Keep one set per area, not only one for the whole event.
A good item is one line, names a concrete action and cites its evidence.
The "did not do" list is for things you skipped and think the next team should not skip.
The "differently" list is for things you did and would change.

### Expected but never written down

This is the list earlier conferences never produced.
Look for promises made by habit: speaker discounts, trainer accommodation, who pays for the sprint room, who owns the video.
Record the expectation, its owner and the cost it created.
The next team turns each line into a written decision (see [Community and speaker expectations](../job/community-and-speaker-expectations.md)).

### Numbers

Publish the budget and the hours, and say which figures are estimates.
Past teams kept the working budget in a spreadsheet whose revision history readers could not see, and the evolution of the budget was lost to successors (L-2025).
Export a dated copy with the post-mortem.
Use the [budget sheet template](budget-sheet-template.md) so the sheet has the same shape every year.

### What this feeds

Close the loop so the post-mortem does not sit alone.
List which deliverables of the handover contract are done, which are pending and why.
The 2026 case file shows the table with its honest "pending" cells.

## Related

- [Handover contract](../job/handover-contract.md) for the six deliverables.
- [Template: attendee survey](survey-template.md) for the survey the post-mortem links.
- [Annual ritual](../running/annual-ritual.md) for how lessons enter the handbook after filing.
