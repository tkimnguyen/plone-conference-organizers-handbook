---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to plan Plone Conference trainings: days, ticket model, trainer terms, call for trainers, rooms and replacements."
    "keywords": "Plone, Plone Conference, trainings, trainers, pre-conference"
---

# Trainings

## Why it matters

Pre-conference trainings are one of the strongest draws of a Plone conference, and the Foundation requirements register lists them as part of the conference design (as of 2026-11).
They bring newer community members in, and they give experienced people a way to teach.
They are also where an unwritten promise can cost the most.

Trainers have received lodging reimbursement and a free ticket, and some have asked what the work earns them.
The Foundation has no rule on any of this, so the first-time organizer meets the question late, with a published training offer already in the world.
The 2026 debrief named conference-funded trainer lodging near the venue as the largest financial risk of the conference (S098).
This chapter helps a team settle the terms before announcing the offer, and the money side is covered in `finance`.
What the community expects from trainers is covered in `community-and-speaker-expectations`.

## Applies when

- `all` The Foundation register expects pre-conference trainings at every conference.

## Decisions you must make

- {bdg-danger}`MUST` (req: R-017; as-of: 2026-11-02) **Will the conference include pre-conference trainings, and for how many days?** The register records one to two days in the call for proposals, and the day count comes from the call only.
  (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-4115, L-4189, L-5021) **What does a trainer receive, and is it agreed in writing before the training offer is announced?** Compensation is unregulated, and costs arise regardless of session length.
  Agree fee, ticket and travel terms with each trainer before any announcement.
  (decide-by: T-10m)
- {bdg-primary}`DEFAULT` (basis: L-4115, L-5020) **Who pays trainer lodging, and is it on site or nearby?** Conference-funded lodging close to the training venue was an implicit expectation.
  Fix the lodging commitment before confirming the training offer.
  (decide-by: T-10m)
- {bdg-primary}`DEFAULT` (basis: L-4068, L-4127, L-4200) **Are the training classes included in the ticket price?** Teams at several conferences included them, and the Foundation encourages inexpensive or included classes.
  Check the effect on ticket price and on trainer terms before deciding.
  (decide-by: T-9m)
