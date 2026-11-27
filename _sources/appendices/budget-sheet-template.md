---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "A copyable budget sheet skeleton for a Plone conference: unavoidable and optional costs, fixed and per-person costs, attendance levels and cash-flow timing."
    "keywords": "Plone, Plone Conference, budget, budget sheet, cash flow, template"
---

# Template: budget sheet

Copy the table skeletons below into a spreadsheet or a plain-text ledger, and fill in the placeholders in angle brackets.
The sheet has no amounts on purpose: every figure comes from your own quotes, and a figure from this handbook is a dated example, never a rule.
The decisions behind the sheet are in [Finance](../workstreams/money-and-law/finance.md), and the cost context is in [Cost benchmarks](../evidence/cost-benchmarks.md).

## What the sheet must do

The Foundation's planning schedule asks organizers to develop and track a budget with sponsor income, ticket income and expenses, including a Plone Foundation line (R-005, verified-current as of 2026-11-02, guidance and not a hard requirement).
The sheet below meets that ask and adds four things that past teams wished they had.

1. Costs are split into unavoidable and optional, so cuts can be made without touching the core event (L-1035).
2. Costs are split into fixed and per-person, so each attendance level has its own result (L-3118).
3. Every line has a due date, so the sheet shows how much cash you need before income arrives (L-1032).
4. The sheet is one file with revision history that successors can read (L-2025).

## Structure choices

### Unavoidable and optional

Seattle's sheet separated unavoidable expenses from optional ones.
Unavoidable lines were venue, internet, catering, supplies, name tags, cables, banners, screens, microphones, a logo, registration fees, the sprint and tutorial honoraria.
Optional lines were video, t-shirts, a brochure and press checks (L-1035).
The same sheet showed which single unavoidable line dominated and which optional line was largest, which told the team where cuts would matter (L-1036; see [Cost benchmarks](../evidence/cost-benchmarks.md)).
Mark every line in your sheet with one of the two labels, and agree the optional lines with the team before you commit to them.

### Fixed and per-person

The Brasília bid separated fixed costs from per-person costs.
Fixed costs were venue, keynote, network, office supplies, AV, video, translation, signage, transport and the Foundation fee.
Per-person costs were badge, t-shirt, bag, gift and food (L-3118).
The split matters because the result moves with attendance.
Under free registration and fixed sponsor income, the projected surplus shrank as attendance rose, because every extra attendee only added per-person cost (L-3117).
Payment-processor fees are per-person costs too, and made up about one sixth of per-person costs at one conference (L-2030).

### Three attendance levels

Build the sheet at three attendance levels: the number you hope for, the break-even number, and the number you can cope with.
Bristol used a hoped-for level, a break-even level and a capacity level (L-2020).
Estimating attendance was the hardest part, and the estimate turned out wrong (L-2021).
Break-even attendance is the fixed costs divided by the net ticket income per attendee after the per-person costs and the Foundation share.
Compute it in the sheet and do not carry it in your head.

### Income lines

- Ticket income by ticket type, net of payment-processor fees.
  Include complimentary tickets and discounted tiers in the counts, because they were underestimated at more than one conference (L-3012, L-5023).
- A funded reduced-price route for participants who could not otherwise come, if you offer one (L-5003).
- Sponsor income at a low and an expected level, with in-kind support listed separately and not counted as cash (L-3119).
- Grants only when signed.
  An unanswered request is not income (see [Finance](../workstreams/money-and-law/finance.md)).
- Earmarked funds carried from the previous edition, with the purpose noted (L-3022).

### The Foundation line

Put a Plone Foundation line in the cost side from the first draft (R-005).
The base and the rate depend on your year and on whether the Foundation acts as financial agent.
One hosting call set the share at 15 percent of registration income only, not of sponsorship, collected after the conference (L-4077).
Ask the Board for the rule that applies to you, and record the answer with its date in the sheet.

### Cash-flow timing

A host that cannot advance costs before income arrives needs a bridge.
Seattle's seed loan was far smaller than its up-front costs, which were room rental, internet, catering, supplies, equipment rental and a logo (L-1031, L-1032).
A later host in Brasília bridged early costs with loans from friends until the first sponsor payment arrived, and tracked income and expenses in a cash-flow spreadsheet checked often against the bank and the payment-provider statements (L-3096, L-3097).
Community members tend to buy tickets late, so judge sales against a late-buying forecast before treating a slow start as a shortfall (L-5008).
Each line therefore carries a due month and an expected payment month, and the sheet totals cash by month.

## Cost lines skeleton

Copy the block into a spreadsheet.
Labels: U unavoidable or O optional; F fixed or P per person.
Amounts for levels A, B and C are your three attendance levels, computed from the basis column.

