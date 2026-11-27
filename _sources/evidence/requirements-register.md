---
steward: unassigned
deputy: unassigned
review-by: 2027-05-02
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "The register of Plone Foundation requirements for conferences that back the MUST badges in this handbook, with status and as-of date per row."
    "keywords": "Plone, Plone Conference, Foundation requirements, register, MUST, requirements register"
---

# Foundation requirements register

<!-- Mirror of data/requirements-register.yml as of 2026-11-02. The YAML is the source of truth. A generator may replace the hand-rendered table below; when it does, this page becomes a generated page and the note about the mirror goes away. -->

## What the register is

The Plone Foundation has never published one list of what a conference must do.
Its own board named a written list of conference and sprint requirements as a 2025 priority, which confirms that none existed (L-4060).
In 2023 an organizer had already asked for written guidelines (L-4190).
The requirements existed anyway, scattered across Foundation resolutions, calls for proposals, a planning schedule, sponsorship policy pages and committee minutes.
Teams met them as expectations that nobody had written down in one place.

This register is the handbook's attempt at that list.
It is **Level A** of a two-level model.
Level A is what a document says: a requirement located in a Foundation text, with its source and the date a person last checked it.
Level B is what the Foundation itself confirms in answer to a question, and the ask is described below.
Nothing here is Foundation policy.
The handbook is advisory, and the register records what the sources say, not what the Foundation has agreed to.

Read this register as a basis for negotiations, not as a rulebook.
It is the draft of a letter of intent between the Foundation and an organising team: what the Plone Conference should be, and how it is handled.
Which rows bind a given edition depends on the organisational model the Board and the team choose, and every edition should fix that choice in writing at bid time.

## Two organisational models

The rows that pass risk and money between the Board and the organiser read differently under each model.

**Model 1: the Foundation carries the risk.**
The Foundation, acting as financial agent, assumes the financial risk and keeps any surplus (R-008, R-009).
In exchange the Board can dictate rules about budget and planning: regular updates, a Board member in the planning, final authority on financial decisions, and the share of registration revenue (R-010).
The rows marked conditional in this register bind under this model.

**Model 2: the organiser carries the risk.**
The organising company or group bears the full risk and keeps any surplus.
This was the de-facto model before the 2017 financial policy and remains the common one (L-4056).
The Foundation's involvement is the naming approval, the community floor and the conference timeline, and the budget and planning rows become guidance the organiser adopts or negotiates.

Hybrids exist.
Brasília 2013 replaced the percentage share with a fixed fee (L-3116), and Eibar 2023 ended in a donation (L-4189).
Some rows bind under every model, because they are the community floor rather than conference rules: the naming approval (R-001, R-002) as a trademark matter, insurance due diligence (R-012) as legal prudence, the Code of Conduct agreement (R-013) as community policy, and the photo consent (R-014) as privacy practice.
Everything else is the negotiation surface, and the outcome belongs in a short letter of intent per edition.

The register backs the MUST badge.
A decision with the MUST badge cites one row by ID and carries that row's as-of date, for example `req: R-012; as-of: 2026-11-02`.
When a row is re-verified, every badge that cites it fails the build until the date is updated, which is the intended behavior.

## Status values

| Status | Meaning | Effect on badges |
|---|---|---|
| `verified-current` | The live Foundation text was read and still says this. | May back a MUST. |
| `verified-changed` | The live text was read and differs from the older call for proposals. The row states the current form. | May back a MUST. |
| `unverifiable` | The requirement appears only in older calls for proposals, and no current text restates or contradicts it. | Cannot back a MUST. The chapter shows a DEFAULT with a thin marker. |
| `unverified-pending-Foundation-ask` | The handbook team believes the requirement applies but found no Foundation text that states it. | Cannot back a MUST until the Foundation answers. |

Rows with status `unverifiable` still carry a proposed badge of the form "pending confirmation".
Read that as a proposal, not as a rule.

## As of 2026-11-02

The register was last verified as of 2026-11-02 and has 37 rows, R-001 to R-037.
Twenty rows are `verified-current`, one is `verified-changed`, twelve are `unverifiable` and four are `unverified-pending-Foundation-ask`.
The four pending rows (R-034 to R-037) are written as questions, because no Foundation text read states an answer: the length and streaming of the slot for the Foundation's annual member meeting, the VAT position of a university organizer compared with a company, whether the Foundation sells conference tickets itself, and whether it still offers seed loans, advances or the financial-agent model.

