---
steward: unassigned
deputy: unassigned
review-by: 2027-05-02
maturity: draft
applies-to: ["size=small", "jurisdiction=NL", "organizer=company", "venue=hotel", "format=in-person"]
diataxis: experience-report
myst:
  html_meta:
    "description lang=en": "Draft case file for Plone Conference 2026 in Maastricht: what was planned, what happened, and what the organizers learned."
    "keywords": "Plone, Plone Conference, Maastricht, 2026, case file, post-mortem"
---

# Plone Conference 2026, Maastricht: case file

> **Draft, pending team sign-off.**
> Under decision D9 this page stays marked draft until the 2026 organizing team confirms its voice and its facts.
> Text may change in version 1.1.
> Facts flagged as reported, hearsay or pending verification below are not yet advice.

## Purpose of this document

This is the capstone record of Plone Conference 2026.
It follows the skeleton of the Seattle 2006 account "Things We Learned About Running a Plone Conference", the one early conference that wrote its lessons down.
It feeds the handbook chapters, whose lessons point back to the evidence ledger rows cited here.
It is also the post-mortem deliverable of the 2026 team, still in draft.
Every claim cites a ledger row (L-5000 to L-5068, and L-6001 to L-6053 for the attendee survey) or a source (S098 to S110), and every row passed the D7 privacy screen.

## Overview

- Dates: 2026-09-21 to 2026-09-27, in Maastricht, the Netherlands.
- Schedule: trainings on Monday and Tuesday, a developer conference from Wednesday to Friday, a Business Track in parallel on Friday, and community sprints on Saturday and Sunday.
- Main venue: a conference hotel in Maastricht with three conference rooms, one of them an auditorium.
- Organizing entity: a volunteer-supported team led by a company-based organizer whose tax home differed from the event's country (F1, L-5000).
- Tickets: 117, of which 5 were party-only (S098, F14). This is the conference's own public-facing aggregate.
- Business Track: eight voices, meaning one keynote, seven practitioner talks of 25 minutes each, and a closing conversation.
- Party: Thursday evening at Muziekgieterij, with a community DJ. Friday evening stayed deliberately empty (L-5022).

## What was planned and what happened

The team planned in a public issue tracker with a project board.
A retrospective analysis on 2026-11-02, five weeks after the conference, found 110 issues, 58 closed and 52 open (S099).
The board held only 30 items, so about 80 issues never reached it, and no milestones were used.
The board was therefore never the operational truth it was meant to be (L-5031).
The analysis drew four lessons.
Each rests on a cluster of issues.

### L1: nobody maintains the tracker in the last six weeks

Cluster A holds work that demonstrably happened but stayed open, among them the party, the goodie bag, the sprint organization and session recording.
Open state could not tell unfinished work from missing closure (L-5033).
The recommended fix is closing as you go and a weekly triage through the final phase (L-5032).

### L2: the drops cluster in four places

Cluster B holds work that was genuinely dropped: legal and insurance, accessibility, local audience development and research beyond team capacity.
The venue-insurance due diligence was never completed (L-5034).
The venue-accessibility task was dropped and no accessibility information reached the website (L-5035).
University outreach was never executed (L-5036).
A decision-maker research program reached written scripts and stopped there (L-5037).
The fix is to track required checks as completion gates and to give optional work an owner and a drop-by date (L-5038).
The team's own documentation tooling ambition never started, and a folder of Markdown files became the archive instead (L-5039, L-5040).

### L3: one level of hierarchy too many

The team created an epic layer and abandoned it, while real work continued in small focused issues (L-5041).
For a small team, a flat list with clear titles and regular triage is the cheaper default (L-5042).

### L4: reuse, tooling visibility and external dependencies

The shared budget and sponsor-invoicing issues closed on 2026-09-10, eleven days before the conference, but that is tracker hygiene, not a work date: budgeting and accounting were in place earlier, and the closure dates misled the first pass of this review (L-5043, corrected 2026-11-02).
Budgeting and accounting belong at the start of ticket sales (L-5044).
Reuse of the conference website tooling, and of content that recurs every edition, can be increased; dependency on external deployments was a factor in delays (L-5069).
The last-phase plan did set program, numbers and print-and-order freezes on 2026-09-04, 2026-09-07 and 2026-09-11, and they worked as a model (L-5047, S100).

Beyond the four lessons, the organizer's retrospective adds the framing that ties the drops together.
Started initiatives such as university outreach, decision-maker research and contact to local industry drowned in a large number of surprises that a manual like this handbook could have prevented, and the improvisation the surprises forced made planning obsolete (L-5073).
Many participants and sponsors decided on their attendance only weeks or days before the conference, a major source of planning risk that also gated the production of material (L-5070).
And knowing whether the budget held gated a chain of decisions, from cross-financing global south tickets to extra equipment and keynote speakers (L-5071).