```text
COST LINES: <Conference name and year>   Version: <vN>   Date: YYYY-MM-DD

| Line | Group | U/O | F/P | Basis (quote, rate, unit) | Level A | Level B | Level C | Due month | Paid by | Status |
|---|---|---|---|---|---|---|---|---|---|---|
| Venue and rooms | Venue | U | F | <quote id> | | | | T-<n>m | | |
| Internet and network | Venue | U | F | <quote id> | | | | | | |
| Catering | Venue | U | P | <rate x attendees> | | | | | | |
| Audio, video and streaming | AV | O | F | <quote id> | | | | | | |
| Screens and microphones | AV | U | F | <quote id> | | | | | | |
| Signage and banners | Print | U | F | <quote id> | | | | | | |
| Badges and lanyards | Print | U | P | <rate x attendees> | | | | | | |
| T-shirts | Merch | O | P | <rate x attendees> | | | | | | |
| Bags and gifts | Merch | O | P | <rate x attendees> | | | | | | |
| Program printing | Print | O | F | <quote id> | | | | | | |
| Keynote and invited speakers | Program | O | F | <agreement id> | | | | | | |
| Speaker tickets and discounts | Program | U | P | <share x price> | | | | | | |
| Trainer accommodation | Program | U | F | <agreement id> | | | | | | |
| Sprint space and supplies | Program | U | F | <quote id> | | | | | | |
| Party or social event | Social | O | F | <quote id> | | | | | | |
| Travel and access support | People | O | F | <fund size> | | | | | | |
| Accessibility measures | People | U | F | <quote id> | | | | | | |
| Insurance | Admin | U | F | <quote id> | | | | | | |
| Payment-processor fees | Admin | U | P | <rate x tickets> | | | | | | |
| Accounting and tax advice | Admin | U | F | <quote id> | | | | | | |
| Domain, website and tools | Admin | U | F | <quote id> | | | | | | |
| Plone Foundation share | Foundation | U | F | <rate x base, dated rule> | | | | | | |
| Contingency | Admin | U | F | <percentage of total> | | | | | | |
| TOTAL | | | | | | | | | | |
```

## Income lines skeleton

```text
INCOME LINES: <Conference name and year>

| Line | Basis (price, count, rate) | Level A | Level B | Level C | Expected month | Confidence | Status |
|---|---|---|---|---|---|---|---|
| Regular tickets | <price x count> | | | | | | |
| Early-bird tickets | <price x count> | | | | | | |
| Student and reduced tickets | <price x count> | | | | | | |
| Speaker tickets | <price x count> | | | | | | |
| Complimentary tickets (cost side shows the matching cost) | <count> | | | | | | |
| Funded access tickets | <fund size> | | | | | | |
| Sponsor tier 1 | <amount x count> | | | | | | |
| Sponsor tier 2 | <amount x count> | | | | | | |
| Sponsor tier 3 | <amount x count> | | | | | | |
| Public-body or in-kind support (listed apart from cash) | <value> | | | | | | |
| Grants (signed only) | <agreement id> | | | | | | |
| Carried earmarked funds | <purpose> | | | | | | |
| TOTAL CASH INCOME | | | | | | | |
```

## Result and break-even block

```text
RESULT

| Row | Level A | Level B | Level C |
|---|---|---|---|
| Attendees (paying, speaker, complimentary) | | | |
| Total cash income | | | |
| Total fixed costs | | | |
| Total per-person costs | | | |
| Total costs | | | |
| Result before Foundation share | | | |
| Result after Foundation share | | | |
| Break-even attendance | | | |
| Unavoidable costs only: result | | | |
```

The last row answers the question every team asks in a bad month: can we still hold the core event if we cut every optional line.

## Cash-flow grid

Use one column per month from T-12m, the month you could first owe money, to T+3m, after the event.
Copy the block and add one column per month.

```text
CASH FLOW

| Row | T-12m | T-9m | T-6m | T-3m | T-1m | Event month | T+1m | T+3m |
|---|---|---|---|---|---|---|---|---|
| Opening cash | | | | | | | | |
| Income received | | | | | | | | |
| Costs paid | | | | | | | | |
| Closing cash | | | | | | | | |
| Bridge drawn (seed loan, agent, reserve) | | | | | | | | |
| Bridge repaid | | | | | | | | |
| Lowest closing cash and its month | | | | | | | | |
```

The lowest closing cash is the size of the bridge you need, and the month shows when you need it.
If the bridge is smaller than that figure, change the plan before you sign the first large contract.
The [cash-flow crunch playbook](../risk/playbooks/cash-flow-crunch.md) covers what to do when the grid goes negative.

## Publishing the budget

Publish the budget and the final figures, with the staff hours, as aggregates (L-1037, L-2031).
Strip vendor names and private details before publishing, and keep a dated copy with the post-mortem (see [Template: post-mortem](post-mortem-template.md)).
A plain-text budget with import rules helped one team keep the forecast aligned with actual transactions through the campaign (L-5013).

## Related

- [Template: sponsor prospectus](sponsor-prospectus-template.md) for the income side.
- [Finance](../workstreams/money-and-law/finance.md) for the decisions and the Foundation share.
