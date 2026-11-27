---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to decide which products make up the conference week, which session formats to offer and how they fit together."
    "keywords": "Plone, Plone Conference, program, session formats, portfolio"
---

# Programme portfolio

## Why it matters

The program is the reason people travel.
Venue, tickets, marketing and sponsors all serve a set of sessions that someone has to design as a whole before the first call goes out.

Past conferences covered related technologies, accessibility, user experience, documentation and community organizing, and served as meeting places for special-interest groups such as universities and NGOs (L-4086, S096).
A team that treats the program as a list of talks misses most of that range.

Without an explicit portfolio, trainings, talks, business days and sprints compete for the same rooms, volunteers and attention.
Each product then gets its own call, price and audience by accident.
The cost shows up as thin rooms, double-booked helpers and sponsors who cannot tell what they are paying to reach.

The Foundation, speakers, sponsors, the venue and volunteers are all touched by these choices.
They fix the scope that [CFP and selection](cfp-and-selection.md), [Scheduling](scheduling.md) and [Keynotes and invited talks](keynotes-and-invited-talks.md) then work inside.

## Applies when

- `all` Every conference has a program, and its shape drives every other workstream.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-4088, L-4213) **Which products fill the week?**
  Name each product (trainings, conference days, sprints, and any business track) with its own audience, owner and call.
  Bids and recaps from different conferences show the same week-long shape of trainings, conference days and sprints.
  (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-2051, L-4213) **Which session formats go beyond regular talks?**
  Plan regular talks, lightning talks and open space as a set, because they serve different attendees.
  Attendees at one conference judged that mix well selected, and another delivered it at scale.
  (decide-by: T-12m)
