---
steward: unassigned
deputy: unassigned
review-by: 2027-11-02
maturity: stub
applies-to: [jurisdiction]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to review conference contracts, establish who may sign, and do the insurance due diligence that Plone conference hosts must perform."
    "keywords": "Plone, Plone Conference, contracts, legal, insurance, liability, venue contract"
---

# Contracts, legal and insurance

## Why it matters

This chapter is general information, not legal, tax or insurance advice.
Check current rules with a qualified local adviser.

A conference is a bundle of contracts: venue, hotel, catering, equipment, ticket platform, sponsors and speakers.
Each one commits the team to dates, minimums and liabilities, often months before income arrives.
A minimum-attendance clause or a missing cancellation term can cost more than a bad week of sales.

Insurance is the part organizers know least about.
As of 2026-11, the Foundation states that organizers must work out locally which insurance types and limits the event needs, and that it cannot help because the rules differ widely between countries (L-4047, S005).
The question of who signs, and for whom, belongs to `legal-entity-and-financial-agent`.

## Applies when

- `jurisdiction` Contract law, liability rules and insurance requirements depend on the country of the venue and of the organizer.

## Decisions you must make

- {bdg-danger}`MUST` (req: R-012; as-of: 2026-11-02) **Have you done due diligence on local law to establish which insurance types and limits the event needs?** The Foundation's sponsorship policy and the hosting call of 2020 both require it (S005, S096). Whether you must show proof to the Foundation is an open question. (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Will you negotiate attendance minimums and cancellation terms before signing the venue contract?** One conference had a guaranteed minimum of 300 attendees, and the shortfall cost the organizers money (L-2022). (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Will you carry a participant insurance line in the budget?** One conference recorded such a line (L-3109). Whether you need one depends on the advice you receive. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Who signs each contract, and who may commit the conference?** Name the signer per contract type and write it down. See `legal-entity-and-financial-agent`. (decide-by: T-12m)

## How-to

1. List every contract the conference will sign, from venue and hotel to sponsors and speaker agreements.
   Done when each has an owner and a named signer.
1. Read each contract for minimum guarantees, cancellation and relocation terms, payment dates and liability.
   Done when the minimums and dates are in the budget and the timeline (L-2022).
1. Ask a local adviser which insurance types and limits the event needs (L-4047).
   Done when a written note names the types, the limits and the adviser.
1. Ask the venue which insurance it carries and what it expects from the organizer.
   Done when the answer is filed with the contract.
1. Close the insurance task with a dated decision, not an open issue (L-5034).
   Done when the decision log shows what you decided and why.
1. Store contracts in shared storage with limited access, and pass successors a redacted summary rather than the signed originals.
   Done when the next team can find terms without seeing private amounts.

## Principles and general lessons

No general lesson has passed the promotion rule yet.

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5034 | confidence: reported | status: active

The review records the venue-insurance due-diligence task as never completed.
An open legal-risk issue gave no decision gate before the event.
```

```{note} [specific · 2019 · n/a · 7 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2019 | place: n/a | org: Plone Foundation | source: S096 | ledger: L-4085 | confidence: observed | status: active

The 2020 call, the latest hosting call located, added insurance due diligence to the required elements of a bid.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S093 | ledger: L-3109 | confidence: observed | status: active

The expense record includes a line for participant insurance.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S016 | ledger: L-2022 | confidence: observed | status: active

The venue contract guaranteed a minimum of 300 attendees, so a shortfall below that minimum cost the organizers money.
```

## Risks

```{warning} The venue minimum exceeds actual attendance
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Negotiate the minimum at or below the low attendance case and plan the cost of a shortfall | owner-role: treasurer | playbook: low-ticket-sales

Judged for a mid-size conference.
```

```{warning} Insurance due diligence stays open until after the event
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Give the task a decision date in the master timeline and record the decision in the log | owner-role: legal lead

An open issue is not a decision.
```

```{warning} An incident exposes an insurance gap
:class: hb-risk hb-likelihood-low hb-impact-high
risk | likelihood: low | impact: high | mitigation: Get written advice on required cover and keep the answer with the venue contract | owner-role: legal lead | playbook: force-majeure

The cost falls on the organizing entity.
```

```{warning} Someone without authority signs a contract
:class: hb-risk hb-likelihood-low hb-impact-high
risk | likelihood: low | impact: high | mitigation: Name the signer for each contract type and check the signer's authority before signing | owner-role: legal lead

The organizing entity may not be bound by the signature.
```

## Thin content

```{warning} Proof of insurance
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A Foundation statement of whether hosts must show proof of insurance, and to whom | who-might-know: Foundation Board; Conference Committee

R-012 states the due-diligence duty and is silent on proof.
```

```{warning} Contract clauses and templates
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Sanitized clause checklists for venue, hotel and speaker agreements, with no private terms | who-might-know: Venue leads and treasurers of past conferences

The located sources record one minimum-guarantee clause and no other contract terms.
```

```{warning} Law outside the EU
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Dated accounts of contract and insurance practice in hosts outside Europe | who-might-know: Past organizers in the United States, Brazil and Japan | area: non-eu-legal-tax-visa

The Brasília line is the only insurance example outside Europe.
```

```{warning} Jurisdiction annexes
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Reviewed country annexes with the rules a host must check | who-might-know: Local advisers; past organizers per country | area: jurisdiction-annexes

The annexes are stubs.
```

## Sources and further reading

- S005 Plone Foundation, Plone Event and Sprint Sponsorship Policy.
- S016 Bristol 2010, "Plone Conference 2010, The Numbers".
- S093 Brasília 2013, PythonBrasil operational record.
- S096 2020 call for proposals, the latest hosting call located.
- S099 Maastricht 2026, GitHub issues and project board review.