## The fifteen debrief facts

The organizers' debrief of 2026-11-02 produced fifteen facts (S098).
Each is summarized with its confidence as the ledger records it.

**F1, cross-border VAT.**
Organizing in the Netherlands from a company in another tax jurisdiction made VAT a top-level challenge, and buyer refund questions needed public instructions during the campaign.
The consequences of organizing in another country were underestimated, and unexpected tax issues cost a lot of time (L-5074).
The exact place-of-supply and refund rules are not verified here.
Confidence: observed. Ledger: L-5000, L-5001, L-5074.

**F2, who sells the ticket.**
The selling entity changes the price a participant who cannot reclaim VAT pays.
The debrief reported that a university organizer sometimes charges no VAT, and that Foundation-sold tickets carry no EU VAT.
**Pending verification:** the university claim and current Foundation practice, tracked as requirements-register candidates R35 and R36 (S106).
Confidence: reported. Ledger: L-5002.

**F3, Global South tickets.**
Maastricht introduced Global South pricing and pursued dedicated grant support, as two separate tasks.
Confidence: observed. Ledger: L-5003, L-5004.

**F4, reusable grant argumentation.**
The application for ticket-access funding is reusable once its economics are replaced with synthetic ones.
It explained the subsidy per place and described eligibility and independent review (S109).
The final plan records that it was abandoned after no response (S100).
Confidence: observed. Ledger: L-5005, L-5067, L-5068.

**F5, funding can go wrong.**
A community grant request stayed open with no recorded response.
Unconfirmed grants stay out of committed income.
Confidence: observed for the principle, reported for the case. Ledger: L-5006, L-5007.

**F6, late purchases.**
The community buys late, which strains cash flow and organizer nerves.
A dated forecast separates normal late buying from a shortfall.
Confidence: observed. Ledger: L-5008, L-5009.

**F7, honest community size.**
The debrief described the recurring in-person community as roughly a hundred people and possibly shrinking.
It attributed extra audiences at earlier editions to a joint event and reduced-price local tickets.
**Pending verification:** both statements need comparable per-edition data.
Planned university outreach in 2026 was never executed (L-5036).
Confidence: observed for the planning principle, hearsay for the figures. Ledger: L-5010, L-5011, L-5012.

**F8, reusable accounting.**
A plain-text budget with periodic transactions, a shadow double-entry ledger and import rules worked, and was reconciled to actuals (S104, S105).
It kept manual boundaries for bank entry and refunds, and a committed-spend overlay whose assumptions need testing.
It needs a sanitized rewrite before reuse.
Confidence: observed. Ledger: L-5013, L-5014, L-5015, L-5060, L-5061, L-5062, L-5063.

**F9, the platform fee.**
The ticket platform's fee is a real line item.
Verified by the organizer on 2026-11-02: the conference paid 2.89 EUR per ticket that was paid via Stripe.
A self-hosted alternative with invoice payment was proposed, not evaluated.
Confidence: observed. Ledger: L-5016, L-5017, L-5018.

**F10, expectations never written down.**
Trainer accommodation paid by the conference was an implicit expectation and the debrief's largest financial risk.
Trainer compensation was unregulated.
Nobody is entitled to a party, yet the community values one.
Speaker discounts belong in the pricing model from day one, because speakers form a large minority of participants.
Verified on 2026-11-02 against the conference website: 56 listed presenters against 117 tickets, about 48 percent (L-5075).
Confidence: observed. Ledger: L-5019, L-5020, L-5021, L-5022, L-5023, L-5024, L-5075.

**F11, recording is real work.**
Recording needs its own workstream and owner.
Recordings were made while the related issues stayed open.
Recording equipment was purchased for the conference and is likely not being reused afterwards (L-5072).
Confidence: observed. Ledger: L-5025, L-5049, L-5072.

**F12, the annual meeting slot.**
The debrief said the Foundation's annual meeting needs more than a 25-minute slot and should be streamed.
The organizer confirmed this for the 2026 edition on 2026-11-02; the general rule still awaits Foundation confirmation as register row R-034 (L-5076).
Confidence: observed for 2026. Ledger: L-5026, L-5076.

**F13, PeerTube and the streaming tradeoff.**
PeerTube worked well for live access by people outside the venue.
Streaming might keep some people from attending in person, which is a possibility without measured effect.
Confidence: observed for the tooling, hearsay for the tradeoff. Ledger: L-5027, L-5028.

