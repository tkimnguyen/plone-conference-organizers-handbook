---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "The risks that span several workstreams of a Plone conference: money timing, key persons, community size, the Foundation relationship and the legal entity."
    "keywords": "Plone, Plone Conference, risks, cash flow, legal entity, continuity"
---

# Cross-cutting risks

Most risks belong to one workstream and live in that chapter's "Risks" section.
The risks on this page do not.
They start in one place, for example the budget model, and do their damage somewhere else, for example in the catering order or in an organizer's private bank account.
Nobody owns them by default, so they are the risks most likely to be noticed late.

Read this page with the whole team at kickoff, as step 8 of [The risk register method](risk-method.md) describes.
Agree on one owner role for each risk before the first contract is signed.
The scores use the scale on that page and assume a typical mid-size conference.
Every risk here also appears in the generated [Risk register](../generated/risk-register.md).

## Money timing

Conference money arrives late and leaves early.
Venue deposits, internet, catering and design are due before most tickets sell, and the largest bills arrive in the final week (L-1032, L-3007).
The Foundation's own call for proposals asked bidders to explain how they would manage this gap (L-4064, R-006).

```{warning} Commitments fall due before matching income arrives
:class: hb-risk hb-likelihood-high hb-impact-high
risk | likelihood: high | impact: high | mitigation: Keep a dated cash view of every committed payment against confirmed income from the first contract onward and agree a bridge, such as an advance or a staged deposit, before signing | owner-role: treasurer | playbook: cash-flow-crunch

This risk is close to certain for a first-time organizer without a financial agent.
The question is not whether a gap opens, but who carries it while it is open.
The full advice is in `finance` and `legal-entity-and-financial-agent`.
```

```{warning} An organizer carries conference costs privately
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Set a written limit on what any individual may front, record every personal advance as a loan with repayment terms, and route payments through the organizing entity | owner-role: conference chair | playbook: cash-flow-crunch

Past organizers fronted costs on personal cards and savings, or borrowed from friends to pay for the first publicity (L-3008, L-3096).
The damage falls on one person and stays invisible to the community unless someone writes it down.
```

## Ticket timing and community size

The Plone community buys tickets late, and its recurring in-person core is smaller than headline attendance figures suggest.
Both facts push a team toward the wrong reaction: panic in the weeks when sales are quiet, or a budget built on a number the community never reached.

```{warning} Normal late purchasing is misread as a demand collapse
:class: hb-risk hb-likelihood-high hb-impact-medium
risk | likelihood: high | impact: medium | mitigation: Agree a dated sales forecast that models late purchasing before tickets go on sale and judge every low-sales alarm against it | owner-role: treasurer | playbook: low-ticket-sales

One conference had sold fewer tickets than its break-even count four weeks before the event, and a late rush carried it past break-even (L-2084).
Another treated organizer anxiety about slow sales as a lesson in itself (L-5008, L-5009).
The wrong reaction is cutting reversible costs too early or committing more money without evidence.
```

```{warning} The attendance plan overstates the community that will travel
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Build the budget on separate estimates for the recurring community and for local or partner audiences, and set break-even on the community estimate alone | owner-role: treasurer | playbook: low-ticket-sales

Bids planned for 700 and for 200 participants; the history pages later report just over 400 and around 150 (L-4089, L-4142).
The two largest in-person editions were co-hosted with a regional Python conference, so total attendance does not measure the community (L-4021, L-5010).
One debrief puts the recurring in-person community at roughly a hundred people; that figure is an unverified estimate (L-5011).
Three-scenario budgets at hoped-for, break-even and capacity levels are the established response (L-2020, L-4149).
```

## Key persons

Small volunteer teams concentrate knowledge and access in a few people.
When one of them is ill, exhausted or leaves, whole workstreams stop.

```{warning} A key person becomes unavailable and has no deputy
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Name a deputy for every role with a risk score of 3 or more, and have the deputy shadow the role and hold its accesses before T-2m | owner-role: conference chair | playbook: key-person-loss

The person responsible for one conference's Wi-Fi was hospitalized two weeks before the event, and there was no backup plan (L-3075).
Another team found that one person owning daytime operations and a late social event left no recovery time (L-5054).
The full advice is in `team-and-governance` and `volunteers-and-roles`.
```

```{warning} Accounts and credentials are held by one person
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Keep every conference account, domain and payment login in a shared password manager or with the Foundation, with at least two holders | owner-role: conference chair | playbook: key-person-loss

The handover contract already requires an asset and credential list at the end of each conference, as described in [The annual ritual](../running/annual-ritual.md).
The same list is the protection during the conference year.
```

## The Foundation relationship

The Plone Foundation approves the conference and may act as its financial agent.
Several Foundation terms are written only in past calls for proposals, and some cannot be confirmed in a standing document as of 2026-11-02.
A team that assumes support exists, or assumes it does not, can be wrong in either direction.

