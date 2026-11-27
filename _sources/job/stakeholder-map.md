---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "Who has a stake in a Plone Conference and what each group holds: Foundation, Conference Committee, community, sponsors, venue and local bodies."
    "keywords": "Plone, Plone Conference, stakeholders, Foundation, Conference Committee, organizing"
---

# Stakeholder map

## Why it matters

A Plone conference is never run by one body.
The Plone Foundation approves the name and selects the location, the Conference Committee holds the memory of earlier editions, the hosting team does the work, and the community, sponsors, venue and local public bodies each expect something different in return.
A team that does not know this map finds its stakeholders one surprise at a time, usually after a contract is signed or an announcement is out.

The map is not stable from year to year, because the host is not stable either.
As of 2026-11 the Committee page says that traditionally a different group proposes and hosts the conference each year, usually led by a Plone service provider (L-4024, S003).
The Foundation described the same pattern in 2015: a company, user group or other entity with ties to the community, running an event that is in essence not for profit (L-4076, S049).
Continuity therefore lives outside the hosting team, in the Foundation and in people who organized before.

Money, time and trust are all at stake.
Money, because the stakeholder who carries the loss risk decides how cautious the team must be.
Time, because every unnamed stakeholder adds a late conversation.
Trust, because the community notices when a decision that touches it was taken without it, and the chapter `community-and-speaker-expectations` covers that side in detail.

## Applies when

- `all` Every Plone conference has the same core stakeholders, whoever hosts it.

## Decisions you must make

- {bdg-secondary}`OPTION` **What kind of organizer are you: a service company, a volunteer group, a university or a mix?** The kind decides who carries loss risk, who signs contracts and who sells tickets. A university hosted in 2025 (L-4225), so the service-company pattern is not a rule. (decide-by: T-14m)
- {bdg-primary}`DEFAULT` (basis: L-1007, L-4023) **Which experienced community members will advise you, including the Conference Committee, and have they agreed?** Ask them before the bid is written, and agree how often you will report to them. (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Who is the single named contact for each stakeholder group?** One owner per group stops two people from giving a venue, a sponsor or the Board different answers. (decide-by: T-11m)
- {bdg-secondary}`OPTION` **Will you invite local public bodies or the host institution to open the conference?** In 2023 the mayor and regional representatives opened the talks (L-4193). This adds visibility for local funders and costs coordination time. (decide-by: T-6m)

## How-to

### Draw the map

1. Copy the table below into your Tailoring Record and add every group your own context adds.
   Done looks like one page that a team member who joins late can read in five minutes.
1. Write one owner next to each row.
   Done looks like a name in every cell of the owner column.
1. Write for each group one sentence on what they expect from you and one sentence on what you expect from them.
   Done looks like a list you can show to an experienced community member for correction.

| Stakeholder | What they hold | Where to read more |
|---|---|---|
| Foundation Board | Approves the event name, selects the location, may act as financial agent. | `bid-and-selection`, `legal-entity-and-financial-agent` |
| Conference Committee | Past organizers who keep process, checklists, people and vendors, and give each team continuity (as of 2026-11, S003). | `team-and-governance` |
| Hosting team | Delivers the event and carries the day-to-day risk. | `team-and-governance` |
| Community | Attendees, speakers, trainers and volunteers, with unwritten expectations. | `community-and-speaker-expectations` |
| Sponsors | Pay for visibility and have promises to be kept. | `sponsors` |
| Venue and hotels | Contract partners, sometimes a university or public body. | `venue`, `hotels-and-local-logistics` |
| Local public bodies | May open the event, fund it or host it. | This chapter |

### Make the map work

1. Meet the Conference Committee before you bid.
   The planning schedule it publishes starts the planning year (S004), and the register lists working with the Committee as guidance (row R-029, as of 2026-11-02).
   Done looks like a first meeting date in your calendar.
1. Ask the Foundation Board who is its current liaison for conferences.
   Done looks like a named liaison written in the map.
1. If the Foundation acts as financial agent, plan the Board's role in the budget and in your reporting rhythm with `legal-entity-and-financial-agent`.
   Done looks like a reporting calendar both sides have seen.
1. Name a deputy for each owner.
   Done looks like a second name per row, which is the first defense in `key-person-loss`.
1. Review the map at each planning milestone and after every change in the team.
   Done looks like a dated edit in the Tailoring Record.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S003, S009, S049 | ledger: L-1007, L-4024, L-4076 | confidence: observed | status: active | basis: independent-conferences

A different group hosts each year, so continuity does not live in the hosting team.
Ask a small circle of experienced community members to advise on strategic and tactical questions from the start.
```

## Case notes

```{note} [specific · 2025 · Jyväskylä · 1 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2025 | place: Jyväskylä | org: University of Jyväskylä | source: S081 | ledger: L-4225 | confidence: observed | status: active

The 2025 conference was organized by a university rather than a Plone service company, which broke the usual host pattern.
```

```{note} [specific · 2023 · Eibar · 3 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2023 | place: Eibar | org: CodeSyntax | source: S071 | ledger: L-4193 | confidence: reported | status: active

The mayor and regional commerce and innovation representatives opened the talks, stressing open source's contribution to local jobs and growth.
```

## Risks

```{warning} Key organizer leaves and takes stakeholder relationships along
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Name a deputy for every stakeholder group and keep a shared record of agreements and contacts | owner-role: lead organizer | playbook: key-person-loss

If one person alone holds the Foundation, sponsor and venue relationships, their absence stops decisions.
The judgment is for a typical mid-size conference run by a small team.
```

```{warning} A decision touching the community is announced without consulting it
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Show proposed changes to experienced community members before the announcement and record their answer

Community members who feel shut out of a process turn a practical decision into a trust problem.
See `community-and-speaker-expectations`.
```

## Thin content

```{warning} Committee mandate and Board liaison unconfirmed
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A written answer on whether the Conference Committee owns conference requirements, who the Board's current conference liaison is and how the member list is renewed | who-might-know: Foundation Board; Conference Committee | area: other | since: 2026-11-02

The Committee page claims no authority to set or waive requirements, and binding decisions sit with the Board.
How the two cooperate in practice is not documented in the sources read.
```

```{warning} Hosting by a university rests on one edition
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Accounts from other university-hosted or institution-hosted editions on what changed in roles, contracts and ticketing | who-might-know: Past university-hosted organizers; Conference Committee | area: other | since: 2026-11-02

Only the 2025 edition in the ledger was organized by a university.
```

## Sources and further reading

- S003 Conference Committee page, plone.org, as of 2026-11.
- S004 Conference Planning Schedule, plone.org, as of 2026-11.
- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
- S049 Call for proposals for the 2016 conference, which describes the organizer as a company, user group or other community entity.
- S071 Plone Conference 2023 recap.
- S081 Official Plone Conference 2025 record.
