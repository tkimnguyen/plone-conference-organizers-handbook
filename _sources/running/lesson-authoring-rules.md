---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "Writer-facing rules for lessons, thin markers and risks: scopes, fields, confidence, promotion, contradictions, age ranking and one worked example."
    "keywords": "Plone, Plone Conference, lesson authoring, ledger, conventions, writing rules"
---

# Lesson authoring rules

This page is for the person who writes a lesson, a thin marker or a risk into a chapter.
It condenses the conventions in `docs/spec/conventions.md`, sections 3 to 7, into the rules a writer needs.
The spec holds the exact grammar and is what the lint scripts implement.
If this page and the spec disagree, the spec wins, and this page needs a correction.
The route from an issue form to a merged pull request is on the page [Update](update.md).

## The two scopes

A **general** lesson is a timeless claim.
It lives only in the section *Principles and general lessons*.
It carries no year, no place and no organizer.

A **specific** lesson is what one conference did at one time and place.
It lives only in the section *Case notes*.
It carries a year, a place and the organizing body.

A specific lesson anywhere else fails the build, and so does a general lesson in Case notes.
When you are unsure, write a specific lesson.
Promotion to general is a separate step with its own test.

## Write the ledger row first

Every lesson cites at least one ledger row.
A row is one extraction from one source, with a disposition such as `placed: <chapter id>#case-notes`.
The lesson's fields must agree with its rows.

- For a specific lesson, the year, place and organizing body equal those of every cited row.
- The `source` field is the union of the rows' source IDs.
- The `confidence` is the weakest confidence among the rows.
- Every cited row names this chapter in its disposition, and every row placed in a section of the chapter is cited in that section.

The ledger format is in `docs/spec/ledger-schema.md`.
Write the row, then the block, then run the generator.

## The block and its fields

A lesson is a stock `note` admonition with a fixed class line and one field line, followed by a short body.
The field line is one physical line.
Segments are separated by a space, a pipe and a space, and each segment reads `key: value`.

| Field | Used for | Rule |
|---|---|---|
| `scope` | all | `general` or `specific` |
| `year`, `place`, `org` | specific only | Four digits, a place name, an organization. Never a person. |
| `source` | all | Source IDs, comma separated |
| `ledger` | all | Ledger IDs, comma separated |
| `confidence` | all | `observed`, `reported` or `hearsay` |
| `status` | all | `active`, `contested` or `superseded` |
| `basis` | general only | `independent-conferences` or `structural` |
| `reason` | general with `basis: structural` | One sentence naming the structural reason |
| `context` | optional | Context tokens; see [Context dimensions](../start/context-dimensions.md) |
| `issue` | when `contested` | An issue number or link |
| `by` | when `superseded` | The ledger ID of the replacing lesson |
| `conflicts-with` | optional | Ledger IDs of lessons this one contradicts |

The title and the class line are computed from these fields.
Do not type them.
Write any placeholder, run the generator, and commit its result.

## Confidence

Confidence says how the evidence reached the source, and it is judged per ledger row.

- `observed`: the source author took part, or the source is a primary document such as a policy.
- `reported`: the source passes on what it learned from others.
- `hearsay`: an anecdote that cannot be checked. It never supports a MUST or a DEFAULT badge.

A lesson built from several rows carries the weakest of their confidence values.
Do not round up.

## Writing the body

1. One lesson, one statement.
   If the text needs "and" to join two points, split it into two blocks.
2. Put the transferable point first, then at most a short reason.
3. Keep it under 80 words.
   Longer material belongs in the chapter's how-to or in the source.
4. A specific lesson says what happened and where it applies.
   It never starts with "always" or "never".
5. Generalize.
   Keep out names of private persons, contact details, private amounts and buyer data.
   A public price appears only with an as-of date and a source, for example "as of 2026-09".
6. Use a `context` field when the lesson depends on size, jurisdiction, format or another dimension.

## Order and age ranking

Ranking is computed, never hand-written.