- {bdg-secondary}`OPTION` **If classes are sold separately, who registers the students?** One conference let each trainer register students, which removed financial risk and confused some registrants.
  Handling registration centrally reduces the confusion.
  (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Do you write a quality floor into each trainer agreement?** The 2026 survey analysis proposed hands-on exercises, stated prerequisites and stated outcomes after one attendee reported learning nothing; it is one voice, and the fix costs little (L-6022).
  (decide-by: T-10m)
- {bdg-secondary}`OPTION` **Do you recruit an experienced community member as training lead?** The call for proposals has said since 2018 that teams may wish to.
  (decide-by: T-8m)

## How-to

### Plan the offer

1. Record the day count, the ticket model, the trainer terms and the lodging commitment in the Tailoring Record.
   Done looks like one entry that the treasurer and the program lead have both read.
1. Recruit a training lead if you chose to.
   The call for proposals from 2018 says a team may wish to recruit an experienced community member for this role (L-4081, S055).
   Done looks like a named lead.
1. Open the call for trainers with a quality check on proposals.
   Done looks like a call with published criteria and a review step.
1. Label each session honestly: a session called a training or tutorial is hands-on, with prerequisites announced in advance.
   Done looks like a prerequisites line in every class description.

### Announce and register

1. Release a preliminary program without talks, and send a survey on training registration before early-bird and regular tickets.
   The Foundation planning schedule places this in May (L-4038, S004, as of 2026-11).
   Done looks like survey results that size the rooms.
1. Publish class descriptions, dates and rooms, and tell trainees where each class meets.
   Done looks like an email to every trainee and room signs on the first morning.

### Run and close

1. Name a stand-in for every class, from experienced community members.
   Done looks like a list of stand-ins held by the training lead.
1. If a trainer withdraws, follow the `speaker-dropout` playbook.
   Done looks like the class run by the stand-in or released with an apology.
1. Check each training room for power outlets and a large screen before the first class.
   Done looks like outlets for every seat and a screen that shows code to the back row.
1. Survey trainees after the conference.
   Done looks like a rating per class that you hand to each trainer.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009, S032, S049 | ledger: L-1089, L-3068, L-4068 | confidence: observed | status: active | basis: independent-conferences

Pre-conference training by experienced trainers is a major draw and good marketing, especially for newer community members, and it works best when classes are inexpensive or included in the ticket.
An open call keeps the community involved, but it still needs quality control.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S046, S050, S054, S073 | ledger: L-4114, L-4127, L-4140, L-4200 | confidence: reported | status: active | basis: independent-conferences

Several organizing teams have chosen to include training in the ticket price.
The records show the choice repeated; they do not show its effect on trainer income or on ticket revenue.
```

Three further Seattle statements come from a single conference and are recorded in Case notes, not promoted: dropping three-hour tutorials (L-1094), handling training registration centrally (L-1095) and hands-on labeling of tutorials (L-1096).

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6020 | confidence: observed | status: active

Seventeen survey respondents attended trainings and 13 rated them, averaging 4.31 with eight top scores; the same ratings hold the only 1 in the dataset.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6021 | confidence: reported | status: active

One attendee expected hands-on work, reported learning nothing and listed stopping trainings that do not train as their stop-doing item. No respondent defended specific sessions in return.
```

```{note} [specific · 2025 · Jyväskylä · 1 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2025 | place: Jyväskylä | org: University of Jyväskylä | source: S079 | ledger: L-4219 | confidence: reported | status: active

Attendees praised training rooms with plenty of power outlets and a very large screen that made code examples easy to follow.
```

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S074 | ledger: L-4201 | confidence: reported | status: active

In-person training sessions averaged 4.5 out of 5 in the feedback survey.
```

```{note} [specific · 2023 · Eibar · 3 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2023 | place: Eibar | org: CodeSyntax | source: S073 | ledger: L-4200 | confidence: observed | status: active

Training classes were included in the conference ticket price.
```

```{note} [specific · 2023 · Eibar · 3 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2023 | place: Eibar | org: CodeSyntax | source: S070 | ledger: L-4186 | confidence: reported | status: active

Trainings went well except for one missing presenter, whose session experienced community members covered.
```

```{note} [specific · 2017 · Barcelona · 9 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2017 | place: Barcelona | org: Iskra SCCL | source: S054 | ledger: L-4140 | confidence: observed | status: active

A wide range of training classes was included in the conference ticket price.
```

```{note} [specific · 2016 · Boston · 10 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2016 | place: Boston | org: Plone Foundation | source: S050 | ledger: L-4127 | confidence: observed | status: active

Two days of training were included in the ticket price.
```

```{note} [specific · 2016 · Boston · 10 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2016 | place: Boston | org: Plone Foundation | source: S051 | ledger: L-4132 | confidence: observed | status: active

Training classes were spread across several locations, and attendees had to plan travel time between morning and afternoon sessions.
```

```{note} [specific · 2015 · Bucharest · 11 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2015 | place: Bucharest | org: Eau de Web | source: S046 | ledger: L-4114, L-4117 | confidence: reported | status: active

Training was included in the ticket price, with five courses of one or two days each.
The Foundation board left open whether this would become policy for future conferences.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2089 | confidence: observed | status: active

Training ran both at the venue and at the host company's office, with more than 50 participants.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1090, L-1092 | confidence: observed | status: active

Three two-day classes drew over 120 students, an idea that came from a trainer when the venue's classrooms were free.
At USD 175 per class (as of 2006, S009), about 15 students covered the room cost.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1091, L-1095 | confidence: observed | status: active

Trainings were financially separate: trainers paid the room rental and registered students themselves, which removed financial risk but confused some registrants.
The organizers would consider centralizing registration, and left a flat trainer rate undecided.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S086 | ledger: L-1093 | confidence: observed | status: active

In the evaluation, 28% called the trainings a strong influence on attending, and they rated 4.39 of 5.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1094 | confidence: observed | status: active

The organizers would consider dropping three-hour tutorials as long for students and hard to prepare, since 90 minutes is enough for most workshops.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S087 | ledger: L-1096 | confidence: observed | status: active

Several attendees said a session labeled tutorial should be hands-on with their own laptop and announced prerequisites, and otherwise be called a talk or demo.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S088 | ledger: L-1097 | confidence: hearsay | status: active

One trainee received no pre-training email and found no signs showing which room held which course on the first morning.
```

## Risks

```{warning} Trainer lodging and fee commitments exceed the budget
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Agree trainer terms and lodging in writing before announcing the training offer, and cost them at the worst-case number of trainers | owner-role: treasurer

The 2026 debrief named conference-funded trainer lodging near the venue as the largest financial risk.
Costs arise regardless of how long a session runs.
```

```{warning} A trainer does not appear
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Name a stand-in from experienced community members for every class before the first training day | owner-role: training-lead | playbook: speaker-dropout

One conference lost a presenter and relied on community members to cover the session.
```

```{warning} Trainees cannot find their class
:class: hb-risk hb-likelihood-medium hb-impact-low
risk | likelihood: medium | impact: low | mitigation: Email every trainee the room and the prerequisites, and post room signs before the first morning | owner-role: training-lead

An attendee at one conference received no instructions and found no room signs.
```

## Thin content

```{warning} No Foundation guideline on trainer compensation
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A Foundation guideline on trainer fees, lodging and tickets, or a recorded decision that none will exist | who-might-know: Foundation board; Conference Committee; past organizers | since: 2026-11-02

An organizer asked the Foundation for such guidelines in 2023 (S070), and the 2026 debrief still describes compensation as unregulated (S098).
This chapter offers a decision frame, not a rule.
```

```{warning} Effect of included training on revenue and trainer income
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Revenue and trainer-income figures from a conference that included training, set against one that sold it separately | who-might-know: Treasurers of past conferences; Foundation board | since: 2026-11-02

The pattern of including training is documented across conferences, but its financial effect is documented nowhere in the archive.
```

```{warning} Remote and hybrid training delivery
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Practice for delivering training to remote participants | who-might-know: Organizers of online and hybrid conferences; trainers who taught remotely | area: hybrid-online | since: 2026-11-02

This chapter covers in-person training.
See `hybrid-online` for the format as a whole.
```

```{warning} Trainer payment evidence is old
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: Current accounts of how trainers were paid and how room costs were shared | who-might-know: Recent training leads; trainers | since: 2026-11-02

The documented model, in which trainers paid the room rental and kept the fees, dates from 2006.
```

## Sources and further reading

- S004 Plone Foundation, Conference Planning Schedule.
- S009 Seattle 2006, "Things We Learned About Running a Plone Conference."
- S032 San Francisco 2011 wiki, "Assumptions and community expectations."
- S036 Arnhem 2012, organizer wrap-up.
- S046 Foundation board minutes of 2015-06-25, included training and trainer compensation.
- S049 Boston 2016 call for proposals.
- S050 Boston 2016 conference site and post-event note.
- S051 Boston 2016 attendee logistics.
- S054 Barcelona 2017 conference site.
- S055 Tokyo 2018 call for proposals.
- S070 Foundation board minutes of 2023-11-02, organizer's conference report.
- S073 Eibar 2023 conference site.
- S074 Results of the 2024 conference feedback survey.
- S079 Feedback, videos and photos from Plone Conference 2025.
- S086 Seattle 2006 overall conference evaluation.
- S087 Seattle 2006 agenda suggestions from attendees.
- S088 Seattle 2006 logistics suggestions from attendees.
- S098 Plone Conference 2026 facts and lessons for the handbook, organizers' debrief.
- S110 Maastricht 2026 attendee survey analysis.
