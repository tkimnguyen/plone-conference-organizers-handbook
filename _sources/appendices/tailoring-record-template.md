---
steward: unassigned
deputy: unassigned
review-by: 2028-11-01
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "A copyable Tailoring Record: the Adopt, Adapt, Skip and Replace table with a decision-record style reason column and a worked example."
    "keywords": "Plone, Plone Conference, Tailoring Record, adopt adapt skip replace, template"
---

# Template: Tailoring Record

The handbook is tailored by overlay, not by fork.
You keep the text as it is, record where your conference deviates, and file the record as evidence.
This page holds the template and one worked example.
The method behind it is on the page [Tailor](../start/tailor.md), which you should read first.

The record lives in your own planning repository while you plan.
After the conference you file it in the handbook under `conferences/<year>-<city>/tailoring.md`, inside the `docs/` tree.
The target date is 100 days after the last conference day, as set out in [The annual ritual](../running/annual-ritual.md).

## Copy this template

````markdown
# Tailoring Record: <conference name and year>

Handbook release: <CalVer tag, for example 2026.1>
Record owner: <role>
Filing date: <YYYY-MM-DD, 100 days after the last conference day>

## Context

| Dimension | Our value |
|---|---|
| size | small, medium or large |
| jurisdiction | ISO country code such as NL, or EU |
| organizer | company, volunteer-group, foundation-led or mixed |
| budget | seed-loan, financial-agent or own-risk |
| venue | hotel, university, conference-center or mixed |
| format | in-person, hybrid or online |
| language | ISO language code such as en |

## Decisions

| Chapter id | Choice | Reason | Owner | Date |
|---|---|---|---|---|
| finance | Adopt, Adapt, Skip or Replace | Context, Decision, Consequence | Role | YYYY-MM-DD |

## Foundation exceptions

| Requirement | Exception granted | Link or reference |
|---|---|---|
| R-000 | What the Foundation agreed in writing | Where the written exception is filed |
````

## How to fill it in

1. Fill the context block first. The dimension values come from the page [Tailor](../start/tailor.md) and from each chapter's "Applies when" section.
1. Open the generated decision register and add one row for every badged decision you rely on, in chapter order. One line in the register becomes one row in your table.
1. Pick one of the four choices for each row, using the table below.
1. Write the reason in three short parts, in the style of an architecture decision record: Context, Decision, Consequence.
1. Add an owner role and a date. The owner is the role that will answer questions about the row later, not the person who typed it.
1. For every deviation from a MUST, add a row to the Foundation exceptions table and link the written exception. A legal necessity cannot be waived by the handbook.
1. At handover, check that each deviation from a DEFAULT has a three-part reason and that the record has an owner who knows the filing date.

## The four choices

| Choice | Meaning | What the reason must say |
|---|---|---|
| Adopt | You follow the chapter as written. | Nothing beyond the name of the chapter. For a DEFAULT, one clause on why the default fits. |
| Adapt | You follow it with changes. | What changed. |
| Skip | You do not do it. | Why that is safe in your context. |
| Replace | You do something else for the same purpose. | What you do instead, and why it is better here. |

## What a deviation needs, by level

| Level | What a deviation needs |
|---|---|
| MUST | A written Foundation exception, linked in the Foundation exceptions table. |
| DEFAULT | A recorded reason in the three-part form. |
| OPTION | Nothing beyond naming your choice. |

## Writing the reason

The reason has three parts, each one sentence.

- **Context** names the facts of your situation that drive the choice.
- **Decision** says what you chose, in one sentence.
- **Consequence** says what you accept or must watch because of it.

Write for the reader who opens the record in two years, after the team has moved on.
A reason such as "it did not fit" tells that reader nothing.

## Worked example

The example uses a fictional conference.
It shows three of the four choices.
An Adopt row would read, for example, "ticketing-and-registration, Adopt, Context: the default platform fits our payment methods, Owner: Ticketing lead".

````markdown
# Tailoring Record: Example Conference 2027, Exampletown

Handbook release: 2026.1
Record owner: Conference chair
Filing date: 2028-01-15

## Context

| Dimension | Our value |
|---|---|
| size | small |
| jurisdiction | XX |
| organizer | volunteer-group |
| budget | own-risk |
| venue | university |
| format | in-person |
| language | en |

## Decisions

| Chapter id | Choice | Reason | Owner | Date |
|---|---|---|---|---|
| finance | Adapt | Context: the university collects fees and pays suppliers for us. Decision: we keep a shadow budget and skip our own books. Consequence: the treasurer reconciles against the university statement each month. | Treasurer | 2027-02-10 |
| hybrid-online | Skip | Context: the venue has no upstream capacity for a stream and nobody on the team has capacity to run one. Decision: we record rooms and publish after the event. Consequence: remote followers wait for the recordings. | AV and recording lead | 2027-03-05 |
| cfp-and-selection | Replace | Context: the team is small and the community is local. Decision: we invite talks from known contributors and open a short call for the rest. Consequence: fewer unknown speakers, a narrower program. | Program lead | 2027-03-20 |
````

## Where the record goes after the conference

1. File the record under `conferences/<year>-<city>/tailoring.md`, in the handbook's `docs/` tree, by 100 days after the last conference day.
1. Open a pull request. Records are only added, never overwritten.
1. Strip names and private amounts first, because the handbook publishes generalized information only.
1. Expect the stewards to read recurring deviations as a signal. When several conferences deviate from the same DEFAULT for similar reasons, that DEFAULT becomes an OPTION, or the chapter gains a regional or variant section.

The record is evidence, not a report card.

## Applies when

Every team that uses the handbook should keep a Tailoring Record, whatever the size of the conference.

## Thin content

```{warning} No filed record yet
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A filed Tailoring Record from a real conference, to test the template and the level rules against actual deviations | who-might-know: The organizing team of the next conference; the handbook stewards

The template follows the method in the page Tailor and has not been used for a full conference.
The Foundation exceptions table is an addition to that method and needs to be tested the same way.
```

## Sources

This template has no external source.
It implements the method on the page [Tailor](../start/tailor.md) and the filing step in [The annual ritual](../running/annual-ritual.md).
