---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to plan the network, projectors, session recording and publication for a Plone conference, and what has failed before."
    "keywords": "Plone, Plone Conference, AV, recording, Wi-Fi, internet, video"
---

# AV, recording and internet

## Why it matters

Plone attendees work on laptops and expect the network to carry more than web and mail.
When it fails on the first morning, the program and the mood of the event suffer.

Recording is the second half of the topic.
Sessions nobody can watch afterward are lost to people who could not travel and to those who missed a parallel track.
Recording takes hardware, hands and a named owner.

AV and video were the largest cost group at one past conference (as of 2010, S016), a network failure costs trust, and missing footage cannot be recovered.
For live access by remote viewers, see [Hybrid and online](../formats-and-values/hybrid-online.md).

## Applies when

- `all` Every conference needs a network, projection and a decision about recording.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-2016, L-4070, L-4174) **Will you record sessions and publish them fast?**
  Register row R-016 (verified-current, as of 2026-11-02) records the call-for-proposals guidance, which strongly encourages recording as many sessions as possible with fast turnaround, and treats live streaming as optional.
  (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-3084, L-5025) **Who owns recording, and who is their deputy?**
  Give recording its own workstream and task list, separate from the program.
  (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-1115, L-4096, L-2076) **Can the network carry every attendee connecting at once, and is that in writing?**
  Ask for capacity, address pool size and open ports before signing.
  Register row R-022 (venue provides reliable wireless for all attendees at once) is unverifiable as of 2026-11-02, so treat it as advice.
  (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Do you hire a wireless provider or run the access points yourself?**
  Two recorded views disagree (L-1116, L-1117), and one specialist returned for two conferences (L-2036, L-2077).
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Do you pay for a dedicated internet line and your own power backup?**
  Two conferences did (L-2076, L-3110).
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Which rooms and sessions are filmed, trainings included?**
  Seattle prioritized tutorials in two rooms (L-1124, L-1125), Bristol filmed four rooms (L-2046), attendees asked for everything (L-1126), and a 2024 survey summary recommends exploring trainings (L-4208).
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Where do you host video?**
  One team reports that PeerTube worked well (L-5027).
  (decide-by: T-3m)

## How-to

### Before you sign the venue
1. Ask the venue for a written network statement: capacity for all attendees at once, address pool size, upstream bandwidth, open ports and whether non-work use is permitted.
   Done: the statement is in the planning folder.
2. Ask what "install date" means to the provider: the day work starts or the time the network is live.
   Done: a written live-by time, earlier than the first session of the first training day.
3. Get a direct phone line to the upstream network administrators, and see the `wifi-failure` playbook for what to do with it.
   Done: the number is on the production contact sheet.
4. Name the recording owner and a deputy.
   Done: both names appear on the role map.

### Before setup day
5. Rehearse recording with the actual hardware through capture and playback, and document file destinations and the upload handoff (L-5049; S100).
   Done: one test file played back from the real destination, and a one-page handoff note.
6. Check projector brightness and screen size for the biggest room, plus a spare.
   Done: a projector list with spares.

### During the conference
7. Test the network with many real devices at once on setup day.
   Done: the pool and the uplink hold under load.
8. Confirm every evening that the day's recordings reached their owner and the uploader.
    Done: a tick on the daily readiness list.

### After the conference
9. Convert and publish the raw footage within the agreed days.
    Done: the playlist is public and linked from the program page.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009, S012, S036 | ledger: L-1115, L-1118, L-1119, L-2076, L-2077, L-4096 | confidence: observed | status: active | basis: independent-conferences

Size the network for every attendee connecting at once, and get the provider's capacity in writing.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009 | ledger: L-1121 | confidence: observed | status: active | basis: structural | reason: Developer tools such as remote shell and chat use ports beyond web and mail, whatever the year.

Check that no ports are blocked upstream.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S015, S049, S066 | ledger: L-2016, L-4070, L-4174 | confidence: reported | status: active | basis: independent-conferences

Prefer fast publication of recordings over longer, higher-quality post-production.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S098 | ledger: L-5025 | confidence: observed | status: active | basis: structural | reason: Capturing, converting and uploading video is hands-on work per session, whatever the community value.

Give recording its own workstream and accountable owner.
```

Four pieces of advice rest on one conference each:

- Pay an accountable provider rather than run the wireless network yourself (L-1116; S009), contradicted in the case notes.
- Record every talk even without post-production (L-1126; S088), set against prioritizing in the case notes.
- Provide a bright projector per room plus a spare, and screens of about 3 by 3 meters (L-1145, L-1146; S009, as of 2006).
- Do not learn video codecs and formats yourself, advice that ages fast (L-1127; S009).

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S098 | ledger: L-5027 | confidence: observed | status: active

The debrief described PeerTube as working well for live access by people outside the venue.
It is a tooling note, not a tested setup recipe.
```

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S074 | ledger: L-4208 | confidence: reported | status: active

The survey summary recommended exploring recording of training sessions.
```

```{note} [specific · 2023 · Eibar · 3 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2023 | place: Eibar | org: CodeSyntax | source: S069 | ledger: L-4182 | confidence: reported | status: active

During the conference days the video channel recorded more than 3,500 views and 400 hours of watch time.
```

```{note} [specific · 2022 · Namur · 4 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2022 | place: Namur | org: iMio and Affinitic | source: S066 | ledger: L-4174 | confidence: reported | status: active

All talks were streamed live and published quickly, drawing about 5,400 views a week.
```

```{note} [specific · 2021 · Online · 5 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2021 | place: Online | org: Plone Foundation | source: S064 | ledger: L-4169 | confidence: reported | status: active | context: format=online

Every training, talk, keynote and lightning talk was recorded and published online.
```

```{note} [specific · 2018 · Tokyo · 8 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2018 | place: Tokyo | org: Plone Conference 2018 Steering Committee | source: S095 | ledger: L-4154 | confidence: observed | status: active

The winning bid planned to film and live-stream all keynotes and sessions with the AV company that already served the national Python conference.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S093 | ledger: L-3110 | confidence: observed | status: active

A dedicated internet link and power generators were each among the larger cost lines, alongside filming of all talks.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2076, L-2077 | confidence: observed | status: active

The venue sat on a government network that blocked non-work use, so the team paid for a dedicated fiber line.
The returning Wi-Fi specialist covered the venue with 12 access points and no major problems.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2078 | confidence: observed | status: active

Streaming and recording all talks produced over 700 GB of raw footage to convert afterward.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S034 | ledger: L-3075 | confidence: observed | status: active

The person responsible for the Wi-Fi was hospitalized two weeks before the conference, and no backup plan existed.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S034 | ledger: L-3084 | confidence: observed | status: active

The organizer judged that recording and streaming could have been handled much better.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S015, S016, S017 | ledger: L-2016, L-2027, L-2046 | confidence: observed | status: active

All four rooms were filmed, camera and projector feeds recorded to disk and uploaded daily, so most talks were online by day's end.
AV rental and videography were nearly half of the final fixed costs, the largest cost group.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S017 | ledger: L-2036 | confidence: observed | status: active

The returning Wi-Fi specialist's equipment was stolen beforehand, and ten access points from a local stockist saved the setup.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S021 | ledger: L-2068 | confidence: reported | status: active

A community member who could not afford to travel found the talk videos a substantial substitute and said they set a high bar.
```

```{note} [specific · 2008 · Washington, D.C. · 18 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2008 | place: Washington, D.C. | org: ZPUGDC | source: S011, S012 | ledger: L-4094, L-4096 | confidence: observed | status: active

A contemporary report said: "We swamped the network this morning, and it's been down ever since."
The official record still links video and slides for most sessions.
```

```{note} [specific · 2007 · Naples · 19 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2007 | place: Naples | org: Abstract Open Solutions | source: S010 | ledger: L-4091 | confidence: observed | status: active

The bid sold the venue on 20-megabit internet connections in every hall.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009, S086 | ledger: L-1114, L-1115, L-1123 | confidence: observed | status: active

The sole venue vendor read "install at 9 a.m." as the time to start work, so the network was down until after lunch on day one.
The address pool of about 254 ran out for 350 users on day two.
Attendees rated internet access 2.72 of 5, the lowest logistics score.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1116 | confidence: observed | status: active

The organizers advised paying a provider who is accountable to you and can fix failures, instead of running the wireless network yourself.
This conflicts with the hearsay view recorded below, and the handbook does not resolve it.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1124 | confidence: observed | status: active

The first professionally recorded Plone conference covered two rooms for three days, at USD 15,000 (as of 2006), the most the budget allowed.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1125 | confidence: observed | status: active

Recording priorities were the key tutorials with lasting teaching value first, then sessions that market Plone to newcomers.
Not recording everything also kept a reason to attend in person.
This conflicts with the attendee request below, and the handbook does not resolve it.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S088 | ledger: L-1126 | confidence: observed | status: active

Several attendees asked for every talk to be recorded, even without post-production, because parallel tracks made them miss sessions.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S088 | ledger: L-1117 | confidence: hearsay | status: active

One attendee argued the opposite of paying a provider: never trust anyone else with conference Wi-Fi, and get a dedicated line and run your own routers.
```

## Risks

```{warning} Wi-Fi fails on the first morning
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Get capacity, pool size, open ports and a live-by time in writing and keep a direct line to the upstream administrators | owner-role: network lead | playbook: wifi-failure

Failures hit the first days in 2006 and 2008.
```

```{warning} The person who runs the network is unavailable
:class: hb-risk hb-likelihood-low hb-impact-high
risk | likelihood: low | impact: high | mitigation: Name a deputy with access to every credential and contact before setup day | owner-role: network lead | playbook: key-person-loss

One conference lost its Wi-Fi owner two weeks before the event.
```

```{warning} Recording has no owner and publication stalls
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Assign a recording owner and rehearse capture, file handoff and upload before setup day | owner-role: recording owner

Raw footage still needs conversion after the event.
```

## Thin content

```{warning} Network capacity standard
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A Foundation confirmation of whether the venue network requirement (register row R-022) has a capacity standard | who-might-know: Foundation Conference Committee; past AV leads

Only the call for proposals states the requirement, and it names no number.
```

```{warning} Live streaming setup recipe
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A tested streaming and recording setup recipe with hardware, software and handoff steps | who-might-know: Recording owners of past conferences; the video team | area: hybrid-online

One debrief reports that PeerTube worked well; no setup details are archived.
```

```{warning} Projector and bandwidth figures
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: Current projector brightness, screen size and bandwidth guidance from a recent AV company | who-might-know: AV companies serving recent conferences; recording owners | area: other

The figures in the lessons date from 2006 and are marked as such.
```

## Sources and further reading

- S009 Things We Learned About Running a Plone Conference, Seattle 2006.
- S010 Naples 2007 conference record.
- S011 Washington, D.C. 2008 conference record.
- S012 Contemporary report on the first-day Wi-Fi failure, 2008.
- S015 Plone Conference 2010, an organizer's view.
- S016 Plone Conference 2010, the numbers.
- S017 Plone Conference 2010 wrapup.
- S021 Plone Metrics assessment of the 2010 conference.
- S034 Interview with the 2011 organizer.
- S036 Plone Conference 2012 wrap-up, organizer account.
- S049 2016 call for proposals, codified requirements.
- S064 2021 conference video and platform recap.
- S066 Plone Conference 2022 recap.
- S069 Reflecting on Plone in 2023, conference statistics.
- S074 Results from the 2024 conference feedback survey.
- S086 Seattle 2006 overall conference evaluation.
- S088 Seattle 2006 logistics suggestions.
- S093 PythonBrasil organizer manual, Plone Conference 2013.
- S095 Tokyo 2018 winning proposal.
- S098 Plone Conference 2026 facts and lessons for the handbook.
- S100 Last-phase plan, 2026 conference organizing team.
