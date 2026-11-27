---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to build the day-by-day schedule: the Foundation meeting slot, rooms, tracks, breaks and lightning talks, and what to freeze early."
    "keywords": "Plone, Plone Conference, schedule, agenda, annual meeting"
---

# Scheduling

## Why it matters

The schedule is the product attendees actually consume.
It decides who can see which session, whether they can change rooms, eat and talk to peers, and whether the sessions they care about collide.

It is also where fixed obligations meet the program.
The Plone Foundation holds its annual member meeting at the conference, so the grid has to reserve that slot before anything else is placed.
Getting its length or its remote access wrong is hard to repair once speakers and attendees have planned around a frozen grid.

Late changes cost trust with speakers who have booked travel and with attendees who chose days by the published agenda.
Sessions chosen in [CFP and selection](cfp-and-selection.md) and shaped in [Programme portfolio](programme-portfolio.md) arrive here as a list that has to fit rooms, time and people.

## Applies when

- `all` Every conference with more than one session has a schedule to build.

## Decisions you must make

- {bdg-danger}`MUST` (req: R-015; as-of: 2026-11-02) **Does the published schedule include the Foundation annual member meeting?**
  Reserve a slot for the annual member meeting, which the Foundation holds once a year at the conference.
  Place it before the grid is built around other sessions.
  (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-5026, L-4113) **How long is the annual meeting slot, and does it need remote access?**
  Resolve duration and remote-access expectations through the Foundation confirmation process before freezing the schedule (L-5026, S106).
  A 2026 debrief reports that a 25-minute slot proved insufficient, and register row R-034 holds the question as unverified as of 2026-11-02.
  (decide-by: T-3m)
- {bdg-secondary}`OPTION` **How many sessions run in parallel?**
  One team advises three to five in place of two (L-1078), another ran four rooms over two days (L-2041).
  Let room count follow program size and venue.
  (decide-by: T-6m)
- {bdg-primary}`DEFAULT` (basis: L-1082, L-2097, L-4205) **How long are changeovers and breaks?**
  Plan more than five minutes between sessions and 30-minute main breaks.
  A 2024 survey asked for punctual sessions and enough breaks.
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Where do lightning talks go, and how long are they?**
  Rows from one conference suggest an hour per session at three to four minutes a talk (L-2099, L-2100).
  Sessions filled the room and grew from day to day (L-2096).
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Which tool builds and publishes the schedule?**
  One organizer advises paying for a hosted service over building one (L-3035).
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Which sessions are recorded or streamed, and does that constrain rooms or slots?**
  Room choice and slot length follow recording needs; see `av-recording-internet` and `hybrid-online`.
  (decide-by: T-3m)
- {bdg-secondary}`OPTION` **When does the draft go to speakers and the full agenda to the public?**
  Circulate the draft to speakers first (L-1079) and publish as early as accepted sessions allow.
  (decide-by: T-3m)

## How-to

### Before the grid
1. Collect the fixed slots: Foundation annual meeting, keynotes, meals, social events and the closing lightning talks.
   Done: a fixed-slot list with durations.
2. Confirm the annual meeting's duration and remote access with the Foundation.
   Done: a written answer, dated, in the planning folder.
   The Foundation meetings page states that member meetings are held once a year and coincide with the conference (L-4063; S007, as of 2026-11).
3. Check the candidate dates against major religious and national holidays; see `master-timeline`.
   Done: the dates are cleared or the conflict is recorded.
4. Set the slot template: session length, changeover, breaks and lunch.
   Done: a one-page timing template.
5. List rooms with capacity, projection and recording capability, and assign sizes using attendee interest data.
   Done: a room list, with the expectation that slots will move, because interest data keeps changing (L-3039; S026).

### Building the grid
6. Place keynotes and the fixed sessions first.
   Done: the draft grid shows them.
7. Place accepted sessions to balance ability levels, keep the best-known presenters apart and fit rooms.
   Done: a full draft grid.
8. Spread panels and other heavy formats across the days.
   Done: no day carries most of one format.
9. Have a second person who knows every session check pacing and sequence.
   Done: the second reader has signed off.

### Publishing and changes
10. Circulate the draft to speakers with a reply date.
    Done: replies are logged.
11. Publish the grid and link the grid view from the home page.
    Done: the public page matches the final draft.
12. Set a date after which a slot move needs the program lead.
    Done: the rule is written down and shared with speakers.

## Principles and general lessons

Three principles have passed the promotion rule on structural reasons.
Five further pieces of advice rest on one conference each and are tracked here until independent evidence arrives:

- Run three to five parallel sessions rather than two, with at least three tracks loosely defined by skill level (L-1078, L-1080; S009).
- Put longer sessions in the morning and keep the afternoon fast-paced (L-1085; S009).
- Do not require advance signup to attend sessions (L-1086; S009).
- Give lightning talks three to four minutes rather than seven, and allow one hour per session rather than 45 minutes (L-2099, L-2100; S036).
- Pay for a hosted scheduling service rather than building one (L-3035; S026).

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009, S087 | ledger: L-1081, L-1083 | confidence: observed | status: active | basis: structural | reason: Two sessions held at the same time cannot both be attended, so overlap costs attendance at both.