Ten questions to the Foundation would turn the pending and unverifiable rows into confirmed ones.
They are collected as one ask bundle and have not been sent as of 2026-11-02.
Sending them is a human decision that is still open as of 2026-11-02.
Until an answer arrives, treat every row marked `unverifiable` or `unverified-pending-Foundation-ask` as a question to put to the Conference Committee at the start of your planning, not as a settled rule.

## How the YAML relates to this page

The file `data/requirements-register.yml` is the source of truth.
The lint rule N02 reads it, not this page.
This page mirrors it as of 2026-11-02, in a shorter form: it leaves out the status note, the verification date per row and the source locators, to keep the table readable.
For those columns, and for the source IDs behind each row, see `data/requirements-register.yml`.
Two public role addresses in the YAML text are replaced here by a description, so that no address appears on a published page.

If the two disagree, the YAML wins, and the page needs a correction through [Update](../running/update.md).

## The register

| ID | Requirement | Status | Source force | Proposed badge | Target chapters |
|---|---|---|---|---|---|
| R-001 | An event may only be called "Plone Conference <year>" or "International Plone Conference" if the Foundation approves it, and the Foundation selects its location. | verified-current | required | MUST | `team-and-governance`, `web-comms-brand` |
| R-002 | An event using "Plone" in its name must primarily feature Plone and must not present itself as Foundation-endorsed unless the Foundation explicitly endorsed it. | verified-current | required | MUST | `web-comms-brand` |
| R-003 | Hosting proposals go to the Board's public role address as PDF or ODF, the Board pre-qualifies them, Foundation members vote, and the Board bears ultimate responsibility for the award. | unverifiable | required | MUST pending confirmation | `team-and-governance`, `city-selection` |
| R-004 | A hosting proposal must include a complete conference budget covering all costs and revenue. | unverifiable | required | MUST pending confirmation | `finance` |
| R-005 | The organizer develops and tracks a budget with sponsor income, ticket income and expenses, including a Plone Foundation line. | verified-current | guidance | DEFAULT | `finance` |
| R-006 | A hosting proposal must explain how the organizer will manage cash flow, because money must be committed before sponsorship and registration income arrives. | unverifiable | required | MUST pending confirmation | `finance`, `cash-flow-crunch` |
| R-007 | A hosting proposal must state explicitly whether the organizers ask the Foundation to be the financial agent for the event. | verified-current | required | MUST | `legal-entity-and-financial-agent` |
| R-008 | If the Foundation acts as financial agent, it assumes the financial risk and grants use of its banking and PayPal accounts, accounting systems and Treasurer, but does not pay the organizers' extra work hours. | verified-current | conditional | MUST (when agent) | `legal-entity-and-financial-agent`, `finance` |
| R-009 | In exchange, the organizers send the Board regular updates, at least one Board member joins the planning, the Board has final authority on all financial decisions, and the Foundation receives any surplus. | verified-current | conditional | MUST (when agent) | `legal-entity-and-financial-agent` |
| R-010 | The Foundation collects a share of per-person registration revenue (15 %, not of sponsorship) after the conference, and the organizer budgets for it. | verified-changed | required | MUST pending confirmation | `finance` |
| R-011 | A hosting proposal estimates the cost per attendee and keeps the conference affordable, with a target of USD 250–450 per person. | unverifiable | required | DEFAULT | `ticketing-and-registration` |
| R-012 | Organizers must perform due diligence on local law to establish which types and limits of insurance coverage the event requires. | verified-current | required | MUST | `contracts-legal-insurance` |
| R-013 | The conference adheres to the Plone Code of Conduct, publishes it on the website, and makes ticket buyers agree to abide by it. | verified-current | required | MUST | `code-of-conduct-operations`, `ticketing-and-registration` |
| R-014 | The website and ticketing include the attendee's agreement to be photographed. | verified-current | guidance | DEFAULT | `privacy-gdpr`, `ticketing-and-registration` |
| R-015 | The published schedule includes the Plone Foundation annual member meeting, which is held once a year at the conference. | verified-current | guidance | MUST (Foundation meeting coincides with conference) | `scheduling` |
| R-016 | The organizer plans to record as many sessions as possible, preferring fast turnaround, with live streaming optional. | verified-current | encouraged | DEFAULT | `av-recording-internet` |
| R-017 | The conference design includes pre-conference trainings (CFPs: 1–2 days). | verified-current | encouraged | DEFAULT | `trainings` |
| R-018 | The conference design includes post-conference sprints (CFPs: 2–3 days, with an experienced sprint leader). | verified-current | encouraged | DEFAULT | `sprints` |
| R-019 | The conference design includes three days of conference talks. | unverifiable | encouraged | DEFAULT | `programme-portfolio` |
| R-020 | The conference is held between mid-September and mid-November and avoids major religious and national holidays. | unverifiable | required | DEFAULT pending confirmation | `master-timeline`, `city-selection` |
| R-021 | The venue must hold 200–500 people (250–500 in 2016–2017) in a plenary room, with breakout rooms for 2–3 tracks and informal gathering space. | unverifiable | required | OPTION pending confirmation | `venue` |
| R-022 | The venue provides reliable wireless access for all attendees at once and appropriate audio-visual support. | unverifiable | required | DEFAULT pending confirmation | `av-recording-internet`, `venue` |
| R-023 | The venue is at most one hour from an international airport, with affordable transport so attendees need no car. | unverifiable | required | DEFAULT pending confirmation | `city-selection`, `hotels-and-local-logistics` |
| R-024 | The conference provides snacks, coffee and lunch. | unverifiable | required | DEFAULT pending confirmation | `catering` |
| R-025 | The organizer provides invitation letters and visa-application support throughout the planning period. | verified-current | guidance | DEFAULT | `visas-and-travel` |
| R-026 | A hosting proposal names the key people, their history with the Plone community, and their event-organizing experience. | unverifiable | required | MUST pending confirmation | `team-and-governance` |
| R-027 | A hosting proposal includes a conference marketing plan and a plan for engaging the community in the agenda. | unverifiable | required | MUST pending confirmation | `marketing-and-outreach`, `cfp-and-selection` |
| R-028 | The organizer considers how to reduce the event's environmental footprint. | verified-current | encouraged | OPTION | `sustainability` |
| R-029 | The organizing team works with the Conference Committee, which provides continuity between editions and is reached at the Conference Committee's public role address. | verified-current | guidance | DEFAULT | `team-and-governance`, `handover-contract` |
| R-030 | Any event that receives Foundation funding declares in all its communications "The <EventName> is funded by the Plone Foundation". | verified-current | conditional | MUST (when funded) | `sponsors`, `web-comms-brand` |
| R-031 | Foundation funds may not buy alcohol for resale, and alcohol paid from them is only for consumption with meals. | verified-current | conditional | MUST (when funded) | `social-events-and-party`, `finance` |
| R-032 | A funded event reports back via the Sponsorship Report Form and a plone.org news item before reimbursement. | verified-current | conditional | MUST (when funded) | `sprints`, `finance` |
| R-033 | Funding requests go through the plone.org form, at least one month ahead for community sprints and by December of the prior year for strategic sprints. | verified-current | conditional | MUST (when requesting funds) | `sprints`, `finance` |
| R-034 | Does the Foundation require at least a one-hour, streamed slot for its annual member meeting and report, given that 25 minutes proved insufficient in 2026? | unverified-pending-Foundation-ask | none yet | MUST candidate | `scheduling`, `av-recording-internet` |
| R-035 | Can a university organizer sell tickets without charging VAT where a company organizer must charge it, and in which jurisdictions? | unverified-pending-Foundation-ask | none yet | MUST candidate (jurisdiction annex) | `legal-entity-and-financial-agent`, `finance` |
| R-036 | Does the Foundation still sell conference tickets itself (as a US entity, without EU VAT), and under which conditions? | unverified-pending-Foundation-ask | none yet | MUST candidate | `legal-entity-and-financial-agent`, `ticketing-and-registration` |
| R-037 | Does the Foundation still offer seed loans or advances against up-front costs, or act as financial agent, for the conference? | unverified-pending-Foundation-ask | none yet | MUST candidate | `legal-entity-and-financial-agent`, `finance` |

Read the badge column with the status column.
A badge such as "MUST pending confirmation" belongs to a row that cannot yet back a MUST.
Conditional badges such as "MUST (when funded)" apply only to a team that takes the Foundation's money or accounts.

## Notes on single rows

Row R-010 records the Foundation's share of per-person registration revenue, which moved from 15 percent to 20 percent in 2018 and back to 15 percent in 2019 and 2020.
A 2013 bid shows that the share is negotiable in kind: because registration was planned to be free, the bid offered the Foundation a fixed payment instead of the usual 15 percent share (L-3114).
Read the rate as a figure to confirm with the Foundation, not as a constant.

## Using the register

1. Start from the chapter you are working on and find its rows in the last column.
2. Check the status before you rely on a row.
3. For a row that cannot back a MUST, ask the Conference Committee, and record the answer in your Tailoring Record (see [Tailor](../start/tailor.md)).
4. Deviate from a MUST only with a written Foundation exception, linked in the record.
5. Send back what you learn, so that the next verification starts from your answer: [Update](../running/update.md).
