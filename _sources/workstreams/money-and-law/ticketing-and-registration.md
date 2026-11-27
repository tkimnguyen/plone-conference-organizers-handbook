---
steward: unassigned
deputy: unassigned
review-by: 2027-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to choose a ticketing platform, set prices and tiers, handle VAT and collect the data a Plone conference needs from every attendee."
    "keywords": "Plone, Plone Conference, ticketing, registration, pricing, VAT, tickets"
---

# Ticketing and registration

## Why it matters

Registration is where income, attendee data and the first impression meet.
A platform that fails at the busiest moment costs sales, and a price set by guesswork can cost the break-even point.
Missing per-attendee data surfaces later as lost shirt sizes, dietary needs and unreachable attendees.

The choices reach beyond the registration desk.
The selling entity decides the VAT regime, the platform decides the fees and the refund options, and the tiers decide who can afford to come.
Participants in this community buy late and often ask for group or reduced prices.

The steps are in the How-to section.
Budget questions sit in `finance`.

## Applies when

- `all` Every Plone conference sells or issues tickets, including free and online editions.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-1048, L-3017) **Will you buy a ticketing service instead of building one?** Both teams used a vendor service and kept registration simple. Choose one with a usable API. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Which entity sells the tickets, judged by the final price for a buyer who cannot recover VAT?** The debrief's university exemption and Foundation assumptions need jurisdiction-specific confirmation (L-5002, R-035, R-036). (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Which platform and payment methods, compared after fees?** Count platform fees against net revenue (L-5016). A self-hosted pretix with invoice or bank transfer may suit a community event, if you weigh operating effort and payment access first (L-5018). (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will you publish a no-refund, no-transfer policy?** The 2011 organizer kept it, with a few transfers for extreme cases at discretion, because an open policy could get out of control (L-3016). (decide-by: T-6m)
- {bdg-danger}`MUST` (req: R-013; as-of: 2026-11-02) **Do buyers agree to abide by the Plone Code of Conduct at purchase?** Publish the code on the website as well (L-4037). (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Will the ticket flow collect an agreement to be photographed?** The Foundation's planning schedule lists it (R-014, S004). Legal sufficiency is a question for counsel, see `privacy-gdpr`. (decide-by: T-6m)
- {bdg-primary}`DEFAULT` (basis: L-1043, L-6037) **Will you ask prospective attendees what they would pay?** Seattle surveyed willingness to pay before setting the price, and Maastricht found that price perception was a blind spot. (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-1044, L-2058, L-4145) **Which tiers will you offer?** Early bird closing at a fixed date, regular, speaker and one-day tickets were all used. State each tier's end date on the site. (decide-by: T-6m)
- {bdg-primary}`DEFAULT` (basis: L-1047, L-3012) **Have you budgeted complimentary and speaker tickets explicitly?** One conference gave away about a fifth of its tickets, and another grossly underestimated the number. (decide-by: T-6m)
- {bdg-primary}`DEFAULT` (basis: L-4067, L-5003) **Will you fund a reduced-price route?** Affordability is a key issue for students and the self-employed, and one conference funded a Global South route as an access budget. Hosting calls from 2015 to 2019 set a target of USD 250 to 450 per person (R-011). (decide-by: T-9m)

## How-to

1. Write the requirements: one buyer registers several people with full details for each, people register on behalf of others, international addresses work, prices tier by date and unlock by code, and add-ons such as trainings are sold (L-1050).
   Done when each is tested on the chosen platform.
1. Support institutions: an invoice, card payment outside the web form, and payment by check or bank transfer (L-1051).
   Done when a test invoice is issued without manual work.
1. Collect an e-mail address for every attendee, not only the buyer (L-3018).
   Done when a multi-ticket test order produces one address per person.
1. Offer a group discount and advertise it (L-3015), since groups of more than six come more motivated (L-3080).
   Done when the discount appears on the ticket page.
1. Put the Code of Conduct and the photo agreement into the purchase flow (L-4037).
   Done when a test purchase cannot finish without both.
1. Keep sales open until very late, especially when the venue is easy to reach from Europe (L-4045).
   Done when the closing date is tied to the dates at which food and shirt counts are due.
1. Publish refund and VAT instructions before the campaign starts, and compare weekly sales with a dated forecast.
   Done when support questions point to one page. See `low-ticket-sales` if sales fall behind.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009 | ledger: L-1048 | confidence: reported | status: active | basis: structural | reason: Registration handles money and personal data, and a custom system must be maintained by a volunteer team that changes every year.

Do not write custom registration software, and keep the process as simple as possible.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S088 | ledger: L-1052 | confidence: observed | status: active | basis: structural | reason: A ticket is often paid by an employer or administrator, so payer and attendee differ and both need records.

Record the attendee apart from the payer, and send receipts to everyone, so the desk and the badge show the attendee.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S036 | ledger: L-2080 | confidence: observed | status: active | basis: structural | reason: Registration depends on third-party payment services the team does not control, so any of them can fail at the busiest moment.

Have a backup plan for registration and payment problems.
```

Four themes stay below the promotion rule.
Price setting is hard: San Francisco advised raising the price a bit if in doubt (L-3004) and called guessing 100 percent voodoo (L-3011).
Buyers purchase late: Arnhem asked for ways to make people buy earlier (L-2103), and the Foundation's planning schedule says people buy even very late (L-4044).
Affordability and access matter (L-4067, L-5003).
Seattle recommended a published one-day rate, with one-day attendees marked on badges (L-1046).

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S082 | ledger: L-4227 | confidence: observed | status: active

The Business Track ticket cost 180 euros including 21 percent Dutch VAT, and a Friday one-day ticket at the same price included it (as of 2026-09).
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S098 | ledger: L-5017 | confidence: observed | status: active

The fee is verified: 2.89 EUR per ticket paid via Stripe, as of 2026-11.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6036, L-6037, L-6048 | confidence: reported | status: active

Value for money averaged 4.30 on 20 ratings, and nobody mentioned the ticket price.
The analyst's first reading, that venue cost drove low scores, was contradicted.
One respondent asked for earlier website, advertising and ticket sales.
```

```{note} [specific · 2020 · Online · 6 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2020 | place: Online | org: Plone Foundation | source: S063 | ledger: L-4166 | confidence: observed | status: active

The online edition's early-bird window lasted one week, and regular registration ran until the day before the start.
```

```{note} [specific · 2019 · Ferrara · 7 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2019 | place: Ferrara | org: RedTurtle | source: S060 | ledger: L-4159 | confidence: observed | status: active

One full pass covered training, conference, lunches, party and sprints at 380 euros plus fee and VAT, and a one-day pass cost 150 euros (as of 2019).
```

```{note} [specific · 2018 · Tokyo · 8 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2018 | place: Tokyo | org: Plone Conference 2018 Steering Committee | source: S057, S058 | ledger: L-4145, L-4146, L-4147 | confidence: observed | status: active

The range included a one-day ticket without dinner.
Four weeks out, the organizers asked everyone who already planned to come to buy early, because shirts and food needed numbers.
Multi-ticket orders arrived only late in the sales period.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S042, S093 | ledger: L-3094, L-3131 | confidence: observed | status: active

Free registration fell through when the venue agreement could not be kept.
Registration opened at a symbolic fee, with student and member rates rising by date, and one registration covered both co-located events.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2079, L-2084 | confidence: observed | status: active

Payments failed at the switch from early-bird to regular price, and e-mail requests were hard to track.
Break-even was 220 tickets, 194 were sold four weeks out, and a late rush reached 250.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S024 | ledger: L-3012, L-3014 | confidence: observed | status: active

The team set the budget first, worked back to a price and grossly underestimated complimentary tickets.
Setting the speaker rate equal to the early-bird rate left no refunds to manage.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S024 | ledger: L-3017, L-3020, L-3021 | confidence: observed | status: active

The team chose the cheapest of three services with a usable API, and a chat bot reported live sales from it.
Organizers could not process transfers or refunds, so each took a call to the vendor.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S024, S034 | ledger: L-3019, L-3082 | confidence: observed | status: active

Group orders asked questions such as shirt size once per order, and ticketing was not integrated with marketing.
The team held only a partial attendee e-mail list.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S016, S019 | ledger: L-2030, L-2058 | confidence: observed | status: active

Processor fees made up about one sixth of per-person costs.
The bid committed to a ceiling on the registration fee and an early-bird reduction about two months ahead.
```

```{note} [specific · 2009 · Budapest · 17 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2009 | place: Budapest | org: Greenfinity | source: S013 | ledger: L-4102 | confidence: reported | status: active

Registration cost 150 euros early bird and 200 euros full price, below earlier years, because regional prices ran lower (as of 2009-10).
```

```{note} [specific · 2007 · Naples · 19 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2007 | place: Naples | org: Abstract Open Solutions | source: S010 | ledger: L-4090 | confidence: observed | status: active

The bid priced registration at 300 to 350 euros, covering sessions, a venue shuttle, two coffee breaks and lunch each day (as of the 2006 bid).
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009, S085 | ledger: L-1043, L-1044 | confidence: observed | status: active

A May 2006 survey asked the most people would pay, and 43 percent chose USD 300 (as of 2006, S085).
Pricing followed: USD 300 regular and USD 250 early bird, closing eight weeks out.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009, S090 | ledger: L-1045, L-1047 | confidence: observed | status: active

No student or nonprofit discounts were offered, to keep registration simple.
Of 337 attendees, 68 held complimentary registrations, 44 of them speakers.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1049 | confidence: observed | status: active

The organizers chose a small local ticketing company for its low price and accountability, accepting fewer features.
```

## Risks

```{warning} The payment system fails at the price switch
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Test the switch between tiers with a real purchase before opening and keep a backup way to take orders | owner-role: registration lead

Judged for a mid-size conference.
```

```{warning} Sales stay below break-even
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Track weekly sales against a dated forecast and set decision points before cutting costs | owner-role: registration lead | playbook: low-ticket-sales

Late buying can hide or mimic a shortfall.
```

```{warning} Complimentary tickets are underestimated
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Count sponsor, speaker, volunteer and contest tickets in the budget from the first version | owner-role: treasurer

Free tickets cut revenue without appearing in sales numbers.
```

```{warning} Per-attendee data is lost in group orders
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Test a multi-ticket order and confirm that every attendee answers every question | owner-role: registration lead

Missing answers show up on site as shirt sizes and dietary needs nobody recorded.
```

## Thin content

```{warning} Pricing elasticity
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Sales data by price and tier from several conferences, to show how price changes attendance | who-might-know: Past registration leads; Foundation Treasurer | area: pricing-elasticity

No source measures the effect of price on sales.
```

```{warning} Selling entity and VAT
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Verified answers on whether a university or the Foundation can sell tickets without VAT, per country | who-might-know: Foundation Board; tax advisers in host countries | area: jurisdiction-annexes

R-035 and R-036 are pending Foundation questions.
```

```{warning} Platform fees are unverified
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Dated published tariffs for the platforms organizers use, with a net-revenue comparison | who-might-know: Treasurers of past conferences; platform vendors

The only account is a hearsay debrief note.
```

```{warning} Price target
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: A current statement of the affordability target in USD per person | who-might-know: Foundation Board; Conference Committee

The USD 250 to 450 band dates from hosting calls of 2015 to 2019 (R-011).
```

```{warning} Online and hybrid ticketing
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second account of tiers and registration windows for online or hybrid editions | who-might-know: Organizers of online and hybrid editions | area: hybrid-online

One online edition is recorded.
```

## Sources and further reading

- S004 Plone Foundation, Conference Planning Schedule.
- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
- S010 Naples 2007 conference record.
- S013 Budapest 2009 announcement and context.
- S016 Bristol 2010, "Plone Conference 2010, The Numbers".
- S019 Bristol 2010 conference record and proposal.
- S024 San Francisco 2011, wiki page on tickets.
- S034 San Francisco 2011, organizer interview.
- S036 Arnhem 2012, organizer wrap-up.
- S042 Brasília 2013, contemporary conference report.
- S057 Tokyo 2018 sponsorship program and ticket range.
- S058 Tokyo 2018, request for early ticket purchases.
- S060 Ferrara 2019 conference site.
- S063 Online 2020 post-event record.
- S082 Maastricht 2026 post-conference home page.
- S085 Seattle 2006 pre-conference survey.
- S088 Seattle 2006 logistics suggestions.
- S090 Seattle 2006 public conference budget.
- S093 Brasília 2013, PythonBrasil operational record.
- S098 Maastricht 2026, facts and lessons for the handbook.
- S110 Maastricht 2026 attendee survey analysis.
