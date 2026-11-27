---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: explanation
myst:
  html_meta:
    "description lang=en": "A proposal for who keeps the handbook up to date: stewards, deputies, a maintainer team, CODEOWNERS and the Foundation as repository admin."
    "keywords": "Plone, Plone Conference, governance, stewardship, CODEOWNERS, maintainers"
---

# Governance

**Status: a proposal to the community, not a decision.**
Nothing on this page binds anyone until the Plone Foundation, the Conference Committee and conference organizers accept it.
Until then every `steward` and `deputy` field may read `unassigned`, and the incubating maintainers of the repository act as one interim team.

## The idea

Handbooks decay when their upkeep depends on goodwill.
This proposal ties the upkeep to something that already has to happen: the handover from one conference team to the next.

- Maintaining the handbook becomes part of an organizer's duties.
- The outgoing team owes a handover, listed in the page `handover-contract` and summarized in [The annual ritual](annual-ritual.md).
- The incoming team uses that handover to update the handbook.
- Community members who guide conference organizing across the years carry the stewardship, for example the marketing team that helps each organizing group.
  They can carry it from one conference to the next and guide the upkeep.

The model is a proposal because the people who would carry it have not yet agreed to it.
Version 1 ships the proposal together with the handbook, so the community can accept, change or reject it with the text in front of them.

## Roles

| Role | What it does |
|---|---|
| Steward | Is accountable for one page's accuracy. Named in the page's front matter. |
| Deputy | Steps in for the steward, so a page is never one person away from orphaned. Named in the front matter. |
| Maintainer team | Merges pull requests, runs the annual ritual with the incoming team and keeps the tooling working. |
| Incoming team | The team organizing the next conference. Performs the annual update with the outgoing team. |
| Outgoing team | The team that just ran a conference. Delivers the handover and assists the update. |
| Foundation | Holds repository admin after the transfer to the `plone` organization. |

## Rotation rules

1. The incoming team leads the annual update, and the outgoing team assists.
2. A lesson's author is never its only reviewer.
   For a lesson from year Y, one reviewer comes from an organizing body other than the one that ran Y.
3. A chapter's steward and deputy come from different organizations.
4. At each annual ritual a deputy may move up to steward, and the incoming team nominates the next deputy.
   Rotation guards against capture by one organizer.
5. The Foundation holds repository admin.
   Each annual release reports a bus-factor figure: the number of distinct people who can merge.

## Stewards and CODEOWNERS

Each page names a `steward` and a `deputy` in its front matter.
The values are `unassigned`, a GitHub handle or a GitHub team.
Pages at maturity `reviewed` or `proven` need a named steward.

The `CODEOWNERS` file at the root of the repository maps paths to GitHub teams, so that a pull request asks the right people for review.
A mapping for one workstream looks like this.

```text
/docs/workstreams/marketing/   @plone/conference-marketing
```

The proposal for the maintainer team has two parts.

- **Target model.**
  After the community accepts the proposal, `CODEOWNERS` names at least three maintainers across at least two organizations.
  This gate does not apply to version 1.
- **Interim model.**
  Until then, the repository's `CODEOWNERS` file lists the incubation team under the `syslabcom` organization as the single interim owner of every path.
  The file carries a comment block that states the target model, so nobody mistakes the interim entry for a final decision.

## Orphaned chapters

A chapter is orphaned when nobody is accountable for it: both `steward` and `deputy` read `unassigned`, or a named handle no longer resolves to an active person or team.
Orphans are flagged in three places.

1. The scheduled freshness workflow names the steward and the deputy in each overdue-page issue, and says `unassigned` when that is the case.
2. The coverage map shows the maturity of every page, so a `stub` without a steward stands out.
3. At each annual ritual the maintainer team lists orphaned chapters and asks the incoming team to nominate stewards.

An orphaned chapter is not removed.
It stays published, and its issue says that no one is looking after it.

## The Foundation as repository admin

The repository incubates under the `syslabcom` GitHub organization.
After the community has accepted the proposal, the repository is offered for transfer to the `plone` organization.
GitHub keeps redirects from the old address.
The Foundation then holds repository admin, and the maintainer team holds write access.
Hosting of the published site is left to the Plone community; the Read the Docs setup in the repository is an offering, not a commitment.

## Open questions

These questions remain open and belong to the community.

1. Who accepts this model: the Foundation board, the Conference Committee or both?
2. Is 60 days after the conference a realistic deadline for volunteer teams to deliver the handover?
3. Which team carries stewardship from version 1 onward?

Raise answers as issues or in a pull request that edits this page.
