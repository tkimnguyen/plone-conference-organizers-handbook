---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: how-to
myst:
  html_meta:
    "description lang=en": "The yearly update process: who updates the handbook after each Plone conference, which handover items arrive, and when each step is due."
    "keywords": "Plone, Plone Conference, annual ritual, handover, update process, CalVer"
---

# The annual ritual

**Who keeps the handbook up to date, and when?**
The team that organizes the next conference updates the handbook together with the team that just finished.
The work takes about 120 days after the last conference day, and a scheduled workflow reminds everyone about stale pages all year.

The dates on this page count from the last conference day, T+0.
They are proposed, as part of the governance proposal in [Governance](governance.md), and the community may change them.

## Why a ritual

The origin problem of this project is that most conferences passed on little.
A ritual makes the handover a fixed event with named deliverables, so that updating the handbook does not depend on anyone's spare time.

## Who does what

- The **incoming team** leads the update.
- The **outgoing team** delivers the handover, answers questions and reviews the lessons from its own year.
- The **maintainer team** merges pull requests, runs the generator and cuts the release.
- The **stewards and deputies** of the touched chapters review.

## The handover deliverables

The outgoing team owes these items by T+60 days.
They are defined in the page `handover-contract`.

1. **Post-mortem**, on the Seattle 2006 skeleton; the template is `post-mortem-template`.
2. **Financial summary**: final income and costs by category, the result and the budget model, generalized.
3. **Anonymized survey data**: aggregates only.
4. **Asset and credential handover**: a list of accounts, domains and assets with their holders after the handover.
   Credentials pass through a password manager or the Foundation, never through the repository.
5. **Vendor contacts**: organization-level, handed over privately.
   The public handbook lists none.
6. **The "expected but never written down" list**: every implicit expectation the team ran into.

Two more items belong to the same contract.

- The **Tailoring Record**, filed later in the sequence; see [Tailor](../start/tailor.md).
- A **shadowing arrangement**: the incoming team follows the outgoing team's final months and the event itself.

## The sequence

| By | Step | Done looks like |
|---|---|---|
| T+60 days | The six handover deliverables arrive. | Each item is delivered, or its absence is recorded with a reason. |
| T+75 days | The post-mortem and the anonymized survey results are filed under `conferences/<year>-<city>/`. | Both files exist in the handbook's `docs/` tree and pass the privacy lint. |
| T+90 days | Lessons arrive as pull requests. | Every ledger row has a disposition, every lesson cites a ledger ID, and the promotion rule has been applied. |
| T+100 days | The outgoing team's Tailoring Record is filed as `conferences/<year>-<city>/tailoring.md`. | The record is merged. Recurring deviations are listed as candidates for a DEFAULT to become an OPTION. |
| T+110 days | The requirements register is re-verified and every MUST badge is re-dated. | The as-of date in each MUST badge equals that of its register row. |
| T+120 days | The release is cut. | `as-of-year` is bumped, the generator has run, help-wanted issues are refreshed, promotions are logged and the CalVer tag `<year>.1` exists. |

## Step by step

### 1. Collect the handover (by T+60 days)

1. The incoming team asks the outgoing team for the six deliverables in writing, with the date.
2. The outgoing team delivers what it has and lists what is missing.
3. A maintainer opens one tracking issue for the year and links each deliverable.
4. Credentials and vendor contacts stay out of the repository.

### 2. File the records (by T+75 days)

1. Place the post-mortem and the anonymized survey aggregates under `conferences/<year>-<city>/` in the `docs/` tree.
2. Check the files against the privacy rules: no personal data, no private amounts, no contact details.
3. Open a pull request.
   The continuous integration run applies the privacy lint.

### 3. Turn lessons into pull requests (by T+90 days)

1. Add a ledger row for each lesson worth keeping, with a disposition: placed in a chapter, or dropped with a reason.
2. Write the lessons as case notes, following [Update](update.md).
3. Apply the promotion rule: a specific lesson becomes general only with evidence from three independent conferences across two organizing bodies, or with a structural reason that does not depend on the year.
4. Record each promotion as one line in the changelog.
5. Review each lesson with a reviewer from a different organizing body than the one that ran that year.

### 4. File the Tailoring Record (by T+100 days)

1. The outgoing team copies its record into `conferences/<year>-<city>/tailoring.md`.
2. The maintainer team compares it with earlier records and opens an issue for each DEFAULT that several conferences deviated from.

### 5. Re-verify MUST items (by T+110 days)

1. The incoming team re-checks the Foundation requirements register against the Foundation's own documents.
2. It updates the as-of date of each verified row.
3. It re-dates every MUST badge that cites a changed row.
   Until that is done, the badges fail the lint on purpose.

### 6. Cut the release (by T+120 days)

1. Bump `as-of-year` in the handbook configuration by hand.
   Lesson ages follow from it.
2. Run the generator in write mode, then in check mode; see [Update](update.md).
3. Refresh the help-wanted issues from the thin registry; see [About the thin registry](thin-registry-about.md).
4. Tag the release with a CalVer tag: `2026.1`, then `2027.1` and each year after.
   There is one living main branch and no branch per year.
5. Report the bus-factor figure in the release notes.

## The stale-page workflow all year

A scheduled workflow runs monthly.
It lists every written page whose `review-by` date has passed and opens one issue per page, naming the steward and the deputy.
If a page already has an open freshness issue, it adds no second one.
Closing an issue takes a commit that moves `review-by` forward, which is the act of re-confirming the page.

The workflow lives in `.github/workflows/stale-pages.yml`.
It calls the freshness script, which belongs to the test harness.
If the script is absent, the workflow only reports that fact and does not fail.

## What the permanent record holds

The living handbook changes every year.
The conference records under `conferences/<year>-<city>/` do not.
They hold the post-mortem, the numbers, the Tailoring Record and source links for one year, and they are added to, never overwritten.
A tag such as `2026.1` is a citable snapshot of the handbook as it stood after that year's ritual.