- {bdg-secondary}`OPTION` **How many days of conference talks?**
  A three-day talk schedule is a suggested design in past calls for proposals, but no Foundation page confirms it (register row R-019, unverifiable as of 2026-11-02).
  (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Will another event share the program?**
  Co-locating adds audience and shares costs, but it gives away program space (L-3112).
  See `business-and-side-tracks` for the 2025 co-location.
  (decide-by: T-12m)
- {bdg-secondary}`OPTION` **How are sessions grouped into tracks?**
  Options seen are by topic (L-4139) or by skill level, which `scheduling` covers.
  (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Which languages do sessions run in?**
  One conference ran most sessions in English and a minority in the host region's language (L-4173).
  (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Is there a community strategy or roadmap session?**
  A strategic open space produced a community roadmap (L-4111).
  (decide-by: T-6m)

## How-to

1. Write three to five attendee goals as plain sentences.
   Done: the program committee has signed off the goals page.
2. List every product of the week and give each an audience, an owner and a call date.
   Done: a one-page product table.
   Chapters: `trainings`, `business-and-side-tracks`, `sprints`, `social-events-and-party`.
3. Derive session types from the goals, so every goal has at least one session type that serves it.
   Done: a table of goal, session type and format.
4. Decide how sessions group into tracks and sketch the number of parallel rooms.
   Done: a track list handed to [Scheduling](scheduling.md).
5. Reserve fixed slots before opening any call: the Foundation annual meeting, keynotes and social events.
   Done: the slots appear in a draft grid.
6. Write one call per product from `cfp-template`, each with its own deadline, following [CFP and selection](cfp-and-selection.md).
   Done: calls published.
7. Compare accepted sessions with the goals once selection ends.
   Done: a gap list, filled with invited sessions from [Keynotes and invited talks](keynotes-and-invited-talks.md).

## Principles and general lessons

No general lesson has passed the promotion rule yet.
Two pieces of advice rest on one conference each and are tracked here until independent evidence arrives:

- One organizing team advises a strong focus on sector-specific users, because education and government attendees came in especially strong numbers (L-1058, S009).
- The same team advises more facilitated workshop sessions on shared community problems, led by a strong facilitator, with a broader part of the community in planning (L-1059, S009).

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6038 | confidence: observed | status: active

Of 18 respondents profiling why they attend, 9 come technology-first but appreciate context and business talks, 6 come equally for both, 2 want deep technical content only and 1 came mainly for business.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6040, L-6053 | confidence: reported | status: active

The analyst's opinion, not a data finding: keep the broadening keynotes and practical AI content, make the technical core unmistakably strong and treat AI as one topic among many.
One respondent suggested a co-located PyCon day.
```

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S076 | ledger: L-4213 | confidence: reported | status: active

The program had 12 trainings, 80 talks, 3 keynotes, 30 lightning talks, open spaces and a yoga session, delivered by more than 80 speakers.
```

```{note} [specific · 2022 · Namur · 4 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2022 | place: Namur | org: iMio and Affinitic | source: S066 | ledger: L-4173 | confidence: reported | status: active

Of 60 presentations, 45 were in English and 15 in French, the language of the host region.
```

```{note} [specific · 2017 · Barcelona · 9 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2017 | place: Barcelona | org: Iskra SCCL | source: S054 | ledger: L-4139 | confidence: observed | status: active

Barcelona offered three tracks: Plone, Python web technologies and modern JavaScript frontends.
```

```{note} [specific · 2014 · Bristol · 12 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2014 | place: Bristol | org: Netsight | source: S044 | ledger: L-4111 | confidence: reported | status: active

A strategic open space used sticky-note brainstorming to gather a large crowd's ideas. It produced a community roadmap with surprising consensus.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S094 | ledger: L-3112 | confidence: observed | status: active

A bid gave four reasons to run the conference side by side with a national Python conference: reach a broader audience, lower operating costs for both events, offer better sponsorship packages and have more fun. It followed a regional Plone symposium held together with that event.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S094 | ledger: L-3126 | confidence: observed | status: active

The bid committed to balancing open spaces with traditional talks and to giving lightning talks generous time, as low-barrier ways to get involved.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S040 | ledger: L-3129 | confidence: observed | status: active

The program included a Show Me How session where attendees brought their Plone problems and experts demonstrated solutions.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S018 | ledger: L-2051 | confidence: observed | status: active

From the attendee side, the mix of regular talks, lightning talks and open space was judged well selected. It ranged from technical to social topics and from beginners to developers.
```

```{note} [specific · 2009 · Budapest · 17 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2009 | place: Budapest | org: Greenfinity | source: S013 | ledger: L-4103 | confidence: reported | status: active

Open Space sessions were added alongside the talk tracks for the first time, to allow more interaction between presenters and listeners.
```

```{note} [specific · 2007 · Naples · 19 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2007 | place: Naples | org: Abstract Open Solutions | source: S010 | ledger: L-4088 | confidence: observed | status: active

The bid laid out two training days, three conference days and three sprint days, the week-long shape later conferences kept.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1056 | confidence: observed | status: active

The program kept the established format of short talks, longer tutorials, keynotes, lightning talks and birds-of-a-feather sessions. It derived its session types from the goals: evergreen basics by the best teachers, emerging technology, non-technical implementation topics, community and roadmap sessions, and sector case-study panels.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S085 | ledger: L-1057 | confidence: observed | status: active

In a pre-conference survey, sessions for beginning, intermediate and advanced users scored highest of the tested program ideas (4.26 of 5). A community strategy workshop (3.98), facilitated problem-solving groups (3.96) and a newcomer sprint (3.92) followed, with open space lowest (3.62).
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S086 | ledger: L-1060 | confidence: observed | status: active

Asked about formats for future conferences, 44% wanted more 90-minute tutorials and 40% more workshop sessions. 25% wanted fewer three-hour tutorials and 23% fewer case-study panels.
```

## Risks

```{warning} A core audience has no sessions
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Compare accepted sessions with the written attendee goals before the schedule freezes and fill gaps with invited sessions | owner-role: program lead

Selection by merit alone can leave a goal, such as beginner content, uncovered.
```

```{warning} Products compete for the same rooms and volunteers
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Give every product an owner and reserve its rooms and helper hours in the draft grid before any call opens | owner-role: program lead

Trainings, talks and sprints draw on one venue and one volunteer pool.
```

## Thin content

```{warning} Number of conference days
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A Foundation or organizer statement of the preferred number of conference talk days | who-might-know: Foundation Conference Committee; past organizers

Register row R-019 stays unverifiable as of 2026-11-02, so the day count is an option here.
```

```{warning} Audience focus and facilitated workshops
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second conference account that tested sector focus or facilitated community workshops | who-might-know: Past program chairs; sector working groups

Both pieces of advice in the principles section come from one team.
```

```{warning} Format reception evidence is old
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: Attendee survey data on format preference from conferences within the last eight years | who-might-know: Past survey owners; Foundation Conference Committee

Most format evidence comes from conferences more than eight years before the 2026 pin.
```

## Sources and further reading

- S009 Things We Learned About Running a Plone Conference.
- S010 Official Naples 2007 conference record.
- S013 Contemporary conference announcement and context.
- S018 Plone Conference 2010: a retrospect, attendee perspective.
- S040 Official announcement: Plone Conference 2013 coming to Brasília.
- S044 Plone 2020: documented strategic open-space results.
- S054 Barcelona 2017 conference site.
- S066 Plone Conference 2022 recap.
- S076 Plone Conference 2024 recap.
- S085 Seattle 2006 pre-conference survey.
- S086 Seattle 2006 overall conference evaluation.
- S094 Brasília 2013 conference proposal.
- S096 2020 Call for Proposals: the most recent hosting call located.
- S110 Maastricht 2026 attendee survey analysis.
