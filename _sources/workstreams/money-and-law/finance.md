---
steward: unassigned
deputy: unassigned
review-by: 2027-11-02
maturity: draft
applies-to: [budget, jurisdiction]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to budget a Plone conference, bridge the cash gap, handle the Foundation share and VAT, and keep books a successor can read."
    "keywords": "Plone, Plone Conference, finance, budget, cash flow, VAT, accounting"
---

# Finance

## Why it matters

A Plone conference spends money before it earns any.
Deposits, catering and equipment fall due while sponsor and ticket income is still arriving, so the team carries a gap that grows toward the final weeks.
Teams that did not plan for the gap fronted costs from private funds or borrowed from friends.

The Plone Foundation may act as financial agent and collects a share of registration income.
The host company or association rarely recovers its staff time in full.
VAT adds difficulty when the organizer and the event sit in different countries.

Good finance work means a budget the whole team can read, cash when bills arrive, and books a successor can pick up.
The steps are in the How-to section.

## Applies when

- `budget` The money flow differs by model: a seed loan, the Foundation as financial agent, or the organizers' own risk.
- `jurisdiction` VAT, accounting rules and payment options depend on the country of the organizer and of the event.

## Decisions you must make

- {bdg-danger}`MUST` (req: R-007; as-of: 2026-11-02) **Does your proposal state whether the Foundation acts as financial agent?** The Foundation's event financial policy requires an explicit statement. The legal side belongs to `legal-entity-and-financial-agent`. (decide-by: T-18m)
- {bdg-danger}`MUST` (req: R-008; as-of: 2026-11-02) **If the Foundation is your financial agent, have you budgeted your own work hours?** The Foundation takes the financial risk and lends its bank accounts, accounting systems and Treasurer, but does not pay the organizers' extra hours. (decide-by: T-18m)
- {bdg-danger}`MUST` (req: R-009; as-of: 2026-11-02) **If the Foundation is your financial agent, have you agreed Board updates and Board authority?** The Board receives regular updates, joins the planning, decides on all financial matters and receives any surplus. (decide-by: T-18m)
- {bdg-primary}`DEFAULT` (basis: L-2020, L-4028, L-4149) **Do you have a full budget at three attendance levels before you commit money?** Include sponsor income, ticket income, all expenses and the Foundation line. Hosting calls from 2015 to 2019 required it (R-004, R-005), and no later statement confirms it. (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-1031, L-3008, L-3096) **How will you cover costs that fall due before income arrives?** Name the bridge before signing: a seed loan, the financial agent, a reserve or a bank facility. Hosting calls required a plan (R-006), and no later statement confirms it. (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-2023, L-4077, L-4900) **What share of registration income goes to the Foundation, and is it in the budget?** Calls from 2015 to 2019 set 15 percent of registration income, not of sponsorship, with one call at 20 percent (R-010). The rate for your year is a question for the Board (see Thin content). (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Which VAT regime applies to your ticket income, and who verified it?** Settle this before you set prices (L-5000). One conference reports the evidence, so this stays an option. A qualified adviser should confirm place of supply and refund rules. (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Will you keep a plain-text budget and ledger from the first ticket sale?** One team paired a budget with a shadow double-entry ledger (L-5014) and kept it from the start of sales (L-5044).
- {bdg-secondary}`OPTION` **Will you apply for outside grants, and keep them out of committed income?** An unanswered request cannot fund a contract (L-5006).

## How-to

1. Build the budget from the Foundation's planning schedule: sponsor and ticket income against shirts, trainer housing, venue, services, catering, optional travel support and the Foundation share (L-4028).
   Done when the budget shows low, expected and high attendance.
1. Open shared budget and accounting books when ticket sales begin (L-5044).
   Done when every commitment signed after that day is booked against the budget.
1. Make repeated cumulative imports idempotent and reconcile balances after each cycle (L-5060).
   Done when a second import changes no balance.
1. Track contracted but uninvoiced obligations in a report-only overlay, apart from statutory balances and VAT reports (L-5061).
   Done when the overlay reconciles with the reserve it assumes.
1. Save or scan every receipt from the first day and reconcile on a fixed rhythm (L-3006).
   Ask vendors for invoices up front (L-3010).
   Done when no vendor invoice is missing a month after the event.
1. Ask each funder for its lead time and file early (L-4039).
   As of 2026-11, the planning schedule names eight weeks before the event for Python Software Foundation and EuroPython funding, and recommends early June for a September event (S004).
   Done when each application is filed and booked as unconfirmed.
1. Publish accounting patterns as sanitized templates with synthetic examples (L-5015).
   Done when a successor can run them without your bank data. See `budget-sheet-template` and `cost-benchmarks`.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S023, S049, S098 | ledger: L-3007, L-4064, L-5008 | confidence: observed | status: active | basis: independent-conferences

Plan cash flow before you commit, because costs fall due before income does.
The largest bills cluster in the final week, and a community that buys late leaves income thin until then.
```

Two single-conference statements stay below the promotion rule.
Seattle held that a host should be paid fairly for its time and should not seek a large profit from the user community (L-1034).
Maastricht treated accounting as a maintained operating instrument, with a plain-text budget and import rules (L-5013).

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S098 | ledger: L-5001 | confidence: observed | status: active

Cross-border VAT questions became a major challenge.
Buyer support needed published refund instructions during the ticket campaign.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S104, S105 | ledger: L-5014, L-5063 | confidence: observed | status: active

A periodic-transaction hledger budget and a shadow ledger supported budget-to-actual and VAT reporting.
Imports were automated, but bank entry and refunds stayed manual.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S098 | ledger: L-5030 | confidence: observed | status: active

Attendance-prediction research supported late-sales decisions.
A reusable version needs a separate, sanitized model description.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5007, L-5043 | confidence: reported | status: active

Tracker status proved weak evidence.
A grant request stayed open without a recorded response, and the budget and invoicing issues closed shortly before the event while the tooling itself had been in place earlier.
```

```{note} [specific · 2023 · Eibar · 3 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2023 | place: Eibar | org: CodeSyntax | source: S070 | ledger: L-4188 | confidence: reported | status: active

The organizing company planned a 10 percent donation to the Foundation, below the 15 percent of registration income in the hosting calls.
```

```{note} [specific · 2018 · Tokyo · 8 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2018 | place: Tokyo | org: Plone Conference 2018 Steering Committee | source: S058, S095 | ledger: L-4148, L-4150 | confidence: observed | status: active

City funding depended on international visitors reaching a minimum number of room nights.
The organizers asked attendees to report accompanying family and friends, because the count helped secure support.
```

```{note} [specific · 2018 · Tokyo · 8 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2018 | place: Tokyo | org: Plone Conference 2018 Steering Committee | source: S095 | ledger: L-4149 | confidence: observed | status: active

The winning bid modeled income, fixed costs and per-person costs at 150, 200 and 250 attendees.
```

```{note} [specific · 2018 · n/a · 8 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2018 | place: n/a | org: Plone Foundation | source: S059 | ledger: L-4900 | confidence: observed | status: active

The 2019 call set the Foundation contribution back to 15 percent of registration income.
```

```{note} [specific · 2015 · n/a · 11 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2015 | place: n/a | org: Plone Foundation | source: S049 | ledger: L-4077 | confidence: observed | status: active

The 2016 call set the contribution at 15 percent of registration income only, collected after the conference, and asked bidders to budget for it.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S093 | ledger: L-3096, L-3097 | confidence: observed | status: active

The association had no cash at the start of the year, and loans from friends paid early costs until sponsorship arrived.
The lead organizer checked a cash-flow spreadsheet against bank and payment-provider statements.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S094 | ledger: L-3117 | confidence: observed | status: active

With free registration and fixed sponsorship, the projected surplus shrank as attendance rose, because each extra attendee added only cost.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S023 | ledger: L-3008 | confidence: observed | status: active

The lead organizer fronted costs on a personal credit card for later reimbursement.
The event was rescued only because the card issuer raised the limit.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S016 | ledger: L-2020, L-2021 | confidence: observed | status: active

The budget used three attendance levels: 400 hoped for, 300 at break-even, capacity for 500.
Estimating attendance was the hardest part and proved wrong, with 285 attending.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S016 | ledger: L-2023 | confidence: observed | status: active

Hosting required the Foundation to receive 15 percent of ticket sales (as of 2010).
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S016 | ledger: L-2026, L-2029 | confidence: observed | status: active

Fixed costs grew by more than half over the bid budget after an unbudgeted keynote and more staging.
The final account showed a small surplus that did not cover the host's staff time.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009, S090 | ledger: L-1031, L-1032 | confidence: observed | status: active

The Foundation lent the host USD 8,000 against a promissory note, repaid shortly after the conference (as of 2006, S009).
The public budget flagged about USD 30,000 of costs as up-front.
The organizers say they would have declined without the loan.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1033 | confidence: observed | status: active

Costs of about USD 63,000 against income of about USD 99,000 left a profit of about USD 36,000 (as of 2006, S009).
The host treated the work as a consulting project and felt fairly paid.
```

## Risks

```{warning} Costs fall due before income arrives
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Name the bridge before signing and model the weekly balance through the final month | owner-role: treasurer | playbook: cash-flow-crunch

Judged for a mid-size conference.
Several teams relied on loans or a personal card.
```

```{warning} An unconfirmed grant is counted as committed income
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Book unconfirmed applications outside committed income until the funder confirms in writing | owner-role: treasurer

An unanswered request cannot fund a contract (L-5006).
```

```{warning} A wrong VAT assumption changes the price
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Have a qualified adviser confirm the regime before prices are published | owner-role: treasurer

A wrong assumption surfaces as refund requests.
```

```{warning} Late ticket sales are read as a revenue shortfall
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Compare sales with a dated forecast before cutting commitments or raising prices | owner-role: treasurer | playbook: low-ticket-sales

Buyers purchase late.
```

```{warning} A payout to a recipient in some countries fails
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Check the payout route for each recipient country before promising reimbursement | owner-role: treasurer

The Foundation reimburses through a service that does not let charities send rupees to residents of India, and bank wires have also failed (L-4053).
```

```{warning} A committed-spend overlay misstates totals
:class: hb-risk hb-likelihood-low hb-impact-medium
risk | likelihood: low | impact: medium | mitigation: Test the assumptions behind the overlay and retire it if other postings break the equivalence with its reserve | owner-role: treasurer

The overlay is report-only (L-5062).
```

## Thin content

```{warning} Foundation share rate and form
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: A Board statement of the standing share of registration income and how it is collected | who-might-know: Foundation Board; Foundation Treasurer

Evidence from 2010 to 2023 shows 15, 20 and 10 percent, and no standing document states the rate for your year (R-010).
```

```{warning} Budget and cash-flow requirements rest on hosting calls
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: A Board confirmation that a full budget and a cash-flow plan are still required in hosting proposals | who-might-know: Foundation Board; Conference Committee

R-004 and R-006 are documented only in hosting calls up to the 2020 call, so they carry no MUST badge.
```

```{warning} University and Foundation VAT treatment
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Verified rules per country on whether a university or the Foundation can sell tickets without VAT | who-might-know: Tax advisers in each host country; Foundation Board | area: jurisdiction-annexes

R-035 and R-036 are open questions, and the debrief reports an exemption that no source has verified.
```

```{warning} Tax outside the EU
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Dated accounts of sales tax and payout rules for hosts outside the EU | who-might-know: Past organizers in the United States, Brazil and Japan | area: non-eu-legal-tax-visa

The handbook holds one cross-border VAT account.
```

```{warning} Budgets for small conferences
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A worked budget for a conference below 150 attendees | who-might-know: Organizers of regional events and sprints | area: small-budget

Located budgets model 150 to 600 attendees.
```

```{warning} Grant funding is unreliable
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second account of grant applications and their outcomes | who-might-know: Past organizers; Python Software Foundation contacts

One conference reports an unanswered grant request.
```

## Sources and further reading

- S004 Plone Foundation, Conference Planning Schedule.
- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
- S016 Bristol 2010, "Plone Conference 2010, The Numbers".
- S023 San Francisco 2011, wiki page on the budget.
- S049 Boston 2016 call for proposals.
- S058 Tokyo 2018, community request for early ticket purchases.
- S059 Ferrara 2019 call for proposals.
- S070 Eibar 2023, Foundation board minutes with the organizer's report.
- S090 Seattle 2006, public conference budget.
- S093 Brasília 2013, PythonBrasil operational record.
- S094 Brasília 2013, conference proposal.
- S095 Tokyo 2018, winning proposal.
- S098 Maastricht 2026, facts and lessons for the handbook.
- S099 Maastricht 2026, GitHub issues and project board review.
- S104 Maastricht 2026, conference accounting overview.
- S105 Maastricht 2026, accounting operator runbook.
