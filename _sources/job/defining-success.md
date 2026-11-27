---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to define success for a Plone Conference with an honest attendance picture, written goals, outcome measures and a survey that supports the next team."
    "keywords": "Plone, Plone Conference, success, attendance, goals, survey, planning"
---

# Defining success

## Why it matters

Without a written definition, success shrinks to a headcount, and headcounts are easy to inflate and hard to compare.
A team that budgets on the largest numbers in the history of the conference plans for an audience that the recurring community may not supply.

The 2026 debrief described the recurring in-person community as roughly one hundred people and potentially shrinking (S098, as of 2026-11).
That figure is an approximate planning hypothesis from one source, and the record does not yet hold comparable per-edition counts.
The Foundation's history page also shows the difficulty: it counts online-stream viewers next to on-site attendees for some years, and its two largest in-person editions were co-hosted with a regional Python conference (S002, as of 2026-11).

A definition of success written at the start protects the team and the next one.
It tells the community what the event is for, gives the treasurer a number to plan on, and lets the survey show whether goals were met.

## Applies when

- `all` Every conference needs goals, an attendance baseline and a way to learn afterward.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-1018, L-2055) **Do you write down what the conference is for before you build the program?** Seattle fixed four goals before it built a program, and Bristol stated its goals in the bid. (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-4089, L-4142, L-5010) **What planning number do you use for the recurring community, kept apart from local and partner audiences?** Forecasts in 2007 and 2018 ran above the reported outcome. (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Will you co-locate with a partner event?** Both 2024 and 2025 did (L-4214, L-4215). It adds attendance and talks, and it blurs the measure of the community. (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Will you set a goal for local activation, and who owns it?** A 2009 host company noted that few local users attended and called a local meetup afterward (L-4109). (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-1019, L-4183, L-4218) **Will you survey attendees and publish the results?** Editions in 2006, 2023 and 2025 each reported survey results. (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Will you count remote viewers, and report them apart from on-site attendees?** The history page lists both and does not make them comparable (L-4021). (decide-by: T-6m)

## How-to

### Set the definition

1. Write three to five goals in plain language, for example who the event teaches, whom it connects and what it shows.
   Done looks like a one-page statement that the team and its advisers have read.
1. Attach one measure to each goal that you can collect, such as a count, a survey question or an outcome.
   Done looks like a table with a goal and a measure per row.
1. Estimate the recurring community separately from local and partner audiences, and write down the method.
   Done looks like two numbers in the budget, not one.
1. Define what you count: on-site attendees, speakers, sponsors, sprinters, remote viewers.
   Done looks like a definitions line that travels with every published number.

### Measure and report

1. Draft the survey before registration opens, with questions tied to your goals and not only an overall score.
   Expect roughly one in five ticket holders to answer, and pick measures that a response of that size can still answer (L-6002).
   Done looks like a survey that maps question by question to the measures.
1. Send the survey right after the conference and set the publication date before you send it.
   Done looks like a dated results post.
1. Have someone challenge your reading of the survey before you publish it.
   In 2026, three review rounds found two interpretations that the data contradicted and corrected several counts (L-6005).
   Done looks like a reading that names the evidence behind each claim.
1. Publish the counts with their definitions and the composition of the audience.
   Done looks like an entry in the `conference-data-table` format.
1. Hand the goals, numbers and survey to the next team through the `handover-contract`.
   Done looks like files in the handover package.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S069, S079, S086 | ledger: L-1019, L-4183, L-4218 | confidence: reported | status: active | basis: independent-conferences

Survey attendees after the conference and publish the results.
The editions on record that did so reported high ratings.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S002, S077, S079, S098 | ledger: L-4021, L-4214, L-4215, L-5010 | confidence: reported | status: active | basis: independent-conferences

Estimate the recurring community apart from local and partner audiences.
Attendance added by a partner event or by reduced local tickets does not show how large the community is.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S010, S055, S057 | ledger: L-4080, L-4089, L-4142 | confidence: observed | status: active | basis: independent-conferences

Bid and prospectus numbers ran above the reported outcome in 2007 and 2018, and the Foundation lowered its venue minimum from 250 to 200 for 2018.
Plan the budget on the lower figure.
```

A pre-bid community survey that collected the wisdom of past conferences and gave one team a clear idea of success (L-1016) comes from one conference and is not promoted.

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6015, L-6041 | confidence: observed | status: active

The attendee survey's overall rating averaged 4.57 of 5, with 15 of 21 respondents giving the top score.
Asked about attending in Bucharest in 2027, 16 said yes, 2 perhaps and 3 probably not.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6007, L-6042 | confidence: reported | status: active

The respondents skewed toward insiders: 10 of the 11 who answered the relationship question were already active in the community.
The three who skipped the why-attend profile were the three probably-nots for 2027, so return intent is survivor-biased.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S098 | ledger: L-5011 | confidence: hearsay | status: active

The debrief described the recurring in-person community as roughly a hundred people and potentially shrinking, as an approximate hypothesis awaiting per-edition evidence.
```

```{note} [specific · 2025 · n/a · 1 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2025 | place: n/a | org: Plone Foundation | source: S002 | ledger: L-4021 | confidence: reported | status: active

The history page counts stream viewers beside on-site attendees for 2022 and 2023, and its two largest in-person editions, 2013 and 2024, were both co-hosted with a regional Python conference.
```

```{note} [specific · 2025 · Jyväskylä · 1 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2025 | place: Jyväskylä | org: University of Jyväskylä | source: S079 | ledger: L-4215 | confidence: reported | status: active

The conference was co-located with a revived national Python conference, with one day of Python talks; an attendee met people who became interested in Plone.
```

```{note} [specific · 2025 · Jyväskylä · 1 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2025 | place: Jyväskylä | org: University of Jyväskylä | source: S079 | ledger: L-4218 | confidence: reported | status: active

The overall feedback score was 4.87 out of 5.
```

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S078 | ledger: L-4210 | confidence: observed | status: active

The survey results were announced about ten weeks after the conference ended.
```

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S077 | ledger: L-4214 | confidence: observed | status: active

The conference was held together with a regional Python conference, following the 2013 Brasília model.
```

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S074 | ledger: L-4204 | confidence: reported | status: active

Survey comments emphasized the in-person sense of community and the networking opportunities more than any single session.
```

```{note} [specific · 2023 · Eibar · 3 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2023 | place: Eibar | org: CodeSyntax | source: S069 | ledger: L-4183 | confidence: reported | status: active

The attendee feedback survey gave the conference an overall score of 4.6 out of 5.
```

```{note} [specific · 2018 · Tokyo · 8 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2018 | place: Tokyo | org: Plone Conference 2018 Steering Committee | source: S057 | ledger: L-4142 | confidence: observed | status: active

The sponsor prospectus expected about 200 participants, roughly 90% from overseas; the history page later reports around 150.
```

```{note} [specific · 2017 · n/a · 9 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2017 | place: n/a | org: Plone Foundation | source: S055 | ledger: L-4080 | confidence: observed | status: active

The 2018 call lowered the minimum venue capacity from 250 to 200 people, the first downward adjustment in the calls archived.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S016 | ledger: L-2033 | confidence: observed | status: active

The organizer agreed that circumstances differ every year, such as the economy and competing regional events, so raw attendance comparisons between conferences are unfair.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S019 | ledger: L-2055 | confidence: observed | status: active

The host company's goals were to promote Plone, Python and open source in the host country and city, and to use the conference as a marketing opportunity toward organizations.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S021 | ledger: L-2067 | confidence: reported | status: active

An outside observer placed attendance in the middle of the 2006 to 2010 range and attributed the gap to the weak economy.
```

```{note} [specific · 2009 · Budapest · 17 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2009 | place: Budapest | org: Greenfinity | source: S014 | ledger: L-4109 | confidence: observed | status: active

The host company noted that only a few users from the host country attended, and called a local meetup to turn the conference's momentum into local activity.
```

```{note} [specific · 2008 · Washington, D.C. · 18 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2008 | place: Washington, D.C. | org: ZPUGDC | source: S012 | ledger: L-4099 | confidence: observed | status: active

Organizers had wondered how many people would travel from abroad to a US conference and saw a good turnout from Europe and some from Australia and Japan.
```

```{note} [specific · 2007 · Naples · 19 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2007 | place: Naples | org: Abstract Open Solutions | source: S010 | ledger: L-4089 | confidence: observed | status: active

The bid planned for up to 700 participants; the history page later reports just over 400.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S085 | ledger: L-1017 | confidence: observed | status: active

In the pre-conference survey of about 213 respondents, connecting community members was the highest-rated goal at 4.41 of 5, ahead of teaching current technology at 4.23.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1018 | confidence: observed | status: active

Before building the program the organizers fixed four goals: teach beginning and intermediate users, showcase sectors and regions using Plone, strengthen person-to-person connections and keep a relaxed, grassroots feel.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S086 | ledger: L-1019 | confidence: observed | status: active

The evaluation measured outcomes: 91% rated the conference very good or excellent, 98% felt more connected to the community, 83% felt more empowered to contribute and 42% planned to start contributing code.
```

## Risks

```{warning} The budget rests on an attendance forecast the community does not reach
:class: hb-risk hb-likelihood-high hb-impact-high
risk | likelihood: high | impact: high | mitigation: Budget on the recurring-community number and set dated sales checkpoints with a decision for each | owner-role: treasurer | playbook: low-ticket-sales

Bids and prospectuses ran above the outcome at several editions.
The judgment is for a typical mid-size conference.
```

```{warning} Partner-event attendance is read as community growth
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Publish every attendance figure with its definition and split partner-event attendance from community attendance

A later team that reads the raw number plans for an audience that does not return.
```

## Thin content

```{warning} The community size rests on one debrief
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Per-edition counts that separate community members, partner-event audiences, local and reduced tickets, speakers and sponsors | who-might-know: Past organizers; Conference Committee; Foundation Board | area: other | since: 2026-11-02

The figure of about one hundred people comes from the 2026 debrief only.
```

```{warning} Effect of local activation is unmeasured
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Evidence on whether meetups, university outreach and local ticket programs turned local attendees into community members | who-might-know: Past organizers; local user groups | area: other | since: 2026-11-02

One 2009 account is the only archived record here, and it records a gap, not a result.
```

```{warning} Outcome measures rest on Seattle 2006
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Survey designs from later editions that measured outcomes and goals, not only overall satisfaction | who-might-know: Past organizers; survey authors of recent editions | area: other | since: 2026-11-02

Later editions report overall scores, and only the 2006 survey is on record as measuring goal outcomes.
```

## Sources and further reading

- S002 Plone Conference history 2003 to 2024, as of 2026-11.
- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
- S010 Official Naples 2007 conference record.
- S012 Contemporary report on the 2008 conference in Washington, D.C.
- S014 Post-conference community note on the 2009 conference, Budapest.
- S016 Plone Conference 2010, "The Numbers".
- S019 Official Bristol 2010 conference record and original proposal.
- S021 Plone Metrics assessment of the 2010 conference.
- S055 2018 Call for Proposals.
- S057 Tokyo 2018 sponsorship program.
- S069 "Reflecting on Plone in 2023", conference statistics and feedback score.
- S074 Results from the 2024 conference feedback survey.
- S077 Official Plone Conference 2024 record.
- S078 Community announcement of the 2024 survey results.
- S079 Feedback, videos and photos from Plone Conference 2025.
- S085 Seattle 2006 pre-conference survey.
- S086 Seattle 2006 overall conference evaluation.
- S098 Plone Conference 2026 facts and lessons for the handbook, internal debrief record.
- S110 Maastricht 2026 attendee survey analysis.
