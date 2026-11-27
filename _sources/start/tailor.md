---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: how-to
myst:
  html_meta:
    "description lang=en": "How to adapt the handbook to your Plone conference by overlay, not by fork: context dimensions, the Tailoring Record and annexes."
    "keywords": "Plone, Plone Conference, tailoring, Tailoring Record, context dimensions, annexes"
---

# Tailor

No two Plone conferences are alike.
A 90-person volunteer event in one country needs different advice from a 500-person event run by a company in another.
Forking the handbook for each conference would fragment it, and the next team would again start from nothing.
So the handbook tailors by overlay: you keep the text as it is, record where you deviate and why, and send the record back as evidence.

The process has four steps.

1. Classify your conference along the context dimensions.
2. Copy the Tailoring Record and answer it chapter by chapter.
3. Use the annexes for content that cannot be one-size-fits-all.
4. File the record at handover, so recurring deviations improve the handbook.

## Step 1, classify your conference

Every chapter declares which conferences it fits, in its front matter field `applies-to` and in a section called *Applies when*.
Each entry in that section is a token built from a dimension and one or more values.
Compare your conference with each dimension.

| Dimension | Values |
|---|---|
| `size` | `small` (up to 150 attendees), `medium` (150 to 400), `large` (more than 400) |
| `jurisdiction` | An ISO 3166-1 country code such as `NL`, or `EU` |
| `organizer` | `company`, `volunteer-group`, `foundation-led`, `mixed` |
| `budget` | `seed-loan`, `financial-agent`, `own-risk` |
| `venue` | `hotel`, `university`, `conference-center`, `mixed` |
| `format` | `in-person`, `hybrid`, `online` |
| `language` | An ISO 639-1 language code such as `en` |

A chapter token such as `size=medium,large` means the chapter applies to those sizes.
A bare dimension such as `jurisdiction` means the chapter applies to every value and its content varies by that dimension.
A chapter marked `all` applies to every conference.

If your conference is outside a chapter's *Applies when* section, you have two honest options: adapt the advice, or skip the chapter and record why.

Write your classification once, at the top of your Tailoring Record.
The page `context-dimensions` holds the longer explanation of each dimension.

## Step 2, copy the Tailoring Record

The Tailoring Record is a table with one row per chapter you touch.
Copy it into your own planning repository, not into the handbook.
Fill the context block first, then add a row each time you decide something.

````markdown
# Tailoring Record: <conference name and year>

Handbook release: <CalVer tag, for example 2026.1>

## Context

| Dimension | Our value |
|---|---|
| size | |
| jurisdiction | |
| organizer | |
| budget | |
| venue | |
| format | |
| language | |

## Decisions

| Chapter id | Choice | Reason | Owner | Date |
|---|---|---|---|---|
| finance | Adopt / Adapt / Skip / Replace | Context, decision, consequence | Role | YYYY-MM-DD |
````

The four choices mean the following.

- **Adopt**: you follow the chapter as written.
- **Adapt**: you follow it with changes.
  Say what changed.
- **Skip**: you do not do it.
  Say why that is safe for your context.
- **Replace**: you do something else for the same purpose.
  Say what, and why it is better here.

The reason is written in the style of an architecture decision record, in three short parts.

- **Context**: the facts of your situation that drive the choice.
- **Decision**: what you chose, in one sentence.
- **Consequence**: what you accept or must watch because of it.

How much you must write depends on the level badge of the decision.

| Level | What a deviation needs |
|---|---|
| MUST | A written Foundation exception, linked in the record. A legal necessity cannot be waived by the handbook. |
| DEFAULT | A recorded reason in the three-part form above. |
| OPTION | Nothing beyond naming your choice. |

The generated decision register lists every badged decision in the handbook, in chapter order.
Use it as the checklist for the record: one line in the register, one row in your table.
The page `tailoring-record-template` will hold the complete template with an example per level.

An illustrative row:

````markdown
| ticketing-and-registration | Adapt | Context: attendees are nearly all community members who pay by bank transfer. Decision: use invoice payment through a self-hosted platform. Consequence: we handle reminders by hand. | Treasurer | 2027-01-15 |
````

## Step 3, use the annexes

Content that cannot be one-size-fits-all lives in annexes.

- **Jurisdiction annexes** under `annexes/jurisdictions/` collect general notes on tax and legal points for one country.
  The first four are the Netherlands, Germany, the United States and Brazil, and all of them start as thin stubs.
- **Variant annexes** under `annexes/variants/` adapt the advice to a type of conference.
  The first is the small-budget variant, also a stub.

Every annex opens with this disclaimer: "This annex is general information, not legal, tax or insurance advice.
Check current rules with a qualified local adviser."
Each annex has its own `review-by` date, shorter than that of a normal chapter, because tax and legal facts change fast.
If your country has no annex, say so in your record and consider writing one; see [Extend](../running/extend.md).

## Step 4, file the record at handover

When the conference is over, the outgoing team files its Tailoring Record under `conferences/<year>-<city>/tailoring.md`, inside the handbook's `docs/` tree.
The target date is 100 days after the last conference day, as set out in [The annual ritual](../running/annual-ritual.md).
Records are never overwritten, only added to.

The record is evidence, not a report card.
When several conferences deviate from the same DEFAULT for similar reasons, that DEFAULT becomes an OPTION, or the chapter gains a regional or variant section.
Your deviations are how the handbook learns your context.

## Checklist

1. You have written your context block.
2. Every chapter you rely on has a row, or you have decided to rely on the defaults and said so.
3. Every deviation from a DEFAULT has a three-part reason.
4. Every deviation from a MUST links a written Foundation exception.
5. The record has an owner, and the owner knows the filing date.
