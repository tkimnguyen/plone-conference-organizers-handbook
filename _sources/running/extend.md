---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: how-to
myst:
  html_meta:
    "description lang=en": "How to extend the handbook: add a chapter, a jurisdiction annex or a lesson, and how changes to the specification are made."
    "keywords": "Plone, Plone Conference, extend, chapter, annex, jurisdiction, specification"
---

# Extend

The handbook grows by adding things: a chapter nobody has written, an annex for your country, a lesson from your conference.
This page shows each route and ends with the rule for changing the specification itself.

## Add a chapter

Nobody writes a page that is not in the master chapter list.
The list comes first, then the page.

1. **Open an issue** that names the topic and the reason the handbook needs it.
   Check the existing chapters first: a topic has one canonical home, and a duplicate only creates conflicting advice.
2. **Add an entry** to `docs/spec/chapter-list.yml` with `status: planned`.
   The entry needs an id (lowercase letters, digits and hyphens), a title in sentence case, the part, the workstream, the kind, the path under `docs/` and the status.
3. **Take the expected-failure slot.**
   The contract test treats every `planned` entry as an expected failure.
   You do not edit the test; the entry is the slot.
4. **Name a steward and a deputy** from different organizations in the issue.
   The front matter may read `unassigned` while the page is a stub or a draft.
5. **Copy the chapter skeleton** from `docs/spec/chapter-template.md`, section 9.
   It has the nine fixed sections in their fixed order.
6. **Write from ledger evidence.**
   Each decision carries a badge: MUST cites the requirements register, DEFAULT cites at least two ledger IDs from two conferences, OPTION cites nothing.
   Add thin markers wherever the evidence is weak.
   A stub must have at least one thin marker.
7. **Write the page and flip the entry in one commit.**
   The same commit sets `status: written` in the chapter list.
   An unexpected pass fails the build and forces this cleanup.
8. **Open a pull request** and ask the steward and a reviewer from another organization to review it.

A chapter may hold at most 2500 words, excluding its section *Sources and further reading*.
Above that it must split: add entries with ids of the form `<parent-id>-<subtopic>`, move the content and leave links behind.
The parent stays as the overview page.

Other kinds of page follow lighter rules.
A `page` has free structure.
A `playbook` has exactly four sections: Triggers, First-hour actions, Owner roles and Related chapters.
An `appendix` holds a template or a reference and carries no real names, amounts or contacts.

## Add a jurisdiction annex

Annexes hold what cannot be one-size-fits-all.
The first four are the Netherlands, Germany, the United States and Brazil.
Yours may be next.

1. **Add the chapter-list entry** with `kind: annex`, an id of the form `annex-<code>` and the path `docs/annexes/jurisdictions/<code>.md`, where `<code>` is the lowercase country code.
2. **Start as a thin stub.**
   Write the front matter with `maturity: stub`, `applies-to: [jurisdiction=<CODE>]` and `jurisdiction: <CODE>`, where `<CODE>` is the uppercase ISO 3166-1 code.
   The `jurisdiction` field is allowed on jurisdiction annexes only.
3. **Open the page with the disclaimer**, in exactly these words.
   Place it on the first lines after the heading.

   > This annex is general information, not legal, tax or insurance advice.
   > Check current rules with a qualified local adviser.

4. **Add a thin marker** with `area: jurisdiction-annexes` that names what would close the gap, and the roles that might know, such as a qualified local adviser or a past organizer in that country.
5. **Set a short `review-by` date.**
   Annexes may use at most 12 months, because tax and legal facts change fast.
6. **Grow it by pull request**: general notes on tax, legal form, insurance and permits, each with a dated source.
   Never paste a private figure or a contact.

A variant annex, for example for small-budget conferences, uses the path `docs/annexes/variants/<name>.md` and the same disclaimer and rules, without the `jurisdiction` field.

## Add a lesson

A lesson is the smallest extension.
Follow [Update](update.md): issue form, ledger row, admonition block, steward review.

## Add a template

Templates live in the appendices and are referenced from at least one page.
They contain no real names, amounts or contacts.
Add an appendix entry to the chapter list first, as for a chapter.

## How the specification changes

The specification in `docs/spec/` is the single source of truth for what a page looks like and what is checked.
It changes by pull request, like any other file.

1. **One commit updates every file that mentions the thing you change.**
   A field, a vocabulary or a rule is mentioned in several places: the spec files, the chapter pages that describe it, the generator and the tests.
   Search the repository for the field name before you commit.
2. **Update the tests first.**
   The tests and the generator are the first files to change when a rule changes.
3. **Vocabularies are fixed.**
   The allowed values for a field are defined by the spec tables and are not configurable.
   Only the keys in `handbook-config.yml` are tunable, such as the age thresholds, the word budget and the ID patterns.
4. **The spec says what is checked, not how scripts are named or laid out.**
   Script names and layout are decisions of the people who build the tests.
5. **Say why in the pull request.**
   A change that affects authors needs a note in the changelog.

A change to stewardship, such as the rules on `CODEOWNERS`, is a change to the proposal in [Governance](governance.md) and needs the community's agreement, not only a review.

## Checklist

1. A chapter, annex or template has a chapter-list entry before it has a page.
2. A stub has at least one thin marker.
3. An annex carries the disclaimer and a short `review-by` date.
4. The commit that writes a page flips its status in the same commit.
5. A spec change touches every file that mentions the changed rule.