```{warning} The team relies on Foundation support that was never confirmed
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Ask the Foundation in writing at kickoff whether it offers an advance or acts as financial agent, and keep every unconfirmed grant or support request outside committed income | owner-role: Foundation liaison | playbook: cash-flow-crunch

The Foundation once lent the host money against a promissory note, and the organizers said they would otherwise have declined to host (L-1031).
Whether such advances are still offered is an open question in the requirements register (R-037).
A grant request left unanswered cannot fund a contract (L-5006, L-5007).
```

```{warning} Organizer work hours are assumed to be covered
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Budget organizer time as an explicit cost carried by named organizations and agree it inside the team before the bid | owner-role: conference chair

Under the financial-agent model the Foundation covers losses but not the organizers' extra work hours (L-4059, R-008).
One host's published final account covered every external cost but not its own staff time (L-2029).
```

## The legal entity

The entity that signs contracts and sells tickets decides who carries losses, which VAT regime applies and which bank account receives the money.
These decisions touch finance, ticketing, contracts and privacy at once.

```{warning} The selling entity is chosen after prices are published
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Decide the contracting and ticket-selling entity and have a qualified adviser confirm its VAT treatment before ticket prices are published | owner-role: treasurer

Cross-border VAT became a major organizing challenge in one recent edition and needed published refund instructions for buyers (L-5000, L-5001).
The final price a participant pays depends on which entity sells the ticket (L-5002).
The full advice is in `legal-entity-and-financial-agent`, `finance` and `ticketing-and-registration`.
```

```{warning} Organizers carry losses on their own accounts
:class: hb-risk hb-likelihood-low hb-impact-high
risk | likelihood: low | impact: high | mitigation: Decide in the bid whether to request the Foundation as financial agent, and if not, name the entity that carries losses and check its liability limits | owner-role: conference chair | playbook: cash-flow-crunch

Most past conferences ran on the organizers' own bank accounts, credit and accounting, and the organizers carried the full risk of losses (L-4056).
The financial-agent option trades that risk for board oversight and the surplus (L-4058).
```

## Unwritten expectations and open checks

Some obligations are never written down, and some required checks stay open until the conference is over.
Both surface late, in a workstream that did not budget for them.

```{warning} An unwritten community expectation becomes an unbudgeted obligation
:class: hb-risk hb-likelihood-high hb-impact-medium
risk | likelihood: high | impact: medium | mitigation: List the community's expectations at kickoff with the Conference Committee and decide each one explicitly, with its cost, before the related offer is published | owner-role: conference chair

One debrief names conference-funded trainer accommodation as an implicit expectation and the largest financial risk of that year (L-5019, L-5020).
The full advice is in `community-and-speaker-expectations`.
```

```{warning} A required check stays open with no decision gate
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Turn each required check, such as insurance due diligence, into a gate with an owner and a date, and record a drop decision in the Tailoring Record if it is skipped | owner-role: conference chair | playbook: force-majeure

One review found the venue-insurance due diligence never completed; an open issue was not a decision gate (L-5034, L-5038).
The full advice is in `contracts-legal-insurance` and `team-and-governance`.
```

## Continuity between editions

Each edition starts with a team that has not run a Plone conference before.
What the previous team knew is lost unless it is handed over.

```{warning} The previous team's knowledge does not reach the next team
:class: hb-risk hb-likelihood-high hb-impact-medium
risk | likelihood: high | impact: medium | mitigation: Hold the handover deliverables to their dates in the annual ritual and have the incoming team shadow the outgoing team's final months | owner-role: conference chair

One working budget lived in a spreadsheet whose history successors could not see (L-2025).
The Foundation's own archive page stopped listing editions after 2015 (L-4020).
The Conference Committee exists to carry this continuity (L-4023).
The full advice is in `handover-contract`.
```

## Sources

- S001 Plone Foundation conference archive page.
- S002 Plone conference history page.
- S003 Conference Committee team page.
- S009 Seattle 2006 lessons learned.
- S010 Naples 2007 conference record, including the bid.
- S016 Bristol 2010 published numbers.
- S023 San Francisco 2011 budget wiki page.
- S034 Interview with the 2011 lead organizer.
- S036 Arnhem 2012 organizer wrap-up.
- S049 2016 call for proposals.
- S057 Tokyo 2018 sponsor prospectus.
- S090 Seattle 2006 public budget.
- S091 Plone Event Financial Policy.
- S093 Brasília 2013 operational record.
- S095 Tokyo 2018 winning proposal.
- S098 Maastricht 2026 facts and lessons.
- S099 Maastricht 2026 collaboration review.
- S101 Maastricht 2026 on-site roles.
