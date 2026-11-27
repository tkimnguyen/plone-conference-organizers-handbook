---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [format]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to decide whether a Plone conference offers remote access, from recordings only to full online, and what past online and hybrid editions learned."
    "keywords": "Plone, Plone Conference, hybrid, online, livestream, remote participation"
---

# Hybrid and online

## Why it matters

Some people cannot travel, and some conferences cannot meet in person.
The Plone community has run fully online editions and in-person editions with remote access, and the experience differs a lot between them.

Remote access also costs effort and carries a worry.
Organizers have feared that a live stream would keep people from traveling, while others see remote access as the only way for some community members to take part.
The evidence on that point is thin, and this chapter says so.

Recording and publishing sessions are in [AV, recording and internet](../on-site-production/av-recording-internet.md).
The footprint side of travel is in [Sustainability](sustainability.md).

## Applies when

- `format` Applies to every conference, since an in-person team also decides about remote access, and the content varies by format.

## Decisions you must make

- {bdg-secondary}`OPTION` **Which participation model do you offer: recordings only, live stream with chat, hybrid or fully online?**
  Bristol declined live streaming and promised fast recordings (L-2015), Namur streamed with a chat channel and delayed recordings (L-4179), and the 2020 and 2021 editions ran fully online (L-4163, L-4168).
  (decide-by: T-9m)
- {bdg-secondary}`OPTION` **How will streaming support remote access, and do you accept that it might affect in-person participation?**
  The 2026 debrief raises substitution as a possibility but supplies no measured effect (L-5028).
  Make the choice explicit, whichever way it goes.
  (decide-by: T-9m)
- {bdg-secondary}`OPTION` **How do remote attendees ask questions and meet people?**
  Namur used a chat channel (L-4179).
  An organizer of both online editions said the platform could not recreate hallway encounters (L-4180).
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Do you offer trainings online?**
  A 2024 survey called online training logistically challenging and asked for better integration (L-4202).
  The 2020 edition moved training to a weekend (L-4164).
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Which platform do you use, and who provides it?**
  The 2021 edition used a platform from a sponsoring company (L-4168).
  (decide-by: T-4m)
- {bdg-secondary}`OPTION` **Do you invite community members with their own equipment to cover extras?**
  A Seattle volunteer recorded lightning talks and interviews that the professionals could not cover (L-1128).
  (decide-by: T-3m)

## How-to

1. Write down the participation model and its reasons.
   Done: a one-page decision with an owner, shared with the program and AV leads.
2. For a live stream, set up a question path for remote viewers, for example a chat channel watched by a volunteer (L-4179; S068).
   Done: a named person relays questions to the session chair.
3. Plan fast publication of the recordings, so viewers outside the venue are not left waiting (L-2015; S015).
   Done: a publication date agreed with the recording owner.
4. For training, test the online logistics before the date and decide how remote and in-room participants share exercises (L-4202; S074).
   Done: a trainer checklist covering audio, shared screens and breaks.
5. For an online edition, choose the platform early and check whether a sponsor can provide it (L-4168; S064).
   Done: a written platform decision.
6. Tell remote attendees up front what they will miss, since talks transfer well while hallway talk and sprint work do not (L-4178; S068).
   Done: a short note on the program page.

## Principles and general lessons

No general lesson has passed the promotion rule yet.
One piece of advice rests on one discussion and is tracked until independent evidence arrives:

- Community members who attended both formats say talks are much the same online, but remote attendees miss real-time questions in training, hallway conversations and the sprint (L-4178; S068).

## Case notes

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S074 | ledger: L-4202 | confidence: reported | status: active

