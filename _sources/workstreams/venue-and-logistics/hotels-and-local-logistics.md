---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [format=in-person, size]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to organize lodging, travel information and local logistics for a Plone Conference: hotel lists, group rates and maintenance."
    "keywords": "Plone, Plone Conference, hotels, lodging, travel, logistics"
---

# Hotels and local logistics

## Why it matters

Most attendees travel to the conference and pay for their own lodging.
They need to know where to sleep, how to get from the airport to the venue and where to eat, and they need to know it early enough to book at a fair price.

The organizers do not control the hotel market, but they can shape it.
They can choose a venue with lodging close by, negotiate group rates, publish a vetted list with distances and keep that list accurate.
A venue hotel with discounted rooms also keeps people on site in the evening, which turns hallways and bars into working space, as described in the case notes.

When this work is missed, attendees book far away or at high prices, find a published hotel sold out, or arrive without a plan for the last mile.
The sections below follow the order in which the decisions arise.
The venue itself is covered in [Venue](venue.md), and the choice of city in [City selection](city-selection.md).

## Applies when

- `format=in-person` Lodging and local travel matter only for people who attend in person.
- `size` The number of rooms to negotiate and the pressure on local hotel capacity grow with attendance.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-2105, L-3122, L-4177) **Will you publish a hotel list with distances to the venue and several price tiers, and name an owner who keeps it current?** Attendees rely on the list on the website, so an out-of-date entry sends them to a full hotel. (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Will you negotiate group rates, or leave attendees to the market?** One team called every hotel in the city, and the hotels were reluctant because they hoped to raise prices during large events (L-2075).
  Another conference used the discounted rooms of its venue hotel (L-2003).
  A third promoted its venue hotel together with a discount for an airline group (L-4230). (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will you reserve a dedicated lodging for attendees only?** One conference reserved a floating hotel that became a social hub (L-2082).
  It needs a lodging that can be reserved whole and a price that suits attendee budgets. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **How far may the venue be from an international airport?** Past hosting calls asked for at most one hour, with affordable transport so that attendees need no car (S049, S052, S055, S059, S096).
  The rule is unconfirmed as of 2026-11.
  One bid advised flying to a major hub and connecting (L-3122). (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Will you add local tourism and transport suggestions to the housing information?** The Foundation schedule groups housing for trainers and attendees, travel information and local tourism suggestions in one planning step (L-4030). (decide-by: T-6m)

## How-to

### Research

1. Map lodging within walking distance of the venue or a short transit ride, in at least three price tiers.
   Done when a table lists distance, travel time, an indicative rate with its date of check and the booking route for each hotel.
1. Ask the venue whether it has rooms and whether it offers a block or a discount.
   Done when the answer is in writing.
1. Check the city's event calendar for the conference dates.
   Large events raise prices and make hotels reluctant to discount.
   Done when any clash is noted and negotiation starts early.
1. Contact other hotels for group rates when the venue cannot house attendees.
   Done when each reply is recorded with its terms and expiry date.

### Publish

1. Publish a lodging page with the list, distances, tiers, booking links and any discount codes with expiry dates.
   Done when the page is linked from the venue and travel pages.
1. Publish travel directions: nearest airports, rail, local transit and the route from the airport to the venue, each with a date of check.
   Done when a first-time visitor can plan the whole trip from the page.
1. Publish housing and travel information together with local tourism suggestions.
   The Foundation schedule places this step in March (L-4030).
   Done when the page carries the date of the last check.
1. Mention visa support on the same page where it applies.
   Done when the page links to the visa information the team publishes.

### Maintain and run

1. Name an owner who checks availability every week in the last three months and marks sold-out hotels.
   Done when the owner records each check.
1. Put each discount-code deadline in the team calendar and remind attendees before it expires.
   Done when reminders are sent at least a week ahead.
1. Put the hotel list, a local map and transit information at the registration table.
   Done when attendees can find them without asking.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S036 | ledger: L-2105 | confidence: observed | status: active | basis: structural | reason: Attendees book from the published list, so a stale entry sends them to a full hotel.

Keep the hotel list on the conference website up to date for availability, because attendees rely on it.
```

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S082 | ledger: L-4230 | confidence: observed | status: active | context: venue=hotel

The venue was a hotel with integrated accommodation, promoted as the place to stay.
An airline-group discount applied for one week either side of the conference.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6031 | confidence: observed | status: active

Only 5 of 20 survey respondents stayed at the venue hotel, and all five would stay again; several named the hotel price as high, and one stayed elsewhere because of it.
```

```{note} [specific · 2022 · Namur · 4 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2022 | place: Namur | org: iMio and Affinitic | source: S067 | ledger: L-4177 | confidence: observed | status: active

Seven hotels lay within five minutes of the venue on foot or by bus.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S094 | ledger: L-3122 | confidence: observed | status: active

The bid advised flying to a major Brazilian hub and connecting domestically.
It listed hotels in four price tiers with distance to the venue and reference rates, and the venue was within walking distance of the two main hotel clusters.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2075 | confidence: observed | status: active

The team called every hotel in the city for special rates.
Hotels were reluctant because they hoped to raise prices during large concerts at the local stadium.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2082 | confidence: observed | status: active

A floating hotel on the river was reserved for conference attendees only, a first for the series, and became a social hub.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S015 | ledger: L-2003 | confidence: observed | status: active | context: venue=hotel

The venue hotel gave attendees discounted room rates.
Because of that, the conference could use the venue late into the evening for e-mail, work and group discussions in bars and corridors.
```

## Risks

```{warning} Hotels fill or raise prices before attendees book
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Start rate negotiations before the dates are announced, check the city's event calendar and publish alternatives in several price tiers | owner-role: logistics lead

A large local event on the same dates can remove rooms and raise prices.
Judged for a mid-size conference in a city with few hotels near the venue.
```

```{warning} The published hotel list or a discount code is out of date
:class: hb-risk hb-likelihood-medium hb-impact-low
risk | likelihood: medium | impact: low | mitigation: Name an owner for the list and set calendar reminders for each code's expiry date | owner-role: logistics lead

Attendees book from the list and trust it.
```

```{warning} Attendees cannot find a workable route from the airport to the venue
:class: hb-risk hb-likelihood-low hb-impact-medium
risk | likelihood: low | impact: medium | mitigation: Publish airport-to-venue routes with times and costs, and check them against real connections before publishing | owner-role: logistics lead

The risk grows when the nearest international airport is far from the venue.
```

## Thin content

```{warning} Room blocks and attrition terms
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: How a hotel room block was contracted, and what minimum pickup or attrition terms applied | who-might-know: Past organizers who contracted blocks; venue hotel sales teams | area: other

No account of the contract terms of a block is archived.
```

```{warning} Travel guidance beyond hotels
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Guidance on transfers, group travel, accommodation blocks for sprinters and sustainable travel options | who-might-know: Past organizers; sustainability volunteers | area: sustainability

The located evidence covers hotels and one hub-and-connect travel tip.
```

```{warning} Accessible lodging
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A checklist for accessible rooms and routes between lodging and venue, from an organizer who applied one | who-might-know: Accessibility volunteers; past organizers | area: accessibility

No account of accessible lodging at a Plone conference is archived.
```

```{warning} Airport distance rule
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: Confirmation from the Foundation of the airport and transport expectation in hosting requirements | who-might-know: Foundation board; conference committee | area: other

The requirements register lists R-023 as unverifiable as of 2026-11-02, because only hosting calls from 2016 to 2020 state it.
```

```{warning} Dedicated lodging for attendees
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second example of a reserved lodging and what it cost relative to market rates | who-might-know: Past organizers | area: other

Only one conference reserved a dedicated lodging.
```

## Sources and further reading

- S004 Plone Foundation, Conference Planning Schedule.
- S015 Bristol 2010, organizer's view, Netsight blog.
- S036 Arnhem 2012, organizer wrap-up, Four Digits blog.
- S049 Plone Foundation, 2016 call for proposals.
- S052 Plone Foundation, 2017 call for proposals.
- S055 Plone Foundation, 2018 call for proposals.
- S059 Plone Foundation, 2019 call for proposals.
- S067 Namur 2022, official record with venue, travel and accommodation.
- S082 Maastricht 2026, post-conference home page.
- S094 Brasília 2013, conference proposal.
- S096 Plone Foundation, 2020 call for proposals.
- S110 Maastricht 2026 attendee survey analysis.
