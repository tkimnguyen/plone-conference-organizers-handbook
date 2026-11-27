---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "The seven context dimensions that describe a Plone conference, what each value means, and how chapters and lessons declare which conferences they fit."
    "keywords": "Plone, Plone Conference, context dimensions, applies-to, tailoring, size bands"
---

# Context dimensions

No two Plone conferences are alike, and advice that fits one can mislead another.
Context dimensions are the handbook's shared vocabulary for saying which conferences a piece of advice fits.
Seven dimensions are enough to separate the cases that matter.
This page defines them, explains the values, and shows how chapters use them.
The process of classifying your own conference and recording your choices is on the page [Tailor](tailor.md).

## The seven dimensions

| Dimension | Values |
|---|---|
| `size` | `small`, `medium`, `large` |
| `jurisdiction` | An ISO 3166-1 alpha-2 country code such as `NL`, or `EU` |
| `organizer` | `company`, `volunteer-group`, `foundation-led`, `mixed` |
| `budget` | `seed-loan`, `financial-agent`, `own-risk` |
| `venue` | `hotel`, `university`, `conference-center`, `mixed` |
| `format` | `in-person`, `hybrid`, `online` |
| `language` | An ISO 639-1 language code such as `en` |

The values are a fixed vocabulary.
A chapter or lesson that uses a value outside this table fails the lint.
If a real conference does not fit any value, say so in your Tailoring Record and raise an issue; see [Extend](../running/extend.md).

## Size

The size band is set by paying and registered attendees at the main conference, not by the sprint or the trainings.

| Value | Attendees |
|---|---|
| `small` | Up to 150 |
| `medium` | 150 to 400 |
| `large` | More than 400 |

A conference at exactly 150 is small; one at exactly 400 is medium.
Size drives the number of rooms and parallel tracks, the volunteer count, the catering model, and whether a venue contract needs a minimum spend.
The archive shows the range: the Foundation's conference history lists editions from about 150 attendees (L-4009, L-4011) to more than 400 (L-4002), and a 2022 on-site edition of 151 (L-4017).
Use your expected paying attendance, then plan for the band above it when the forecast is uncertain.
Counts in the archive are not comparable without care, because registrants, streaming viewers and sprinters are different populations.

## Jurisdiction

Jurisdiction means the country whose law governs the contract with the venue, the tax position of the ticket sale and the data you hold on attendees.
It is not the attendees' home country and not necessarily the organizer's.
Use the country of the legal entity that signs the venue contract and sells the tickets.
`EU` marks advice that holds across European Union member states, for example the GDPR.
Chapters whose content varies by country carry the bare token `jurisdiction` and point to the jurisdiction annexes.
Annexes are general information, not legal, tax or insurance advice, and each needs a local adviser to confirm it.

## Organizer type

The organizer type says who carries the work and the accountability.

- `company`: one company, usually a Plone service provider, organizes with paid staff time.
- `volunteer-group`: community members organize in their own time, without a company behind them.
- `foundation-led`: the Plone Foundation itself organizes, as in editions run directly by the Foundation (L-4011, L-4015).
- `mixed`: a company and volunteers share the work, or a university and a company do.

The type changes how you staff roles, how you treat unpaid hours and who can sign contracts.
The 2006 Seattle account is explicit that its host treated the conference as paid project work with hundreds of staff hours (L-1033).
A volunteer group planning the same job needs a different calendar.

## Budget model

The budget model says who carries the financial risk before the money arrives.

- `seed-loan`: the Foundation lends up-front money, repaid after the conference.
  Seattle 2006 is the archived example, with a loan of USD 8,000 as of 2006 (L-1031).
- `financial-agent`: the Foundation acts as financial agent, so its accounts take in and pay out money for the event.
  The archive records trial uses from 2011 and a standing offer from 2018 (L-4057).
- `own-risk`: the organizer's own legal entity carries the risk and holds the money.

Whether any of the first two is still on offer must come from the requirements register, not from this page; see the page `requirements-register`.
The budget model decides which Foundation rules bind you as MUST items and who holds liability if the event loses money.

## Venue type

- `hotel`: a hotel offers rooms, meeting spaces and often catering under one contract.
- `university`: a campus provides rooms, often cheaper, usually with fixed access rules and limited catering choice.
- `conference-center`: a purpose-built center, typically with an in-house AV and catering provider.
- `mixed`: sessions, trainings, sprints or social events are held in different kinds of venue.

Venue type shapes the contract, the catering rules, the AV and Wi-Fi arrangements, and what you can negotiate.
The lessons ledger records both a university venue saving a large sum under nonprofit rental terms (L-3060, as of 2011) and the budget-versus-polish trade-off of a plain city-owned facility (L-1022, L-1023).

## Format

- `in-person`: all participants attend the venue.
- `hybrid`: an in-person event with a live remote audience that can take part.
- `online`: no shared venue.

Recording talks for later viewing does not make an event hybrid.
Hybrid and online events are the thinnest part of the evidence, and the thin registry marks them with the area `hybrid-online`.
The online editions of 2020 and 2021 are in the conference data table.

## Language

Language is the working language of the program and the main communication.
Use an ISO 639-1 code, such as `en`.
Almost all editions in the archive ran in English, so most chapters leave this dimension unstated.
It matters for a conference that runs a track or a whole event in another language, because speaker care, signage, the code of conduct text and marketing then need translation.

## How chapters declare what they fit

Each chapter says which conferences it fits in two places that must agree.

1. The front matter field `applies-to` holds a list of tokens.
2. The section *Applies when* holds one bullet per token, each starting with the token in backticks and followed by one sentence saying why.

A token takes one of three forms.

| Token | Meaning |
|---|---|
| `all` | The chapter applies to every conference. It is the only token on the page. |
| `jurisdiction` | The chapter applies to every value of the dimension, and its content varies by that dimension. |
| `size=medium,large` | The chapter applies only to the listed values. |

Examples that all use the same grammar:

```yaml
applies-to: [all]
applies-to: ["size=medium,large", "format=in-person"]
applies-to: [jurisdiction, budget=financial-agent]
```

Quote a token that contains a comma, because a YAML list otherwise splits it.
Several dimensions on one chapter all have to hold at once.
A chapter on a Foundation-managed budget, for example, uses `budget=financial-agent`, and a team with another budget model skips it and records why.

## How lessons declare context

A lesson may carry an optional `context` field with the same tokens, separated by semicolons: `context: size=small; jurisdiction=NL,BE`.
An absent `context` means the lesson is not limited to any context.
Two lessons distinguish each other when some dimension appears in both with disjoint values.
That is how two active lessons can disagree without breaking the contradiction rule.
A lesson about a small conference can recommend one volunteer-heavy model while a lesson about a large conference recommends another.
The writing rules are on the page `lesson-authoring-rules`.

## Choosing your values

1. Write one value per dimension at the top of your Tailoring Record.
2. If a dimension is uncertain at the start, write the likely value and mark it open.
3. Read the *Applies when* section of every chapter before you adopt it, and note any chapter that does not fit.
4. Revisit the values when a decision changes one, for example when the venue type changes after the first contract.
5. Send the record back at handover, so that lessons from your context reach the next team with the right label.