Online training was logistically challenging, and respondents asked for better integration of online and in-person participants.
```

```{note} [specific · 2022 · Namur · 4 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2022 | place: Namur | org: iMio and Affinitic | source: S068 | ledger: L-4179 | confidence: observed | status: active | context: format=hybrid

The conference focused on in-person attendees.
Talks were live-streamed, remote participants asked questions in a chat channel, and recordings followed after a delay.
```

```{note} [specific · 2021 · Online · 5 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2021 | place: Online | org: Plone Foundation | source: S068 | ledger: L-4180 | confidence: observed | status: active | context: format=online

An organizer of the 2020 and 2021 online editions reflected that, despite efforts, the event platform could not recreate chance encounters in the hallway.
```

```{note} [specific · 2021 · Online · 5 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2021 | place: Online | org: Plone Foundation | source: S064 | ledger: L-4168 | confidence: reported | status: active | context: format=online

The conference was again fully online, on an event platform provided by a sponsoring company.
```

```{note} [specific · 2020 · Online · 6 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2020 | place: Online | org: Plone Foundation | source: S062 | ledger: L-4163 | confidence: observed | status: active | context: format=online

Because of the pandemic, the Foundation board canceled the physical conference and ran it entirely online.
```

```{note} [specific · 2020 · Online · 6 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2020 | place: Online | org: Plone Foundation | source: S062 | ledger: L-4164 | confidence: observed | status: active | context: format=online

The online format kept the week but moved training to a weekend, ran four days of talks plus one day of open spaces, then a weekend sprint.
```

```{note} [specific · 2020 · Online · 6 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2020 | place: Online | org: Plone Foundation | source: S063 | ledger: L-4165 | confidence: observed | status: active | context: format=online

The online conference took place three weeks later than first announced.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S015 | ledger: L-2015 | confidence: observed | status: active

Requests for live streaming were declined because the organizers feared streaming would deter in-person attendance.
They committed to fast publication of recordings instead.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1128 | confidence: observed | status: active

A community volunteer with their own equipment recorded sessions the professionals could not cover and streamed some sessions live into a virtual world.
```

## Risks

```{warning} Streaming reduces in-person attendance
:class: hb-risk hb-likelihood-low hb-impact-medium
risk | likelihood: low | impact: medium | mitigation: State your position on streaming before registration opens and compare registrations with expectations as the date nears | owner-role: program lead

The evidence is a stated fear in 2010 and a 2026 debrief remark, with no measurement.
```

```{warning} The format changes to online at short notice
:class: hb-risk hb-likelihood-low hb-impact-high
risk | likelihood: low | impact: high | mitigation: Keep cancellation terms and a fallback date in the venue contract and decide who can call the switch | owner-role: conference chair | playbook: force-majeure

The 2020 edition moved online and ran three weeks later than first announced.
```

```{warning} Remote attendees get a second-class experience
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Provide a question path, publish recordings quickly and say plainly what remote attendees will miss | owner-role: program lead

Remote attendees reported missing real-time questions, hallway talk and the sprint.
```

```{warning} Online training logistics fail
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Test audio, shared screens and exercise handling with each trainer before the date | owner-role: training lead

A 2024 survey called online training logistically challenging.
```

## Thin content

```{warning} A tested hybrid delivery model
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A tested hybrid setup with equipment, roles, moderation and costs from a conference that ran it | who-might-know: AV and program leads of the 2020 to 2022 editions | area: hybrid-online

No account archived here describes a full hybrid setup, only a stream with chat.
```

```{warning} Effect of streaming on attendance
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Registration and attendance data from conferences with and without a live stream | who-might-know: Registration leads and treasurers of past conferences | area: hybrid-online

Only a stated fear and an unmeasured debrief remark exist.
```

```{warning} Online training practice
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Trainer accounts of online and hybrid training with tools and methods that worked | who-might-know: Trainers of the 2020 to 2024 editions | area: hybrid-online

One survey summary supports the training advice.
```

## Sources and further reading

- S009 Things We Learned About Running a Plone Conference, Seattle 2006.
- S015 Plone Conference 2010, an organizer's view.
- S062 Announcement of the move to an online conference, 2020.
- S063 Official post-event conference record and schedule, 2020.
- S064 2021 conference video and platform recap.
- S068 Community discussion comparing online and in-person conference experiences.
- S074 Results from the 2024 conference feedback survey.
- S098 Plone Conference 2026 facts and lessons for the handbook.
