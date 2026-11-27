---
steward: unassigned
deputy: unassigned
review-by: 2028-11-01
maturity: draft
applies-to: [all]
diataxis: how-to
myst:
  html_meta:
    "description lang=en": "A reusable argument skeleton for a grant application that funds reduced-price tickets for attendees from the global south, with placeholders."
    "keywords": "Plone, Plone Conference, grant, global south, scholarship, ticket subsidy, template"
---

# Global south grant argumentation

This page gives the argument structure of a grant application that asks a funder to subsidize conference tickets for attendees from the global south.
The structure comes from the 2026 application to a Python community foundation's grants program (S109).
It holds no text from the real application, no amounts, no headcounts and no contacts.
Every placeholder in angle brackets is yours to fill with your own figures and your own policy.

Read the outcome before you copy anything.
The 2026 application was drafted, reviewed and sent, and then stayed without a response.
The final countdown plan records it as discarded for that reason (S100, L-5005).
The structure is reusable, and the funding is not guaranteed.
Keep an unconfirmed grant outside committed income, because an unanswered request cannot pay a contractual obligation (L-5006).

## What the application does

The 2026 application made access its central purpose.
It asked for money for one thing, discounted tickets, and showed the funder what each part of the grant would buy (L-5067).
A funder reads many applications, and a single clear purpose with visible arithmetic is easier to say yes to than a general request for event costs.

The pricing initiative and the funding application are separate tasks.
The conference introduced reduced prices for attendees from the global south and also went looking for money to pay for them (L-5004).
Decide the reduced price and the eligible group first, in your own team, and write the application second.

## The argument in six moves

### Move 1, state one purpose

Open with the one thing the grant is for.
Say who the conference is for, how it connects to the funder's community, and what barrier you want to remove.

Skeleton:

> We are applying for <grant name> with one central purpose: to subsidize conference tickets for attendees from <eligible regions>.
> <Cost of travel and registration> is the biggest barrier that keeps <contributors, developers and users> from these regions away from international events.
> A reduced ticket price makes <conference name> accessible to people who are otherwise priced out, and brings a wider range of voices into the community.

Connect the purpose to the funder's own stated priority, in one sentence that quotes their published wording.
Do not paraphrase their mission from memory.

### Move 2, answer the checklist

Funders publish a checklist.
Answer it in order and use their headings.
Typical items are the event name, dates, location and website, the program, the amount requested and its purpose, the overall budget, the use of any surplus, the team background and how the funder will be acknowledged.
Give the dated program status honestly, for example "schedule not yet confirmed, to be posted at <address>".

### Move 3, show the unit economics

Put the arithmetic in the application, in a short block, so the effect of any change to the grant is visible at once.

```text
Unit economics:
  Regular ticket price:              <amount>
  Subsidized global south ticket:    <amount>
  Subsidy per recipient:             <amount>
  Number of beneficiaries:           <number>
  Total requested:                   <amount>
```

Then add one sentence that states the marginal effect: "every <amount> funds one additional attendee".
A funder that can only give part of the amount can see what a partial grant buys (L-5067).
State that the whole grant goes to access and none to general event operations, if that is true.

### Move 4, define eligibility

State who qualifies, in a short list the applicant can check without asking you.
The 2026 draft used three criteria of three kinds.

- Residence in a country on a published economic classification list. Name the list and link it. <published list>
- A self-declared statement that the applicant's employer does not pay the full price.
- A commitment to attend a minimum number of conference days. <number>

Choose criteria you can verify or can accept on a declaration.
Use your own event's eligibility policy, because the funder's list may differ from yours.

### Move 5, explain how you choose when demand exceeds supply

Say how you rank applicants when there are more than tickets.
A scoring rubric with stated weights is easier to defend than a statement that the organizers will decide.
The 2026 draft weighted community engagement most, then intent, then self-declared financial need, and gave a small part to an organizer adjustment for the balance of the group.

Skeleton:

| Criterion | Points | What it measures |
|---|---|---|
| Community engagement | <points> | Contributions, meetups, writing, earlier open-source work |
| Intent | <points> | What the person will do at the conference and bring back |
| Financial need | <points> | Self-declared need |
| Cohort balance | <points> | An organizer adjustment for country, first-timers and diversity |

