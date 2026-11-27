---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: explanation
myst:
  html_meta:
    "description lang=en": "What the thin registry is, the three kinds of thin content, and how to claim a help-wanted item to close a gap in the handbook."
    "keywords": "Plone, Plone Conference, thin content, registry, help wanted, contributing"
---

# About the thin registry

A handbook is only as good as its weakest chapter, and the honest thing is to say where that is.
The thin registry is the public list of those places.
It tells readers how far to trust a page, and it tells contributors where help matters most.

## What the registry is

Every thin marker in the handbook is a small block inside a page, in the section "Thin content" of a chapter.
A generator script reads all the markers and writes one table, the page `thin-registry`.
Nobody edits that page by hand.
A drift check in the continuous integration run fails if the table does not match the markers.

The table has these columns: title (linked to the marker), page, kind, area, what is needed, who might know, issue and the date the marker was placed.
It is sorted by page, then by order on the page.
Combined with each page's maturity, the registry also feeds the coverage map.

A stub with a thin marker is better than a missing chapter.
That is why the handbook was published with its weak spots marked instead of hidden.

## The three kinds

| Kind | Meaning | Typical way to close it |
|---|---|---|
| `gap` | No evidence was located. | Provide a first source, or write the first account. |
| `single-source` | Exactly one source or one conference supports the content. | Add a second, independent account. |
| `stale` | Evidence exists, but it is older than the old threshold or known to be outdated. | Re-verify against the latest rules or practice and update the page. |

A marker may also carry one of ten areas where the handbook predicted thin evidence from the start.

- `hybrid-online`
- `accessibility`
- `non-eu-legal-tax-visa`
- `sponsorship-down-market`
- `pricing-elasticity`
- `small-budget`
- `health-safety`
- `sustainability`
- `jurisdiction-annexes`
- `post-mortem-2026`

A marker outside these areas uses `other`.

## What a marker looks like

The example below is a placeholder.
It shows the shape of a marker, not a real gap.

````markdown
```{warning} Example gap title
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: One sentence naming the evidence that would close the gap | who-might-know: Roles and groups, never private persons | area: other | issue: #0

A line or two of context.
```
````

The `needs` and `who-might-know` fields are required.
The `who-might-know` field names roles, groups or public organizations, never a private person.
The `issue` field links the help-wanted issue, and the `since` field holds the date the marker was placed.

## How to claim a help-wanted item

Each marker can have a matching help-wanted issue in the repository.
The maintainers refresh these issues from the registry at each annual release.

1. **Pick an item.**
   Browse the registry or the issues labeled for help wanted.
   Start with an area you know first-hand.
2. **Claim it.**
   Comment on the issue to say you are taking it, and state what you plan to deliver.
   A maintainer assigns the issue to you.
3. **Collect the evidence.**
   Find a source that can be cited, or write down your own conference's experience.
   Keep it general: no personal data, no private amounts, no contact details.
4. **Send the evidence in.**
   For a lesson, follow [Update](update.md).
   For a chapter rewrite or an annex, follow [Extend](extend.md).
5. **Close the marker in the same pull request.**
   Remove the marker when the gap is closed.
   Change its kind, for example from `gap` to `single-source`, when you only partly close it.
   Update the maturity of the page when the evidence supports it.
6. **Release the claim if you cannot finish.**
   Say so in a comment, so another contributor can pick the item up.
   A steward may release a claim that has gone quiet.

## What a marker is not

A thin marker is not a failure and not a ranking of importance.
Some gaps are thin because few conferences ever faced the problem.
Some are thin because nobody wrote it down.
Both are fair reasons to ask for help.

## Related pages

- [How to read lessons](../start/how-to-read-lessons.md) explains how to read a marker as a reader.
- [The annual ritual](annual-ritual.md) shows when the issues are refreshed.
- [Governance](governance.md) explains who reviews your contribution.
