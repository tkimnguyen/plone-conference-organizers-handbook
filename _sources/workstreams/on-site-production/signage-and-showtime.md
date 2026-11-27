---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to run registration, signs, floor plans and the first day of a Plone conference so attendees arrive, find rooms and start talking."
    "keywords": "Plone, Plone Conference, registration, signage, wayfinding, first day"
---

# Signage and showtime

## Why it matters

The first morning is the one moment when every attendee meets the organization at the same time.
If registration queues up, if nobody can find the room or if the badges are in the wrong order, the first impression is set before the first talk starts.

Showtime is also the stretch when the team has the least slack.
Volunteers are tired, suppliers are late, and the venue is shared with other guests, so signs, bags and equipment can vanish overnight.
Small routines such as a daily team check keep problems from piling up.

Badges and bags are produced in [Print and merch](print-and-merch.md).
The network and projectors that the sessions rely on are in [AV, recording and internet](av-recording-internet.md).

## Applies when

- `all` Every conference has a first morning and rooms to find.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-1150, L-2039) **Do you register people before the opening morning and keep badge handout apart from bags and shirts?**
  One team checked in training attendees the evening before, and another separated badges from bags and funneled people through a corridor toward coffee.
  (decide-by: T-3m)
- {bdg-primary}`DEFAULT` (basis: L-1152, L-3056) **Does every room have a printed schedule and signs from day one?**
  One conference posted one sign per room per day, another put a schedule in front of every room door.
  (decide-by: T-2m)
- {bdg-secondary}`OPTION` **When do shirts and bags go out?**
  One team started shirts on day two to keep check-in fast (L-1151).
  Another sorted bags by last name across several lines (L-2087).
  (decide-by: T-3m)
- {bdg-secondary}`OPTION` **How do you protect signs and bags in a shared venue?**
  Signs and bags disappeared overnight at a shared venue (L-2087, L-2088).
  (decide-by: T-2m)
- {bdg-secondary}`OPTION` **How many registration volunteers, and what master list?**
  One team used about six trusted volunteers and one master paper list with digital copies (L-1149).
  (decide-by: T-3m)
- {bdg-secondary}`OPTION` **Do you hold an opening icebreaker?**
  One team reserved the first 45 minutes of day one for it (L-1113).
  (decide-by: T-3m)
- {bdg-secondary}`OPTION` **Do you hold a daily operations meeting?**
  One team ran a short daily meeting and an end-of-day readiness check (L-5048; S100).
  (decide-by: T-1m)

## How-to

### Before the conference
1. Staff the registration desk with about six trusted volunteers and one master paper list with digital copies (L-1149; S009).
   Done: a desk roster and a printed list.
2. Check in training attendees at the end of the last training day, the evening before the conference (L-1150; S009).
   Done: a check-in slot is on the training schedule.
3. Make the floor plan available to everyone (L-2101).
   Done: a plan on the website and at the desk.
4. Print signs: one per room per day listing that day's sessions, all put up on day one and one removed each night (L-1152; S009).
   Done: a sign set per room.
5. Mark the conference's own equipment with small translucent Plone stickers (L-3044; S027).
   Done: every loan item carries a sticker.

### On the first day
6. Open a separate line for questions next to the bag handout (L-2107).
   Done: a volunteer stands at that line.
7. Put a schedule in front of every room door and make quick direction signs on the spot (L-3056; S029).
   Done: signs are up before the first session.
8. Keep a printer connected to a computer full time, for receipts and boarding passes (L-3057, L-2108; S029).
   Done: the printer is at the information desk.

### Every day
9. Run a short operations meeting and an end-of-day readiness check (L-5048; S100).
   Done: the next day's roster is confirmed and recordings and catering updates have reached their owners.
10. Check the signs each morning and replace missing ones before the first session.
    Done: every room has its sign.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009, S017, S034 | ledger: L-1150, L-1151, L-2039, L-3077 | confidence: observed | status: active | basis: independent-conferences

Spread the first-day registration load before the opening, and keep badges in order.
```

Four pieces of advice rest on one conference each:

- Make the floor plan available to everyone (L-2101; S036).
- Run a separate line for questions when you hand out goodie bags at first entry (L-2107; S036).
- Keep a printer connected to a computer full time during the event (L-2108; S036).
- Reserve the first 45 minutes of day one for an icebreaker: welcome, thanks, then conversation (L-1113; S009).

## Case notes

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2087 | confidence: observed | status: active

Bags were sorted by last name across several lines, and about ten bags vanished overnight during a concert at the shared venue.
The information desk reprinted badges for those attendees.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2088 | confidence: observed | status: active

The floor plan confused attendees, so the team printed more than 100 direction signs.
One morning every sign had been removed overnight and had to be replaced before the program started.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S034 | ledger: L-3077 | confidence: observed | status: active

Badges fell out of alphabetical order on the first day and caused long queues at registration.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S017 | ledger: L-2039 | confidence: observed | status: active

Badges were handed out apart from bags and shirts, an idea taken from a European conference, and people were funneled through a corridor toward coffee.
Almost everyone was registered before the opening keynote.
```

## Risks

```{warning} Signs and bags disappear overnight in a shared venue
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Agree with the venue which areas stay locked overnight, keep a reprint kit and check every sign before the first session | owner-role: venue lead

A shared venue hosting other events can strip or lose conference material between days.
```

```{warning} Registration queues block the opening morning
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Check in trainees the evening before, sort badges alphabetically and run separate lines for badges, bags and questions | owner-role: registration lead

Judged for a typical mid-size conference.
```

## Thin content

```{warning} Accessible wayfinding
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Guidance on step-free routes, large-print signs and signs in several languages | who-might-know: Accessibility lead of past conferences; venue accessibility officers | area: accessibility

No archived account covers wayfinding for attendees with access needs.
```

```{warning} Stage hosting and timekeeping
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Practice from past conferences on hosts, timekeepers and announcements between sessions | who-might-know: Session chairs and program leads of past conferences

Only the opening icebreaker and the daily team check are documented.
```

## Sources and further reading

- S009 Things We Learned About Running a Plone Conference, Seattle 2006.
- S017 Plone Conference 2010 wrapup.
- S027 Wiki: Physical Resources.
- S029 Wiki: Printing.
- S034 Interview with the 2011 organizer.
- S036 Plone Conference 2012 wrap-up, organizer account.
- S100 Last-phase plan, 2026 conference organizing team.
