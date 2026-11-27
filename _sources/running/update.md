---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: how-to
myst:
  html_meta:
    "description lang=en": "How to add a lesson or correct a fact in the handbook: issue form, ledger row, admonition block, steward review and the CI checks that follow."
    "keywords": "Plone, Plone Conference, update, lesson, pull request, ledger, review"
---

# Update

You ran or helped run a conference and learned something.
This page shows how that lesson reaches the handbook, from the issue form to a merged pull request.
The same route handles a correction.
The route stays plain on purpose: issue forms, ledger rows and Markdown files, matching how the community already works.
Documentation tooling that outruns a team's daily habits is how handover records never get written (L-5040).

## Pick the route

| Your change | Route |
|---|---|
| A typo or a broken link | Edit the file in the GitHub web interface and open a pull request. See `CONTRIBUTING.md`. |
| A wrong fact, a wrong date or an outdated figure | Open the correction issue form, or fix it directly if you have the source. |
| A lesson from a conference | The lesson route, below. |
| A gap you can close | Claim the help-wanted issue; see [About the thin registry](thin-registry-about.md). |

## The lesson route

The route has five stages.

1. Open the lesson issue form.
2. A steward accepts it and prepares the evidence.
3. You write the ledger row and the lesson block.
4. You open a pull request.
5. A steward reviews, and the CI gates run.

### 1. Open the lesson issue form

In the repository, open the issues tab, start an issue and pick the form *Lesson submission*.
The form asks for:

- The chapter id where the lesson belongs.
- The scope: specific, which means one conference, or general, which means holds across conferences.
- The year, place and organizing body for a specific lesson.
- A source: a published document, or a conference record you can file.
- The lesson in one sentence, and a short reason.
- Your confidence: observed, reported or hearsay.
- Whether it conflicts with something already in the handbook.

Do not enter personal data, private amounts, contact details or buyer data.
The handbook takes only generalized information.

### 2. A steward accepts it and prepares the evidence

A steward or maintainer reads the issue and replies.
They confirm the chapter, assign a ledger ID and tell you the ledger file to use, and make sure the source has a source ID in the manifest.
If the source is a conference record that is not yet in the archive, the maintainer helps add it.

### 3. Write the ledger row and the lesson block

Every lesson cites at least one ledger row.
A ledger row is one extraction from one source, with a disposition.
For a lesson that goes into a chapter, the disposition is `placed: <chapter id>#case-notes`.
The format is in `docs/spec/ledger-schema.md`.

Then write the lesson as an admonition block inside the chapter's section *Case notes*.
The block has a title, a class line, a field line and a short body.
The example below uses placeholder values.

````markdown
```{note} [specific · 2024 · Examplecity · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Examplecity | org: Example Group | source: S000 | ledger: L-0000 | confidence: observed | status: active

State the transferable point first, then at most a short reason.
```
````

Rules for the block:

1. **One lesson per block**, under 80 words.
   If the text needs "and" to join two points, split it.
2. **The field line is one physical line.**
   Segments are separated by a space, a pipe and a space.
   Each segment is `key: value`.
3. **The title and the classes are computed.**
   Do not type them by hand.
   Write any placeholder, then let the generator compute the title and the class line: run `venv/bin/python -m scripts.generate fix docs/<path-to-page>.md`.
4. **A specific lesson lives only in Case notes.**
   A specific lesson anywhere else fails the build.
5. **Order matters.**
   Case notes run newest year first, then by confidence (observed, reported, hearsay), then by the first ledger ID.
   General lessons run by the first ledger ID.
6. **No dates in general lessons**, and no place or organizer.
7. **A specific lesson never begins with the words always or never.**
   It states what happened and where it applies.
8. **Add a `context` field** when the lesson depends on size, jurisdiction or format, for example `context: size=small; jurisdiction=NL`.

The full field list and the exact grammar are in `docs/spec/conventions.md`.
The page `lesson-authoring-rules` collects the writing guidance.

### 4. Open the pull request

Use the pull request template.
It asks you to confirm each of these.

- The lesson cites a ledger ID, and the ledger row's disposition points to the same chapter.
- Every source ID exists in the manifest and is listed in the chapter's section *Sources and further reading*.
- The generator has been run and its output is committed.
- The privacy rules are met.
- You asked yourself whether the lesson contradicts an existing one.

### 5. Review and CI gates

A steward reviews the pull request.
A lesson's author is never its only reviewer.
For a lesson from year Y, at least one reviewer comes from an organizing body other than the one that ran Y.

The continuous integration run checks the following.

| Gate | Checks |
|---|---|
| Build | The site builds with zero warnings and no orphan pages. |
| Chapter contract | The nine sections in order, valid front matter, maturity minimums, the length budget. |
| Directive validation | Field lines parse, titles and classes match, placement and ordering are right. |
| Ledger coverage | Every row has a disposition, and ledger and chapter agree in both directions. |
| Privacy lint | No emails, phone numbers, bank numbers or deny-listed names. |
| Drift check | The generated pages match what the generator produces. |

Fix what fails and push to the same branch.
A steward merges when the gates are green and the review is done.

## How a lesson becomes general

A specific lesson is restated as a general lesson only when one of two things holds.

1. **Independent evidence.**
   The ledger rows it cites come from at least three distinct conferences (distinct year and place) and at least two organizing bodies.
   The lesson carries `basis: independent-conferences`.
2. **A structural reason.**
   The point rests on a reason that does not depend on the year, such as a legal rule or a physical constraint.
   The lesson carries `basis: structural` and a `reason` field of one sentence.

The general lesson replaces the specific ones on the page.
The specific ones stay in the ledger.
The maintainers record each promotion in the changelog as one line.
Early promotion is not allowed: if the evidence is not there yet, the lesson stays a case note, and the chapter's thin content section says so.

## When two lessons disagree

Two active lessons may not conflict unless a stated context tells them apart.
If you notice a conflict, name the other lesson in the field `conflicts-with`.
Then do one of these.

- Add distinguishing `context` fields to both lessons.
- Mark one lesson `contested` and link a discussion issue in the field `issue`.
- Mark one lesson `superseded` and name the lesson that replaces it in the field `by`.

A `contested` lesson without a valid issue link fails the check.
Reviewers also look for conflicts by reading, because the check cannot find conflicts nobody declared.

## Confirming a page without changing it

When a page has passed its `review-by` date, a scheduled workflow opens an issue.
Read the page, check the facts against their sources, and update anything that has drifted.
Then move `review-by` forward by pull request.
That edit is the confirmation, and the reviewer sees it in the diff.

## Checklist before you open the pull request

1. The lesson is one statement and under 80 words.
2. The ledger row exists, has a disposition and names the source.
3. The generator has computed the title and classes.
4. No private data is present.
5. The chapter's section "Sources and further reading" lists the source ID.
