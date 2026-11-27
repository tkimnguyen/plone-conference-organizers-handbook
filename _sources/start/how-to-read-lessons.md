---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: explanation
myst:
  html_meta:
    "description lang=en": "How to read the badges, age labels, confidence levels and thin markers in this handbook, and how far to trust each lesson."
    "keywords": "Plone, Plone Conference, lessons, badges, confidence, stale-prone, MUST, DEFAULT, OPTION"
---

# How to read lessons

Every claim in the handbook carries a small label that tells you how far to trust it.
This page explains each label, so you can decide in a few seconds whether to rely on a lesson, check it first, or treat it as one story among many.

## General and specific lessons

A **general lesson** is a timeless claim that passed the promotion rule.
It appears in the section *Principles and general lessons* of a chapter.
It is never dated and never names a place or an organizer.
Its title reads `[general]`.

A **specific lesson** describes what one conference did at one time and place.
It appears only in the section *Case notes*, newest first.
Its title carries its provenance, for example:

```text
[specific · 2012 · Examplecity · 14 y] stale-prone
```

The parts are the year, the place, and the age in whole years.
The organizing body and the source ID appear on the first line inside the block.

A specific lesson becomes general only after it has been seen at three independent conferences run by at least two organizing bodies, or when it rests on a structural reason that does not depend on the year, such as a legal rule.
Until then it stays a case note, however convincing it sounds.
The full rule is described in [Update](../running/update.md), and the page `lesson-authoring-rules` holds the writing rules.

## The age badge

Age is computed, never typed by hand.
It is the pinned as-of year of the handbook minus the year of the lesson.
The as-of year is 2026 for the first release and moves at each annual release, so a lesson's age grows on its own.

| Age in years | Bucket | How it looks |
|---|---|---|
| 0 to 3 | recent | Normal emphasis. |
| 4 to 8 | mid | Reduced emphasis. |
| More than 8 | old | The word `stale-prone` in the title, and the body collapsed or clamped. |

A `stale-prone` lesson is not wrong.
It is old enough that the context has probably moved: prices, platforms, tax rules, venues and community habits change.
Treat it as a question to check, not as an answer.
Ask whether the situation it describes still exists, and look at the source before you rely on it.

## Confidence

Each lesson states how its evidence arrived.

- **observed**: the source author took part and describes their own experience, or the source is a primary document such as a policy or a published call.
- **reported**: the source passes on what it learned from others.
- **hearsay**: an anecdote that cannot be checked.
  It may be recorded, but it never supports a MUST or a DEFAULT badge.

When a lesson draws on several rows, it shows the weakest confidence among them.

## Status

A lesson is `active` unless its title says otherwise.

- `contested`: another lesson or a reader disagrees, and the block links a discussion issue.
  Read the issue before relying on the lesson.
- `superseded`: a later lesson replaces it, and the block names the replacement.
  The old text is dimmed or struck through.

Two active lessons never contradict each other unless a stated context distinguishes them, for example size or jurisdiction.

## Level badges: MUST, DEFAULT, OPTION

Decisions in the "Decisions you must make" section carry exactly one badge.
The word is part of the badge, so color is never the only signal.

- {bdg-danger}`MUST` (req: R-012; as-of: 2026-11-02) A Foundation requirement or a legal necessity, citing a register row and its as-of date like this one.
  Deviating needs a written Foundation exception, linked in your Tailoring Record.
  The handbook cannot waive a legal necessity.
- {bdg-primary}`DEFAULT` (basis: L-1082, L-5001) A strong recommendation backed by at least two ledger rows from at least two distinct conferences, like these two.
  You may deviate, with a reason recorded in your Tailoring Record.
- {bdg-secondary}`OPTION` Context-dependent.
  The team chooses, and nothing needs recording except the choice.

A recommendation with weaker evidence than a DEFAULT needs is shown as an OPTION, and the chapter says why.
Badges also appear on single steps in a how-to when a step has its own level.

## Thin markers

A thin marker is a public admission that a chapter is weak at that spot.
It names what would close the gap and which roles might know.

- `gap`: no evidence was located.
- `single-source`: one source or one conference supports the content.
- `stale`: evidence exists but is old or known to be outdated.

A page with thin markers is still useful.
Calibrate your trust to the marker, and consider helping to close it; see [About the thin registry](../running/thin-registry-about.md).

## Maturity

Every page states how far it has come in its front matter.

| Maturity | Meaning |
|---|---|
| `stub` | A skeleton with at least one thin marker. |
| `draft` | All sections have real content and at least one source. |
| `reviewed` | A reviewer other than the author checked it, it has at least two distinct sources, and it has a named steward. |
| `proven` | An organizing team used it in a real conference, and it has at least three distinct sources. |

A page never claims more than its evidence supports.
Each page also has a `review-by` date.
After that date, the page is flagged for a fresh review until someone confirms or updates it.

## A short routine for reading a chapter

1. Read *Applies when*.
   If your size, country or format is not listed, adapt before you adopt.
2. Read the badged decisions and note the MUST items first.
3. Read the principles, which are the most trusted advice on the page.
4. Skim the case notes from the top.
   Check any `stale-prone` note before relying on it.
5. Read the thin markers to see where the chapter is weak.
6. Follow a source ID from the last section when a claim matters to you.

## Where to see all labels at once

- The lesson index lists every lesson in rank order within its chapter.
- The decision register lists every badged decision, and is the checklist for your Tailoring Record.
- The thin registry and the coverage map show where evidence is missing.