End each day with lightning talks and birds-of-a-feather sessions, in consecutive slots and never at the same time.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009, S036 | ledger: L-1082, L-2097, L-2098 | confidence: observed | status: active | basis: structural | reason: Moving between rooms and talking with people takes physical time that depends on the venue layout, not on the year.

Leave at least five minutes between sessions, more where rooms are far apart, and make the main breaks 30 minutes rather than 15.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S087 | ledger: L-1087 | confidence: observed | status: active | basis: structural | reason: Travel and leave are booked months ahead and are costly to change, whatever the year.

Publish the full agenda months before the conference, so attendees can plan travel around the days that matter to them.
```

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6027, L-6046, L-6047 | confidence: reported | status: active

Two respondents independently reported that speakers could not attend roundtables and panels that overlapped their own slots, and fixing that leads the survey's start list.
Respondents kept the two-room parallel structure, the pace, the open spaces and the buffers between talks; one asked for 3-minute lightning talks, as Arnhem 2012 advised (L-2099).
```

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S074 | ledger: L-4205 | confidence: reported | status: active

Several survey respondents asked for punctual sessions and enough breaks between them.
```

```{note} [specific · 2014 · Bristol · 12 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2014 | place: Bristol | org: Netsight | source: S045 | ledger: L-4113 | confidence: observed | status: active

The Foundation's annual business meeting was held during the conference, on the Friday around midday.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2096 | confidence: observed | status: active

Lightning-talk sessions grew each day, from 8 talks to 17 and then 14, and the room was full every day.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S026 | ledger: L-3036 | confidence: observed | status: active

The hosted schedule service had shortcomings: talks could not be edited after submission, the mobile version was not worth paying for, and the default schedule view confused some people. The team linked the grid view from the home page.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S017 | ledger: L-2041 | confidence: observed | status: active

About 48 talks ran in four parallel rooms over two days. The lightning-talk session was oversubscribed, so a second one was added on the open-space day.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S017 | ledger: L-2044 | confidence: observed | status: active

On the open-space day, held the morning after the party, the first slot attracted only one proposal. Rooms were split into eight spaces, of which only a few had projectors and filming.
```

```{note} [specific · 2009 · Budapest · 17 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2009 | place: Budapest | org: Greenfinity | source: S013 | ledger: L-4106 | confidence: reported | status: active

Foundation board elections ran online and in person during the conference days.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1076 | confidence: observed | status: active

The day-by-day agenda balanced ability levels, avoided putting the best-known presenters against each other, fitted sessions to room sizes and included as many top-ranked sessions as possible.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1077 | confidence: observed | status: active

Building the agenda took several days of intense work by one organizer. A second person who knew every session and presenter was extremely helpful for pacing and sequencing.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1079 | confidence: observed | status: active

The draft schedule was circulated to speakers for comment before publication, and only minor changes followed.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S088 | ledger: L-1084 | confidence: observed | status: active

Several attendees found five-minute breaks too short to change rooms or talk to people. Read this as the floor for changeovers, not the target.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S087 | ledger: L-1088 | confidence: observed | status: active

Placing most case-study panels on one day crowded that day with conflicts. Several attendees asked to spread them over the conference.
```

## Risks

```{warning} The annual meeting slot is too short or lacks remote access
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Obtain the Foundation's expectations on duration and remote access in writing before the grid freezes and reserve the slot first | owner-role: program lead

Judgment holds for a typical mid-size conference.
```

```{warning} A schedule change after publication breaks speaker travel plans
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Circulate a draft to speakers, publish early and require program-lead approval for any slot move after publication | owner-role: program lead


```

```{warning} A speaker withdraws after the grid is published
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Keep wait-listed sessions and a spare lightning-talk or open space slot that can absorb the gap | owner-role: program lead | playbook: speaker-dropout


```

## Thin content

```{warning} Annual meeting duration and streaming rule
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Foundation confirmation of the required duration and streaming for the annual member meeting (register row R-034) | who-might-know: Foundation board; Foundation Conference Committee

No Foundation page read states a duration or a streaming rule, so the slot length stays a DEFAULT, not a MUST.
```

```{warning} Single-conference scheduling advice
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Second accounts for parallel session counts, morning and afternoon pacing, lightning-talk length and scheduling tools | who-might-know: Past program chairs; past schedule builders

Five items in the principles section rest on one conference each.
```

```{warning} Scheduling across time zones
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Evidence on building a schedule for remote attendees in several time zones | who-might-know: Organizers of online and hybrid conferences | area: hybrid-online

No archived source describes time-zone choices.
```

## Sources and further reading

- S007 Board and Member Meetings archive.
- S009 Things We Learned About Running a Plone Conference.
- S013 Contemporary conference announcement and context.
- S017 Plone Conference 2010 Wrapup.
- S026 Wiki: Talks and Scheduling.
- S036 Plone Conference 2012 Wrap-up: organizer account.
- S045 2014 Membership Meeting and annual report.
- S074 Results from the 2024 Conference feedback survey.
- S087 Seattle 2006 agenda suggestions.
- S088 Seattle 2006 logistics suggestions.
- S106 Foundation requirements register.
- S110 Maastricht 2026 attendee survey analysis.