**F14, ticket prediction.**
Ticket-purchase prediction research should be preserved as a rerunnable method with synthetic inputs.
The implementation separates daytime attendance from other categories and needs its edition-specific configuration replaced (S108).
Confidence: observed. Ledger: L-5029, L-5030, L-5066.

**F15, issues and a board as method.**
The method is worth keeping with three preconditions: close-as-you-go hygiene, one board holding all work, and required checks as gates.
Confidence: observed for the board, reported for the analysis. Ledger: L-5031, L-5032, L-5038.

## The attendee survey

The team surveyed attendees after the conference with a web form whose submissions arrived as individual emails, then extracted and counted them with scripts (L-6001, L-6003).
About one in five ticket holders answered, 21 people over about three weeks (L-6002).
The respondents skewed toward insiders already active in the community, so the results are the voice of the engaged community, not of the audiences the conference tried to reach (L-6007).

The overall rating averaged 4.57 of 5, with fifteen top marks among 21 (L-6015).
Catering was the strongest area at 4.81, and organizing and logistics followed at 4.62 (L-6016, L-6018).
Trainings averaged 4.31 but held the only 1 in the dataset: one attendee expected hands-on work and learned nothing (L-6020, L-6021).
The analysis answered with a quality floor in the trainer agreement — hands-on exercises, stated prerequisites and stated outcomes (L-6022).

The Business Track averaged 4.12 on eight ratings, and every attendee who answered wants it back, most of them shorter (L-6024).
Its survey-visible audience was mostly providers who came for the conference anyway, so the track showed provider confidence rather than market access.
The analysis recommends keeping and shortening it and judging the 2027 edition by registrations from outside the community (L-6025, L-6026).

The venue bet worked: the hotel that held sessions, rooms and catering was the strongest free-text theme (L-6029).
Its cost was social, because the venue sat far from the town center and from where most people slept (L-6031, L-6032).
Party and socializing tied for the lowest rating at 4.11 (L-6028).
Engineered evenings — organized dinners on training and sprint days, a suggested area and a restaurant list — are the cheapest large gain the analysis found, and they echo Seattle 2006 (L-6033, L-6034, L-6035).

Value for money averaged 4.30 with four unexplained 3s, and the analyst's first reading of it was contradicted by the data, so price perception stays a blind spot (L-6036, L-6037).
Asked about Bucharest in 2027, 16 said yes, 2 perhaps and 3 probably not, and the three probably-nots were the respondents who skipped the profile questions (L-6041, L-6042).

The form itself needs a redesign before the next edition.
Its free-text fields were too small, it had no open comment field, its skip logic hid the audience profile from half the sample, and it asked neither about price nor about what nearly stopped people from coming (L-6008, L-6009, L-6010, L-6011, L-6012).
It reached attendees only; a short version for community members who did not come would hear the people the conference failed to reach (L-6013, L-6014).
Confidence: observed for ratings and counts, reported for free text and the analyst's reading.

## Verdict lists

These lists follow the Seattle 2006 pattern.
They are built from the rows.
A row's general scope records the source's claim and does not pass the promotion rule.

### Good things to do again

- Write day-in-the-life narratives for each role and review them next to adjacent roles (L-5050, S101).
- Separate the responsible manager from helpers, rotate helper shifts, and confirm each assignment the evening before (L-5051, L-5052, L-5053).
- Assign the smaller mandates, such as venue liaison and on-site money, as well as the major roles (L-5055).
- Use separate program, headcount and print-and-order freezes (L-5047).
- Hold a short daily operations meeting and an end-of-day readiness check (L-5048).
- Rehearse recording with the real hardware before setup day (L-5049).
- Keep a plain-text budget aligned to actuals with import rules (L-5013, L-5014, L-5060).
- Run permission-first outreach from one authoritative dataset, and treat introductions, forwarding and audience access as separate permissions (L-5056, L-5057, L-5058, L-5059, S102, S103).
- Keep email source, generated HTML and plain-text fallback together, and preview with a credential-free dry run (L-5064, L-5065, S107).
- Fund a reduced-price Global South route (L-5003, L-5004).
- Offer live streaming through PeerTube for remote viewers (L-5027).
- Keep sessions, rooms and catering under one roof; catering was the best-rated area of the survey (L-6016, L-6029).
- Make the survey numbers reproducible by script, and review the reading adversarially before publishing (L-6003, L-6005).

### Things we did not do that you probably should not either

- Skip the venue-insurance due diligence (L-5034).
- Skip venue and website accessibility information (L-5035).
- Leave website quality assurance to the last day (L-5045, L-5046).
- Leave completed work open on the tracker (L-5033).
- Plan local outreach or audience research and let it lapse without a decision (L-5036, L-5037).
- Settle the VAT regime during ticket sales instead of before them (L-5000, L-5001, L-5074).
- Aim documentation tooling beyond the team's daily habits (L-5039, L-5040).

