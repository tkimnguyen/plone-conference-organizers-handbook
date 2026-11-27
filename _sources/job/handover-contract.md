---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "What an organizing team owes the next one: the six handover deliverables, shared access to accounts and domains, and the list of expectations nobody wrote down."
    "keywords": "Plone, Plone Conference, handover, post-mortem, credentials, continuity"
---

# Handover contract

## Why it matters

Every Plone conference is organized by a team that then disbands.
What it learned leaves with it unless someone writes it down for the next team.
The Seattle 2006 organizers wrote a lessons document addressed to future organizers, and the practice faded afterwards.
As of 2026-11-02 the archive holds few written handovers, and the Foundation's own call for proposals treats earlier organizers' reports as the de facto handover material (L-4065).

The loss is not only knowledge of what worked.
It is the set of things everyone expected to exist and nobody had written down: who holds the domain, where the budget model lives, which supplier answers the phone, what the Foundation expects.
Each next team rediscovers them the hard way, usually in the last month.

This chapter is the origin of the handbook.
It sets out what an outgoing team owes the next one, and when.
The deliverables are a proposal that the community has yet to accept, and the [governance page](../running/governance.md) says how they feed the annual update.

## Applies when

- `all` Every Plone conference ends with a handover, whether or not the team plans one.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-3078, L-4023) **Who on the Conference Committee is your continuity contact, and when do you first meet?** The Committee consists of past organizers who keep the processes, checklists, people and vendors, and the Committee works with each year's team. Meet it before the first major commitment. (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-1003, L-2031) **Will you publish your evaluation and your budget model in generalized form?** Two conferences published their results and budget model so that later hosts would have what the organizers wished they had when bidding. Publish figures only in the generalized form the handbook allows, never private amounts. (decide-by: T-6m)
- {bdg-primary}`DEFAULT` (basis: L-1003, L-3001) **Who owns the six deliverables, and by when are they due?** Assign an owner for each of the six deliverables below. The proposed deadline is 60 days after the last conference day, and the deadline is a proposal, not a rule. (decide-by: T-3m)
- {bdg-secondary}`OPTION` **Where will credentials and account access live?** The 2011 team recommended one shared, team-owned place for all access information (L-3045). The advice comes from one conference. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will the next host shadow your final months and the event?** One lead organizer traveled to meet the previous organizers and called it invaluable (L-2024). A formal shadow arrangement is proposed and untested. (decide-by: T-6m)

## How-to

### Before the conference

1. Meet the Conference Committee and agree how you will report to it. Done when you know who is the contact for each exchange.
1. Start the list of expectations nobody wrote down. Whenever someone says "of course X exists" and X did not, add a line with what was assumed and what actually happened. Done when the list has an owner and a place in the tracker.
1. Keep all account access information in one shared, team-owned place, so that transferring the conference's digital assets means granting access to the next hosts (L-3045).
1. List every asset the team holds: social media accounts, shared storage with design files, mail routing, the domain, code repositories, chat channels, mailing lists and the schedule service. Done when each asset has a holder and a deputy holder.
1. Move the domain and its DNS to the Foundation, or plan how and when you will, and never leave mail routing in one person's personal setup. Done when no single person is the only way to reach the domain.
1. Keep the working archive in one repository or one shared folder, so that it can be handed over as one object.

### After the conference

1. Deliver these six items to the next team within 60 days of the last conference day (proposed deadline).
   1. The post-mortem, on the Seattle 2006 outline.
   1. The financial summary: final income and costs by category, the result and the budget model, in generalized form.
   1. Anonymized survey data, as aggregates only.
      Keep the raw submissions private and out of version control, and number respondents instead of naming them; quoted free text can still re-identify people to insiders (L-6004).
   1. The asset and credential handover: a list of accounts, domains and assets with the holders who take them over.
      Credentials pass through a password manager or the Foundation, never through a repository.
   1. Vendor contacts at organization level, handed over privately, never in the public handbook.
   1. The list of expectations nobody wrote down.
1. List earmarked money and stored equipment next to the financial summary and the asset list, so the next team knows what carries over.
1. Hand over volunteer and attendee contact lists only where a lawful basis exists. Otherwise hand over the role and the method, not the list.
1. Agree a shadowing arrangement if you want one: the next host follows your final months and the event.
1. File the post-mortem and the Tailoring Record in the handbook's conference case folder. See the [governance page](../running/governance.md).

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S003, S016, S034 | ledger: L-2031, L-3078, L-4023 | confidence: observed | status: active | basis: independent-conferences

