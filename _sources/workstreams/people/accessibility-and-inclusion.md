---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to make a Plone conference usable for more people: venue access, legible slides, language support and financial help for travel."
    "keywords": "Plone, Plone Conference, accessibility, inclusion, language, scholarships"
---

# Accessibility and inclusion

## Why it matters

A conference is only open to the people who can get in, read the slides, follow the language and afford the trip.
Each barrier removes contributors the community wants, and it removes them quietly: nobody complains, they simply do not come or leave early.

Most of these barriers are cheap to remove when someone owns them early and expensive or impossible to fix on the day.
The handbook's evidence is uneven.
Venue access, projected text, interpretation and financial help each have a few accounts.
Many other areas have none, and the Thin content section lists them.

This chapter works together with [Volunteers and roles](volunteers-and-roles.md) for the people who staff access tasks, and with [Visas and travel](visas-and-travel.md) for the barriers that border control creates.

## Applies when

- `all` Every Plone conference has access, language and affordability questions, in any size, venue or format.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-4176, L-5035) **Who confirms the venue's accessibility in writing, and who publishes it on the website?** Name one owner before the venue is signed, because this task has been dropped between planning and delivery. (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-1053, L-4101, L-5004) **Will you offer financial help to contributors who cannot afford the trip?** Choose a mechanism, such as grants or a reduced price tier, and treat the pricing and the funding application as separate tasks. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will you offer interpretation or language assistants?** One conference planned an assistant in every English-language training and interpretation in sessions, because most local developers were not fluent in English (L-3105, L-3120). (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will you set a minimum on-screen text size for speakers?** One conference lost an attendee from a session over unreadable slides (L-1054). The rule costs a line in the speaker guidelines. (decide-by: T-3m)

## How-to

1. Name an owner for accessibility, and write the task into the team's plan with a due date. Done when the owner has a name and a deadline before venue signing.
1. Ask the venue in writing about step-free routes, lifts, accessible restrooms and seating, and file the answer with the contract. Done when each room used by the conference is covered.
1. Publish an accessibility page on the conference website with the venue's answers and a contact for questions. Done when the page is linked from the venue page.
1. State a minimum letter size for slides in the speaker guidelines, and ask the venue for screen sizes and sight lines. Done when the guidelines carry the figure.
1. Decide which languages the sessions use and whether participants need help. Check with the local community before the program is final.
1. Choose the financial help mechanism, announce it with the registration opening, and name who decides on applications.
1. Check printed badges for text that is hard to read, such as light gray on white, and choose type and contrast so the name is readable at arm's length.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009, S013, S098 | ledger: L-1053, L-4101, L-5004 | confidence: reported | status: active | basis: independent-conferences

Offer financial help, as grants, scholarships or reduced prices, to contributors who cannot afford to travel.
Without it, some key contributors cannot attend, and it also recognizes their work.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S088 | ledger: L-1054 | confidence: observed | status: active | basis: structural | reason: Legibility depends on letter size, screen size and viewing distance, which do not change with the year.

Set a minimum on-screen letter size for speakers and choose rooms with screens large enough for the back rows.
Text that cannot be read excludes the person who cannot read it.
```

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S098 | ledger: L-5004 | confidence: observed | status: active

The team introduced Global South pricing and pursued dedicated grant support for it.
The pricing initiative and the funding application were separate tasks.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5035 | confidence: reported | status: active

The venue-accessibility coordination task was dropped, and the planned website information on accessibility was not produced.
The review names a delivery gap and does not establish the venue's actual accessibility.
```

```{note} [specific · 2022 · Namur · 4 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2022 | place: Namur | org: iMio and Affinitic | source: S067 | ledger: L-4176 | confidence: observed | status: active

The congress-center venue was fully accessible for people with reduced mobility.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S093 | ledger: L-3105 | confidence: observed | status: active

The conference had simultaneous interpretation, supported by the international affairs office of the Federal District.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S094 | ledger: L-3120 | confidence: observed | status: active

Most local developers were not fluent in English.
The bid planned a Portuguese-speaking assistant in every English-language training, one Portuguese-only track and one English track with translation into Portuguese.
```

```{note} [specific · 2009 · Budapest · 17 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2009 | place: Budapest | org: Greenfinity | source: S013 | ledger: L-4101 | confidence: reported | status: active

A foundation grant program covered registration and part of the travel for participants, especially from Eastern Europe.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S089 | ledger: L-1055 | confidence: hearsay | status: active

One attendee welcomed chat nicknames on badges but found the light gray text unreadable.
```

## Risks

```{warning} Venue accessibility is never confirmed or published
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Assign one owner before the venue is signed and require the written venue answers on the website before ticket sales open | owner-role: accessibility owner

One conference dropped this task and never produced the planned website information (L-5035).
Judged for a mid-size conference.
```

```{warning} Slides are unreadable from the back of the room
:class: hb-risk hb-likelihood-medium hb-impact-low
risk | likelihood: medium | impact: low | mitigation: Put a minimum letter size in the speaker guidelines and test the screens in the largest room before the first session | owner-role: program lead

Attendees leave the session when they cannot read it.
```

```{warning} Financial help is announced after the people who need it have decided
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Announce grants or reduced prices with the opening of registration and keep the funding application on its own timeline | owner-role: treasurer

The pricing initiative and the funding application ran as separate tasks at one conference, so they can finish at different times.
```

## Thin content

```{warning} Accessibility beyond venue access and projected text
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Practice from past conferences on captioning, quiet space, sensory needs, accessible website and accessible video | who-might-know: Accessibility working groups in the community; organizers of other accessible open source events | area: accessibility

No located source covers hearing, vision, cognitive or sensory needs beyond the two points above.
```

```{warning} Venue accessibility at the 2026 conference
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A verified account of the venue's accessibility and what participants actually experienced | who-might-know: The organizing team of the 2026 conference; participants who used the venue | area: accessibility

The review records a delivery gap, but the venue's actual accessibility is not established.
```

```{warning} Language support rests on one conference
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second account of interpretation or assistants, with costs and the quality that attendees reported | who-might-know: Organizers of conferences held in non-English-speaking countries; interpreters hired by earlier teams | area: other

The accounts come from the Brasília conference, from a bid and a manual rather than from a review.
```

```{warning} Financial help rests on thin and dated evidence
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: Up-to-date practice on eligibility, selection and funding of grants and reduced-price tiers | who-might-know: Foundation grant and travel-support roles; treasurers of earlier conferences | area: other

The grant accounts are from 2006 and 2009, and the 2026 account describes a pricing initiative without its outcome.
```

## Sources and further reading

- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
- S013 Budapest 2009, contemporary conference announcement and context.
- S067 Namur 2022, official record of the conference.
- S088 Seattle 2006, logistics suggestions from the attendee evaluation.
- S089 Seattle 2006, general comments from the attendee evaluation.
- S093 Brasília 2013, PythonBrasil organizer manual, operational record.
- S094 Brasília 2013, conference proposal.
- S098 Maastricht 2026, facts and lessons for the handbook.
- S099 Maastricht 2026, review of the GitHub issues and project board.
