---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "The license of the handbook, how to contribute through the Plone Contributor Agreement route, and the writing rules every page follows."
    "keywords": "Plone, Plone Conference, license, CC BY 4.0, contributing, Plone Contributor Agreement"
---

# License and contribute

## License

The text and illustrations of this handbook are licensed under the [Creative Commons Attribution 4.0 International license](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0).
You may copy, adapt and redistribute the content, including for commercial use, if you credit the handbook and indicate what you changed.
The full text is in the file `LICENSE` at the root of the repository.

Plone and the Plone logo are registered trademarks of the Plone Foundation.
Guidelines for their use are at <https://plone.org/foundation/logo>.

## The contributor agreement

The handbook follows the practice of the Plone documentation: contributors grant permission through the Plone Contributor Agreement.
The agreement is explained on the [Plone documentation contributing pages](https://6.docs.plone.org/contributing/index.html).
A volunteer member of the Plone Foundation reviews each signed agreement.
Sign and return the agreement before, or together with, your first substantial contribution.
If you are unsure whether a small change needs it, ask a maintainer in the pull request.

## Ways to contribute

Every kind of contribution is welcome, from a fixed typo to a whole chapter.
The paths are described in the repository's `CONTRIBUTING.md`, in the same two-path form as the Plone documentation.

- **Small fixes** go through the web interface of GitHub.
  Open the file, use the edit button, and propose the change.
- **Larger work** goes through a fork, a branch and a pull request, with a local build.

For the content itself, use these pages.

| You want to | Read |
|---|---|
| Add a lesson from your conference | [Update](../running/update.md) |
| Correct a fact | [Update](../running/update.md) |
| Add a chapter, an annex or a change to the spec | [Extend](../running/extend.md) |
| Help close a gap | [About the thin registry](../running/thin-registry-about.md) |
| Understand who reviews | [Governance](../running/governance.md) |

## Writing rules

These rules apply to every page and are checked in the continuous integration run.

1. **American English.**
   Use the spelling of the Plone documentation.
   The words "organizers" and "organisers" both lead to the handbook through the title and the search terms.
2. **One sentence per line** in the Markdown source.
   This keeps diffs and reviews readable.
3. **Sentence-case headings.**
   Capitalize only the first word and proper nouns.
4. **Plain words.**
   No exclamation marks, no emojis, no hype.
   Prefer commas and periods over dashes.
5. **Dated claims.**
   Do not use words whose meaning depends on the day the page is read without a dated anchor.
   Write "as of 2026-11" instead.
6. **Prices, tax rates and fees** appear only as dated, sourced examples, never as rules.
7. **Generalized information only.**
   No personal data, no private amounts, no contact details and no ticket-buyer data ever enter the handbook.
   Paraphrase, aggregate and anonymize, then check.
8. **Advisory voice.**
   The handbook offers advice.
   It is not Foundation policy and it is not legal, tax or insurance advice.

## The specification

The content contract lives in `docs/spec/` in the repository and is not part of the published handbook.
It defines the chapter template, the front matter, the badges and blocks, the lesson ledger and the governance proposal.
When a page and the specification disagree, the specification is the reference, and the page is corrected.
The specification changes by pull request; see [Extend](../running/extend.md).

## Where to go next

Return to [Choose your path](choose-your-path.md) if you came to read, or to [Update](../running/update.md) if you came to give back.