Continuity does not happen by itself.
It takes published figures and a published budget model, direct work with the previous organizers, and a standing group of past organizers who remember what has to be done when.
```

## Case notes

```{note} [specific · 2016 · n/a · 10 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2016 | place: n/a | org: Plone Foundation | source: S052 | ledger: L-4078 | confidence: observed | status: active

The 2017 call removed two organizer reports from its list of four recommended past accounts.
It offered instead to put bidders in personal contact with previous organizers.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S022 | ledger: L-3001 | confidence: observed | status: active

The organizers left a thirteen-page wiki guide for their successors.
It covered budget, tickets, volunteers, talks, resources, print, nonprofit status, the domain handover and a supplies list.
It is one of the few written handovers in the series.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S024 | ledger: L-3022 | confidence: observed | status: active

Scholarship money raised in 2011 was earmarked for the next conference.
It had to be carried into that budget and paid out through the Foundation.
Earmarked funds are a handover item.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S025 | ledger: L-3032 | confidence: observed | status: active

The volunteer list lived in a mailing-list service and a shared spreadsheet, and the guide told successors to ask previous volunteers for help.
Contact lists like this are personal data and need a lawful basis before they pass to a team.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S027 | ledger: L-3041 | confidence: observed | status: active

Equipment bought with conference funds became Foundation property and went into storage.
It was offered for shipping to any later event, with a published inventory.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S028 | ledger: L-3046 | confidence: observed | status: active

The handover inventory of digital assets listed social media accounts, shared storage with all design files, conference-domain email with an FAQ folder, the domain, code repositories, a chat channel, the mailing-list service and the schedule service.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S028, S031 | ledger: L-3048, L-3063 | confidence: observed | status: active

Conference email routing sat with one organizer's personal DNS setup, a single-person dependency.
At handover the domain's ownership and DNS still had to be transferred to the Foundation.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S015 | ledger: L-2019 | confidence: observed | status: active

The organizers credited their success partly to adopting the best parts of previous conferences.
They hired the previous host's Wi-Fi specialist again.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S016 | ledger: L-2024 | confidence: observed | status: active

The lead organizer traveled to meet the previous year's organizers to learn what had and had not worked.
The lead called the visit invaluable.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S016 | ledger: L-2025 | confidence: observed | status: active

The working budget lived in an online spreadsheet whose revision history anonymous readers could not see.
The evolution of the budget was lost to successors.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S008, S009 | ledger: L-1003, L-1037 | confidence: observed | status: active

The organizers published their whole evaluation on one public page: surveys, attendee comments, the detailed budget as a public spreadsheet with total staff hours, and a narrative lessons document for future organizers.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1004 | confidence: observed | status: active

The lead organizer wrote the lessons document after the event, with input from the co-organizer, finance staff and community advisers.
It states its purpose as passing the host organization's experience to future Plone event organizers.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1005 | confidence: observed | status: active

Per-session evaluation results were kept private but offered to future organizers on request.
No public record shows whether that handover happened.
```

## Risks

```{warning} One person is the only route to the domain or the mail
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Keep access information in one shared team-owned place and move the domain and mail routing to the Foundation or to a role account | owner-role: asset steward | playbook: key-person-loss

A single-person dependency surfaced at one past handover.
If that person is unreachable at the wrong time, the site and mail stop with them.
```

```{warning} The handover is written once and never maintained
:class: hb-risk hb-likelihood-high hb-impact-medium
risk | likelihood: high | impact: medium | mitigation: Name an owner for each deliverable, set a date and store the output where the next team can find it without asking | owner-role: outgoing lead

A written guide that nobody owns ages into a trap.
Past organizer reports have dropped off official lists, and spreadsheet histories have been lost.
```

```{warning} Personal data passes to the next team without a lawful basis
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Hand over roles and methods, not contact lists, unless a lawful basis for the transfer is documented | owner-role: privacy lead

Volunteer and attendee lists are personal data.
```

```{warning} Earmarked funds and stored equipment are lost in the transition
:class: hb-risk hb-likelihood-low hb-impact-medium
risk | likelihood: low | impact: medium | mitigation: List earmarked money and stored equipment next to the financial summary and the asset list | owner-role: treasurer

These items are easy to forget because they belong to neither team's regular work.
```

## Thin content

```{warning} The six deliverables have not been delivered by a team yet
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A first outgoing team that delivers the six items and reports whether the 60-day deadline was realistic | who-might-know: The organizers of the next conference; Conference Committee | area: other

The deliverables and the deadline are a proposal under review, not an accepted rule.
```

```{warning} Asset and credential practice rests on one conference
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second conference's account of how it transferred domains, accounts and mail, and what went wrong | who-might-know: Past organizers; Foundation web and infrastructure roles | area: other

Both the inventory and the advice to keep access in one team-owned place come from the 2011 wiki.
```

```{warning} Few written handovers are archived
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Written handover material from hosts after 2013, so that the handbook can compare what each team passed on | who-might-know: Past organizers; Conference Committee | area: other

As of 2026-11-02 the archive holds no written handover between successive hosts after the 2011 guide.
```

## Sources and further reading

- S003 Plone Conference Committee, team page.
- S008 Seattle 2006, complete evaluation hub.
- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
- S015 Bristol 2010, host company blog, "An Organiser's View".
- S016 Bristol 2010, host company blog, "The Numbers".
- S022 San Francisco 2011, "Guide for Organizing a Plone Conference", GitHub wiki.
- S024 San Francisco 2011, wiki page "Tickets".
- S025 San Francisco 2011, wiki page "Managing Volunteers".
- S027 San Francisco 2011, wiki page "Physical Resources".
- S028 San Francisco 2011, wiki page "Virtual Resources".
- S031 San Francisco 2011, wiki page "Ploneconf.org handover".
- S034 San Francisco 2011, organizer interview.
- S049 Foundation call for proposals, 2016.
- S052 Foundation call for proposals, 2017.
- S110 Maastricht 2026 attendee survey analysis.