- General lessons outrank specific ones.
- Among specific lessons, age is the pinned as-of year of the handbook minus the lesson's year.
  Age 0 to 3 is `recent`, 4 to 8 is `mid`, and more than 8 is `old` and shows the word `stale-prone`.
- In Case notes, order lessons by year, newest first, then by confidence (`observed`, `reported`, `hearsay`), then by the first ledger ID.
- In Principles and general lessons, order lessons by the first ledger ID.

The as-of year is pinned in `handbook-config.yml` and moves at each annual release, so a lesson ages without anyone editing it.

## Promotion: specific becomes general

A specific lesson may be restated as a general lesson only when one of these holds.

1. **Independent evidence.**
   The cited rows come from at least three distinct conferences (distinct year and place) and at least two distinct organizing bodies.
   The lesson carries `basis: independent-conferences`.
2. **A structural reason.**
   The point rests on something that does not depend on the year, such as a legal rule or a physical limit.
   The lesson carries `basis: structural` and a `reason` field.

The general lesson replaces the specific ones on the page, and the specific ones stay in the ledger.
Promotion is recorded as one changelog line.
Do not promote early.
If the evidence is short, leave the case notes in place and add a thin marker.

## Contradictions

Two active lessons may not conflict unless a context tells them apart.
If you notice a conflict, list the other lesson in `conflicts-with` and then do one of three things.

- Add distinguishing `context` fields to both lessons.
- Mark one lesson `contested` and link a discussion issue.
- Mark one lesson `superseded` and name its replacement in `by`.

The lint only sees conflicts that someone declared.
Reviewers therefore ask the question again when they read the pull request.

## Thin markers and risks

A thin marker is a `warning` block in the section *Thin content*.
It needs `kind` (`gap`, `single-source` or `stale`), `needs` (what would close the gap, in one sentence) and `who-might-know` (roles and groups, never private persons).
A stub chapter needs at least one marker.
Details are on the page [About the thin registry](thin-registry-about.md).

A risk is a `warning` block in the section *Risks*.
It needs `likelihood` and `impact` (`low`, `medium` or `high`) and a `mitigation` of one sentence that names an action.
Phrase the risk as an event that can happen, not as a worry.
Risk titles are unique within a page.

## Worked example

The ledger row below uses placeholder values.
Its disposition places it in the Case notes of a chapter.

```yaml
- ledger_id: L-0000
  topic: example-chapter
  scope: specific
  year: 2024
  place: Examplecity
  org: Example Group
  source_id: S000
  text_kind: paraphrase
  quote_or_paraphrase: The registration desk opened one hour before the first session and never had a queue.
  confidence: observed
  status: active
  disposition: "placed: example-chapter#case-notes"
```

The lesson block in the chapter, before the generator has run, can carry any title and any class line.

````markdown
```{note} placeholder
:class: hb-lesson
lesson | scope: specific | year: 2024 | place: Examplecity | org: Example Group | source: S000 | ledger: L-0000 | confidence: observed | status: active

Open the registration desk one hour before the first session, so that arrivals never queue.
```
````

After `venv/bin/python -m scripts.generate fix docs/<path-to-page>.md`, the title and the class line are computed.
The same block, with the age in 2026, reads as follows.

````markdown
```{note} [specific · 2024 · Examplecity · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Examplecity | org: Example Group | source: S000 | ledger: L-0000 | confidence: observed | status: active

Open the registration desk one hour before the first session, so that arrivals never queue.
```
````

The body is one statement with a reason, under 80 words, with no name and no private amount.

## Checklist before you open the pull request

1. The lesson is in the right section for its scope.
2. The ledger row exists and its disposition names this chapter.
3. Year, place, organizer, source and confidence agree with the rows.
4. The body is one statement, under 80 words, with no private data.
5. The generator has computed the title and classes, and its output is committed.
6. You checked for a contradiction and declared it if you found one.
7. For a general lesson, the promotion test holds and the changelog line is written.