Then answer the fairness question the funder will ask.
Who scores, how do two scorers differ, and what happens when they disagree?
The 2026 draft proposed two independent scorers, one from the organizing team and one advisor from the community, with disagreements escalated to a third body (L-5068).
That draft was a proposal, and the implementation was not verified.
Do not name an escalation body in the application until that body has agreed to adjudicate.
Say how the results are reported, for example as anonymized figures in a post-event impact report.
Do not publish applicant records.

### Move 6, commit to acknowledgement and reporting

Funders fund what they can see.
Promise specific, checkable things.

- Where the funder's logo appears, for example the front page, the sponsors section and the opening slide shown before recorded talks.
- Which channels mention the grant before, during and after the event.
- An information table or stickers in the attendee bags, if the funder wants them.
- A short written report after the event, with the number of attendees the subsidy reached and photos the funder may use.

Only promise a report you will write.
Put the date in the project plan and assign an owner.

## The complete skeleton

Copy this into a draft and replace every placeholder.
Remove a move if the funder's checklist does not ask for it.

````text
Subject: Grant application, <conference name and year>, <city> (global south ticket support)

Dear <funder> grants workgroup,

<Move 1: one paragraph on the conference, the community and the single purpose.>

Here is the information requested in your application checklist.

1) Event name, dates, location and website
<...>

2) Description of the conference and program
Expected attendance: <number, from your own forecast>
Duration: <days and formats>
Target audience: <groups>
Tracks and talks: <short description>
Program status: <dated status and address>

3) Amount requested and purpose
We request <amount> to fund a ticket subsidy scheme for <number> attendees from eligible regions.
The grant lowers the registration price from <amount> to <amount>.
The entire grant goes to improving access and participation.

<Move 3: unit economics block and marginal sentence.>

Eligibility. <Move 4: criteria list.>

Prioritization if applications exceed tickets. <Move 5: rubric and scorers.>

4) Overall budget
Projected income: <amount>
Projected expenses: <amount>
<How the remaining gap is covered, and by whom.>

5) Use of any surplus
<One paragraph. Say that none of it is distributed privately.>

6) Organizing team
<Who organizes, how many people, what earlier conference experience they hold, and the Code of Conduct address.>

7) Acknowledgement and reporting
<Move 6: logo placement, channels, report with the number of attendees reached.>

Thank you for considering our application.

<Name and role of the sender>
````

## Before you send

1. Check the amounts against the budget and the published ticket page on the same day. Done when the figures in the application match the live ticket prices.
1. Check every claim about the funder's earlier grants against their published list.
1. Ask someone outside the drafting pair to read it. In 2026 a second reader asked for the unit economics and added the eligibility and scoring notes before the application went out (S109).
1. Agree who answers follow-up questions, and set a date to ask again if there is no reply. The 2026 team asked again and still received no answer (S100, L-5005).
1. Decide the plan if the answer is no or never. Reduced prices that depend on a grant need a fallback, such as a smaller number of places, an organizer-funded budget line or a sponsor-funded seat.

## Applies when

Use this structure when a conference wants to fund reduced-price places for attendees from regions where travel and registration are the main barrier.
The same argument works for a sponsor, a company or a foundation that does not publish a checklist, if you drop the checklist headings.

## Thin content

```{warning} The argument has no recorded success
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A grant application built on this structure that received an answer, with the funder's feedback | who-might-know: Organizers of conferences that applied to Python community funders; the funder's grants workgroup

The only application behind this page received no response, and its scoring and escalation process was proposed and not tested.
Funders' rules change, so check the current checklist before you use the headings.
```

## Sources

- S098 Plone Conference 2026 facts and lessons for the handbook.
- S100 Last-phase plan, 2026, for the outcome of the application.
- S109 Global south grant application discussion, 2026, for the argument structure. Amounts, headcounts, contacts and payee arrangements were withheld.
- Related ledger rows: L-5004 (the pricing initiative), L-5005, L-5006, L-5067 and L-5068.