### Things we might do differently next time

- Write expectations down at the start of planning, including trainer accommodation and compensation, and settle accommodation before confirming trainings (L-5019, L-5020, L-5021).
- Model speaker discounts from day one (L-5023).
- Compare ticket platforms on net revenue, and consider the self-hosted option explicitly (L-5016, L-5018).
- Set attendance goals with separate estimates for the core community and local audiences (L-5010).
- Judge low-sales alarms against a late-buying forecast (L-5008, L-5009).
- Use a flat task list and keep every item on one board (L-5031, L-5042, L-5041).
- Check the combined workload of the person owning daytime operations and a late social event (L-5054).
- Test the assumptions of the committed-spend overlay before relying on it (L-5062).
- Confirm the annual meeting's length and streaming through the Foundation before freezing the schedule (L-5026).
- Decide the streaming tradeoff explicitly for each edition (L-5028).
- Publish the grant argument and the prediction method as sanitized templates (L-5005, L-5067, L-5068, L-5029, L-5066).
- Write a quality floor into each trainer agreement: hands-on exercises, stated prerequisites and stated outcomes (L-6021, L-6022).
- Treat evening programming as an organized deliverable, and pick a venue reachable from where people sleep (L-6033, L-6034).
- Keep the Business Track, shorten it and judge it by registrations from outside the community (L-6026).
- Ask about price perception and attendance barriers directly, and survey community members who did not attend (L-6011, L-6012, L-6014, L-6037).
- Reach out personally to the known participants and ask them for a commitment to come or not come, even when they will only buy late (L-5070).

## Numbers

These figures are aggregates and carry no personal or financial raw data.

- Tickets: 117, of which 5 party-only (S098, F14).
- Recurring in-person community: roughly a hundred people, possibly shrinking, as an approximate planning hypothesis (L-5011, hearsay, pending verification).
- Speakers: 56 presenters listed on the conference website against 117 tickets, about 48 percent (L-5075, as of 2026-11-02).
- Platform fee: 2.89 EUR per ticket paid via Stripe (L-5017, verified 2026-11-02).
- Business Track: eight voices, seven practitioner talks of 25 minutes.
- Attendee survey: 21 responses, about one in five ticket holders, overall rating 4.57 of 5 (L-6002, L-6015).
- Tracker: 110 issues, 58 closed and 52 open at 2026-11-02, with 30 items on the board (S099).

## What this record feeds

The handover contract names six deliverables due at T+60 days (proposed, see [Governance](../../running/governance.md)).
Status as of 2026-11-02:

| Deliverable | Status |
|---|---|
| Post-mortem | Pending. This document is the draft and awaits team sign-off (D9). |
| Financial summary, generalized | Pending. The accounting method is recorded (L-5014), and no generalized result summary is filed. |
| Anonymized survey data, aggregates only | Done. The anonymized analysis is filed as S110 and held back from the public bibliography, because quoted free text can re-identify respondents; the raw submissions stay private (L-6004). |
| The "expected but never written down" list | Pending. F10 supplies the seed (L-5019 to L-5024), and the full list is not complete. |

Two deliverables of the handover contract will not be produced for 2026 and were removed from the table on the organizer's decision of 2026-11-02: the asset and credential handover, and the vendor contacts.
The handbook keeps both in the handover contract for future editions.

```{warning} The 2026 post-mortem awaits team sign-off
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: The 2026 organizing team's sign-off on this case file, plus the generalized financial summary and the full "expected but never written down" list | who-might-know: The 2026 organizing team; Conference Committee | area: post-mortem-2026 | since: 2026-11-02

This record rests on one organizers' debrief and the attendee survey, and the team has not yet confirmed its voice and facts (D9).
```

The ledger rows above are placed in the chapters on finance, ticketing, accessibility, team and governance and others.
Those chapters are the durable home of the lessons, and this page is the case file they cite.

## Sources and further reading

- S098 Plone Conference 2026 facts and lessons for the handbook (organizers' debrief).
- S099 GitHub issues and project board collaboration review.
- S100 Last-phase plan.
- S101 On-site roles.
- S102 Making contact: operator cheat sheet.
- S103 Euregio contact kit.
- S104 Conference accounting overview.
- S105 Conference accounting operator runbook.
- S106 Foundation requirements register.
- S107 Email campaigns.
- S108 Attendance forecast implementation.
- S109 Global South grant application discussion.
- S110 Maastricht 2026 attendee survey analysis (held back, not linked).
