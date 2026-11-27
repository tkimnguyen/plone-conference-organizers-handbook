---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: experience-report
myst:
  html_meta:
    "description lang=en": "A section-by-section annotation of the Seattle 2006 lessons-learned document: what still holds, what has aged and where each point landed in this handbook."
    "keywords": "Plone, Plone Conference, Seattle 2006, lessons learned, digest, appendix"
---

# Annotated Seattle 2006 digest

<!-- Moved from data/ledger/seattle-2006-digest.md, which stays as the T7a working draft. Annotations as of 2026-11-02. -->

**Source and status of this page.**
This appendix annotates the 2006 document "Things We Learned About Running a Plone Conference" (S009) and its companion evaluation pages (S008, S085 to S090).
The plone.org pages carry a CC BY-SA 4.0 footer as archived in 2026, which permits quoting with attribution.
Every quote, figure and price below is as of 2006, in the setting of one U.S. conference with no VAT.
Treat all of it as evidence to weigh, not as a rule.
Every L-1xxx token refers to a row in the lessons ledger, which is rendered on the page `lessons-ledger` and held in `data/ledger/seattle-2006.yml`.

In 2006 the host organization ONE/Northwest (later Groundwire) ran Plone Conference 2006 in Seattle and then did something no later Plone conference repeated for twenty years.
It published a candid account titled "Things We Learned About Running a Plone Conference," together with the full evaluation behind it (S008, L-1003).
This digest follows that document's section order.
For each section it gives one annotation: what still holds, what has aged, and where the point landed in this handbook.
The companion evaluation pages (pre-conference survey, overall evaluation, attendee comments, and the public budget) are covered at the end.

Sources: S009 (the lessons document), S008 (evaluation hub), S085 (pre-conference survey), S086 (overall evaluation), S087 (agenda suggestions), S088 (logistics suggestions), S089 (general comments), S090 (public budget spreadsheet).
The plone.org pages carry a CC BY-SA 4.0 footer as archived in 2026, which permits quoting with attribution; the license that applied to the original 2006 text is for task T3 to confirm.

## How to read the annotations

- **Holds** means the point transfers to a conference as of 2026-11 without change.
- **Aged** means the point depends on 2006 prices, tools, law or circumstances.
- **Landed** names the handbook anchors that cite the ledger rows.
- Rows from a single attendee comment are marked `hearsay` in the ledger and can never back a DEFAULT on their own.
- All rows are `year: 2006, place: Seattle`, so as of 2026 every specific Seattle lesson renders as `[specific · 2006 · Seattle · 20 y] stale-prone`.
  That label is correct for prices and tools.
  For the structural advice, it is the reason this digest exists: a reader should see which old points still hold without reading 20-year-old prose.

## Purpose of this document

The document states its purpose as passing the host organization's experience to future Plone event organizers.
It was written after the event by the lead organizer with input from the co-organizer, the host's finance staff and community advisers (L-1004).
**Holds** completely: this is the handover contract this handbook tries to make routine.
The one weak spot is also instructive: per-session evaluations were offered privately on request, and nothing shows that the offer was ever taken up (L-1005).
An offer without a named recipient and a date tends to lapse.
**Landed:** `handover-contract#case-notes`.

## Overview

About 350 attendees came from 35 U.S. states and 20 countries; more than 110 people took the trainings and about 50 joined the sprint (L-1001).
The training figure is 110 in the overview and 120 in the training section of the same document; the budget counts 337 attendees (L-1047).
Treat all counts as approximate.
**Aged** only as data; it belongs in the conference comparison table, not in advice.
The audience profile from the evaluation (L-1002) is a useful baseline, because about a fifth of attendees had used Plone little or not at all.
**Landed:** `conference-data-table`.

## Master timeline

The headline advice is to start six months out, and starting late is called one of the biggest mistakes an organizer can make (L-1009, L-1010).
The reverse-chronological timeline (L-1011) shows the cost of that minimum: the call for proposals was open only three weeks, sessions were chosen four weeks before early-bird closing, and print went out three weeks before the event.
**Holds** as a floor, not a target.
Seattle had no venue contract risk, no VAT, a sold-out market and a one-bid process.
A European conference with a legal entity, VAT registration, a larger venue and Foundation requirements needs a longer lead time, and the 2026 experience points the same way.
**Landed:** `master-timeline#principles-and-general-lessons`, `master-timeline#case-notes`.

## Why Seattle?

Seattle was chosen because the host lived there and the Foundation received exactly one bid (L-1012).
The upsides were an unreached regional audience and lower costs (L-1013); the downsides were long trips for Europeans and some reluctance to travel to the U.S. (L-1014).
**Holds:** "host city equals organizer's home city" is still how most Plone conferences are placed, and the one-bid situation recurs.
Attendees independently stressed walkability and a lively neighborhood next to the venue (L-1015), which is the most durable city-selection point in the whole archive.
**Landed:** `bid-and-selection#case-notes`, `city-selection#case-notes`, `city-selection#principles-and-general-lessons`.

## Pre-conference survey

The organizers surveyed the community before submitting their bid and credit the survey with telling them what success would look like (L-1016).
The results (L-1017) put building connections above every teaching goal, and the price question (L-1043) set the ticket price.
**Holds**, and it is cheap to repeat.
The survey asked people to rate proposed program ideas rather than to list wishes, and that made the answers usable (L-1057).
**Landed:** `defining-success#principles-and-general-lessons`, `defining-success#case-notes`, `ticketing-and-registration#case-notes`, `programme-portfolio#case-notes`.

## Venue

A small, affordable, city-owned facility was chosen over a downtown hotel, partly for cost and partly because a posh setting would have worked against a grassroots feel (L-1022, L-1023).
Attendees rated the venue only "good to very good" and called it dingy, but praised the neighborhood (L-1024, L-1025).
They asked for a hang-out room separate from the sessions (L-1026).
**Holds:** the trade between budget and polish is still real, and a neighborhood can make up for a plain venue.
The power-outlet advice (L-1147) is a venue question in disguise: check the floor plan for outlets before signing.
**Landed:** `venue#case-notes`, `venue#principles-and-general-lessons`.

## Catering

With cheap food within walking distance, Seattle served only breakfast, an afternoon snack and drinks (L-1027).
The attendee comments are the more transferable part.
Food served inside a session room distracted the session (L-1028), queues cost people the start of talks (L-1029), and people asked for water, less sugar and labeled dishes (L-1030).
**Holds.**
As of 2026-11, dish labels also matter for allergen rules and dietary needs, which turns an attendee's wish into a legal and inclusion requirement in many jurisdictions.
**Landed:** `catering#case-notes`, `catering#principles-and-general-lessons`.

## Why no dinner event?

As novices with an uncertain budget, the organizers skipped a group dinner for 350 (L-1107), and they recommend one for the future (L-1109).
**Holds:** see Social events below, where the attendee evidence makes the same point more strongly.
**Landed:** `social-events-and-party#case-notes`, `social-events-and-party#principles-and-general-lessons`.

## Role of the Plone Foundation

The Foundation lent the host USD 8,000 against a promissory note (as of 2006), repaid after the conference, and the host says it would have declined without the loan (L-1031).
The public budget shows the up-front spending was far larger than the loan, about USD 30,000 of USD 39,000 in minimal costs (L-1032).
Sponsor and early-bird money arriving in time must have covered the gap, but the source does not say so.
**Holds** structurally: up-front cash is the first barrier for a host, and the loan is the lever the Foundation controls.
**Aged:** the Foundation's instruments, amounts and conditions in force must come from the requirements register, not from 2006.
**Landed:** `finance#case-notes`.

## Budget

The conference cost about USD 63,000, earned about USD 99,000 and needed more than 350 staff hours (L-1033, as of 2006).
The host treated it as a paid consulting project and argued for fair pay without a windfall (L-1034).
The detailed budget was published (L-1037).
Its split between unavoidable and optional costs (L-1035) is the most reusable artifact in the archive, and catering and video were the two biggest lines (L-1036).
**Holds:** publish the budget, state the hours, and separate the core event from the cuttable extras.
**Aged:** all amounts, and the U.S. setting with no VAT.
A European conference has to plan around VAT from the start.
**Landed:** `finance#case-notes`, `finance#principles-and-general-lessons`, `handover-contract#case-notes`, `budget-sheet-template`, `cost-benchmarks`.

## Sponsorship

Eighteen sponsors in four tiers brought roughly a quarter of the revenue (L-1038).
Tiers were inherited from earlier conferences, and nobody did much prospecting because matching the previous level was enough (L-1039).
Sponsors found the middle tiers hard to tell apart (L-1040).
The organizers' wish to give sponsors registrant contact data (L-1041) is where this section has aged most.
**Holds:** make each tier's benefits visibly different, and do not assume past sponsors will carry the budget.
**Aged:** see The importance of permission.
**Landed:** `sponsors#case-notes`, `sponsors#principles-and-general-lessons`, `privacy-gdpr#case-notes`.

## Pricing

There were two price tiers, with no discounts and no extra fee for tutorials (L-1044, L-1045).
A one-day rate was recommended after informal one-day sales (L-1046).
The budget shows that about one in five attendees held a complimentary ticket (L-1047), which is easy to forget when forecasting revenue per head.
**Holds:** simple pricing makes revenue predictable, which matters for a first-time organizer.
**Aged:** the prices.
The case against discounts also looks different as of 2026-11, since access and diversity goals often call for targeted reduced tickets; that is a choice for each team to record.
**Landed:** `ticketing-and-registration#case-notes`, `ticketing-and-registration#principles-and-general-lessons`.

## Scholarships

There was no scholarship program beyond speaker payments, and the organizers recommend a Foundation-run fund (L-1053).
**Holds.**
The Foundation offered event and sprint funding (plone.org, as archived in 2026); whether any instrument covers individual travel must come from the requirements register.
**Landed:** `accessibility-and-inclusion#principles-and-general-lessons`.

## Program: starting assumptions

The program kept the community's established format and derived its session types from four explicit goals (L-1018, L-1056).
**Holds:** write the goals before the call for proposals, so the selection has something to be judged against.
**Landed:** `defining-success#case-notes`, `programme-portfolio#case-notes`.

## Program: developing the agenda and invited talks

A wish list of sessions with preferred speakers produced about a dozen invited sessions in two weeks (L-1062).
Announcing those early allowed concrete marketing, which the organizers credit for the sell-out (L-1063).
**Holds** strongly, and it is the clearest causal claim in the document.
**Landed:** `keynotes-and-invited-talks#case-notes`, `marketing-and-outreach#case-notes`, `cfp-and-selection#principles-and-general-lessons` (L-1061).

## Program: the call for proposals

The call published its criteria, suggested topics and announced speaker compensation (L-1064).
A well-connected community member chased proposals personally (L-1065).
**Holds.**
Three weeks is short by 2026 practice, and a published code of conduct, accessibility needs and a privacy notice would sit in the same call as of 2026-11.
**Landed:** `cfp-and-selection#case-notes`, `cfp-and-selection#principles-and-general-lessons`.

## Program: speaker compensation

Seattle paid tutorial leaders and panel organizers but not other speakers, and kept the payments small so the call would not feel high-stakes (L-1070, L-1071).
The budget lists free registration for 44 speakers (L-1047).
**Holds** as reasoning.
As of 2026-11, compensation policy is partly set by Foundation norms, so check the register before copying it.
**Landed:** `speakers-and-speaker-care#case-notes`.

## Program: program committee and evaluating proposals

A mixed committee of experienced and local members rated about 70 proposals 1–5 for content and presenter, in about a week, in a simple online survey tool (L-1066, L-1068).
The organizers decided but mostly followed the scores, and they explicitly advise against letting the committee choose (L-1067).
Four sessions were wait-listed, and rejected proposers were steered into lightning talks and BoFs (L-1069).
**Holds** entirely.
The wait-list also serves the speaker-dropout playbook.
**Aged:** only the named survey tool.
**Landed:** `cfp-and-selection#case-notes`, `cfp-and-selection#principles-and-general-lessons`.

## Program: constructing the agenda

The schedule balanced levels and room sizes, avoided clashes between the best-known speakers, took several days, and needed a second person who knew every session (L-1076, L-1077).
The organizers recommend 3–5 parallel tracks (L-1078), and they circulated the draft to speakers before publishing (L-1079).
Attendees answered with the most consistent complaints in the archive.
They did not want lightning talks against BoFs (L-1083), they wanted the agenda months ahead to plan travel (L-1087), and they did not want all case studies on one day (L-1088).
**Holds.**
The track-count advice depends on audience size; it fitted 350 people with five rooms.
**Landed:** `scheduling#case-notes`, `scheduling#principles-and-general-lessons`.

## Pre-conference training sessions

The trainings were an accident that became, in the organizers' words, one of the biggest reasons for the conference's success (L-1089, L-1090).
They were run financially separate from the conference and priced low (L-1091, L-1092).
That kept the risk with the trainers but confused registrants (L-1095).
The evaluation figures (L-1093) differ slightly from those quoted in the lessons document (6% and 28% against 8% and 26%).
Either way, about a third of attendees were strongly drawn by the trainings.
**Holds:** trainings sell conferences, and attendees expect "tutorial" to mean hands-on work with prerequisites announced in advance (L-1096).
One trainee got no pre-training email and found no room signs on the first morning (L-1097); trainings need their own joining instructions.
**Landed:** `trainings#principles-and-general-lessons`, `trainings#case-notes`.

## Keynote

With no fee budget, an outside keynote arrived through a community member's personal contact and needed only an invitation letter from the Foundation (L-1098).
Attendees asked for a mood-setting opener (L-1099).
**Holds:** ask the community network for keynote leads early, and keep a Foundation invitation letter template ready.
**Landed:** `keynotes-and-invited-talks#case-notes`, `keynotes-and-invited-talks#principles-and-general-lessons`.

## Good things to do again

- Trainings (L-1089).
- Invited sessions plus an open call (L-1061).
- A program committee that reviews (L-1067).
- A simple survey tool for proposals (L-1068).
- At least three skill-level tracks (L-1080).
- A sector focus (L-1058).
- Lightning talks and BoFs at the end of the day (L-1081).
- Defined break lengths (L-1082).

**Holds**, with one internal tension.
Attendees found five-minute breaks too short to change rooms (L-1084), and they did not want lightning talks to compete with BoFs (L-1083).
Read those two rows as refinements of L-1082 and L-1081.
**Landed:** mostly `scheduling#principles-and-general-lessons`, with the rest in `trainings`, `cfp-and-selection` and `programme-portfolio`.

## Things we didn't do that you probably shouldn't either

- Do not require advance signup to attend sessions (L-1086).
- Do not let the program committee choose the sessions (L-1067).

**Holds.**
A few attendees asked for signup for hands-on tutorials to avoid overcrowding.
That points to room sizing, not to general signup.
**Landed:** `scheduling#principles-and-general-lessons`, `cfp-and-selection#principles-and-general-lessons`.

## Things we might do differently next time

- Drop three-hour tutorials in favor of 90 minutes (L-1094); the evaluation agrees (L-1060).
- Add more facilitated workshops (L-1059).
- Possibly take over training registration (L-1095).
- Put long sessions in the morning (L-1085).

**Holds.**
This list is the most honest part of the document and the model for the verdict lists in every handbook chapter.
**Landed:** `trainings#principles-and-general-lessons`, `programme-portfolio#principles-and-general-lessons`, `scheduling#principles-and-general-lessons`.

## Random program-related thoughts

Collecting slides in advance mostly failed; a small reward was suggested (L-1072).
Attendees wanted slides online at the start of each talk at the latest (L-1073), and coaching for weaker presenters (L-1074).
**Holds**, and it is still unsolved in most volunteer conferences.
**Landed:** `speakers-and-speaker-care#case-notes`, `speakers-and-speaker-care#principles-and-general-lessons`.

## Marketing

Outreach to the existing community and one adjacent sector sold out the conference (L-1100).
The organizers recommend a PR committee (L-1101) and channels into education and government (L-1103).
Sector-specific invitations naming relevant sessions worked (L-1102).
The verbatim sample email was not carried over (L-1104, dropped).
The evaluation shows the agenda was the strongest reason to attend (L-1021).
**Holds:** market the program, not the event.
**Landed:** `marketing-and-outreach#case-notes`, `marketing-and-outreach#principles-and-general-lessons`.

## Registration

The advice the organizers themselves inherited was not to build custom registration software and to keep registration simple (L-1048, the ledger's only `reported` rows together with L-1040).
They picked a small vendor for its accountability (L-1049), and they list requirements that still read like a modern ticketing checklist (L-1050, L-1051).
Attendees added automatic receipts, purchase orders and keeping payer and attendee apart (L-1052).
**Holds** almost verbatim.
**Aged:** a 2026-11 checklist adds VAT-correct invoices, consent records and data-processing terms with the vendor.
**Landed:** `ticketing-and-registration#how-to`, `ticketing-and-registration#case-notes`, `ticketing-and-registration#principles-and-general-lessons`.

## The importance of permission

The organizers recommend telling registrants that contact details will be shared, and with whom, with an opt-out checkbox (L-1042).
**Aged** decisively.
Under the EU GDPR and comparable laws, passing attendee data to sponsors needs informed opt-in consent, and the wish behind it (L-1041) is a legal risk as of 2026-11, not a missed perk.
The handbook keeps both rows as case notes, as a dated example of how fast this ground moved.
**Landed:** `privacy-gdpr#case-notes`.

## Visa letters

A U.S. host sent short invitation letters on letterhead to visitors who needed them (L-1105).
**Holds** in form: every host needs a letter template and a turnaround promise.
**Aged** in substance, because visa rules, processing times and the countries concerned change.
A single survey wish for good visa information was dropped as a duplicate (L-1106).
**Landed:** `visas-and-travel#case-notes`.

## Social events

Seattle ran a minimal social program, with dinners on your own and a suggested neighborhood each night (L-1108).
It rated second-lowest of all logistics items (L-1110).
Attendees said unstructured evenings favored insiders and drinking (L-1111), although the neighborhood lists helped (L-1112).
**Holds**, and the attendee evidence is stronger than the organizers' own recommendation (L-1109).
At least one shared, inclusive evening event is a baseline, not a luxury.
The icebreaker (L-1113) is the daytime half of the same lesson.
**Landed:** `social-events-and-party#case-notes`, `social-events-and-party#principles-and-general-lessons`, `signage-and-showtime#principles-and-general-lessons`.

## Internet connectivity

The two failures were a vendor reading "install at 9 a.m." as the time to start work (L-1114) and an address pool too small for 350 users (L-1115).
Internet was the lowest-rated item (L-1123).
The rules (L-1116, L-1118, L-1119, L-1121, L-1122) mostly **hold**.
Size for everyone at once, with several devices each.
Insist on it in writing.
Keep ports open.
Have a direct number for the upstream network administrators.
The run-it-open rule (L-1120) is **aged** and was dropped: an unencrypted network is no longer acceptable practice.
One attendee argued for running Wi-Fi yourself (L-1117, hearsay), which is the opposite of the organizers' rule.
The handbook keeps the organizers' rule as evidence, and teams with in-house network skills may record a different choice.
**Landed:** `av-recording-internet#case-notes`, `av-recording-internet#principles-and-general-lessons`, `wifi-failure#first-hour-actions`.

## Videotaping

Two rooms were recorded professionally (L-1124), with tutorials and outreach talks chosen first, partly to keep a reason to attend in person (L-1125).
Attendees asked for every talk to be recorded (L-1126).
A community volunteer covered the gaps and even streamed some sessions (L-1128).
One attendee already raised the carbon cost of flying in, and suggested remote participation as a remedy (L-1129, hearsay).
**Aged:** costs, and the idea that recording everything is a luxury.
Recording every main-track talk is widely expected as of 2026-11.
**Holds:** do not build your own video pipeline (L-1127), and value the community volunteer.
**Landed:** `av-recording-internet#case-notes`, `av-recording-internet#principles-and-general-lessons`, `hybrid-online#case-notes`, `sustainability#case-notes`.

## Conference communications infrastructure

The conference used one definitive website (L-1130).
An attendee list ran in three modes: announce-only before, open discussion during, and announce-only after (L-1131).
A throwaway wiki held bios and ad hoc events (L-1133), and shared tags covered posts and photos (L-1134).
Attendees called the list and wiki a standard to keep (L-1132).
**Holds:** one source of truth on the web, plus one channel that changes mode around the event.
**Aged:** the wiki software, the social services and the "Plone is slower than a wiki" reasoning, all from 2006.
The modern equivalent is a chat platform used the same way.
**Landed:** `web-comms-brand#case-notes`, `web-comms-brand#principles-and-general-lessons`.

## T-shirts

The organizers chose good, sweatshop-free, screen-printed shirts (L-1135).
They print at least 10% extra (L-1136), collect sizes at registration (L-1137) and use a local printer (L-1138).
**Holds** completely.
The unit cost is a dated benchmark (L-1139), and one attendee asked for pre-shrunk shirts (L-1144, hearsay).
**Landed:** `print-and-merch#case-notes`, `print-and-merch#principles-and-general-lessons`, `cost-benchmarks`.

## Printed materials

There was a glossy schedule brochure that paid off, plus a cheap handout (L-1140).
The name tags showed name, organization, place and chat nickname, with role ribbons (L-1141).
Spare blank tags were needed (L-1142).
Banners were reused afterwards (L-1143).
**Holds.**
Name-tag legibility (L-1055) and screen legibility (L-1054) belong to accessibility as much as to print.
**Landed:** `print-and-merch#case-notes`, `print-and-merch#principles-and-general-lessons`, `accessibility-and-inclusion#case-notes`.

## AV and other physical requirements

Seattle recommends bright projectors with a spare (L-1145), screens of at least about 3 by 3 meters (L-1146), and many floor outlets or a cable crew (L-1147).
One attendee flagged floor cables as a tripping hazard (L-1148).
**Holds**, though projector brightness figures are dated and many venues have built-in displays as of 2026-11.
The cable point is a safety duty, not only a convenience.
**Landed:** `av-recording-internet#principles-and-general-lessons`, `venue#principles-and-general-lessons`, `health-safety-emergencies#case-notes`.

## Showtime

The registration desk advice still reads like a modern checklist (L-1149, L-1150).
Use about six trusted volunteers, keep badges alphabetized and keep one master list.
Check training attendees in the evening before the conference.
Shirts went out from day two onward, with volunteers getting theirs on day one (L-1151).
One sign per room per day was posted (L-1152).
**Holds** in full; badge printing on demand and digital check-in change the tools, not the advice.
**Landed:** `signage-and-showtime#how-to`, `signage-and-showtime#principles-and-general-lessons`.

## Post-conference sprint

A sprint that nobody planned was hosted free by a local institution and run as open space (L-1153, L-1154, L-1156).
The organizers' rules (L-1155, L-1157, L-1158) **hold**.
Fix dates and venue early, treat the sprint as the way newcomers become contributors, and recruit team leads in advance.
About 28% of evaluation respondents attended and rated the sprint 4.18 of 5 (L-1159).
The comments show where that purpose was missed.
The sprint's purpose was not explained to non-developers (L-1161), it was less diverse than the conference (L-1162), and two days felt short (L-1160).
**Landed:** `sprints#case-notes`, `sprints#principles-and-general-lessons`.

## Thanks and acknowledgements

The section credits named people and organizations.
Under D7 the names are not carried into the ledger (L-1164, dropped); the roles they played are recorded in L-1006, L-1007 and L-1008.
**Holds** as practice: name the advisers and volunteers whose help a successor team can ask for.
The two-person core team with host-organization backing (L-1006) is the staffing baseline that later teams can compare against.
**Landed:** `team-and-governance#case-notes`, `stakeholder-map#principles-and-general-lessons`, `volunteers-and-roles#case-notes`.

## Companion evaluation pages

- **Evaluation hub (S008).** The hub makes the point of the whole set: publish the evidence, not only the conclusions (L-1003).
- **Pre-conference survey (S085).** It covers goals, program ideas and price tolerance (L-1017, L-1043, L-1057). Two single-comment rows were dropped (L-1106, L-1163).
- **Overall evaluation (S086).** The outcome questions are worth reusing: felt more connected, felt empowered to contribute, and planned follow-up actions (L-1019). The questionnaire structure became the attendee survey template (L-1020, landed at `survey-template`).
- **Agenda suggestions, logistics suggestions, general comments (S087, S088, S089).** Points made by several attendees are `observed`; points made by one attendee are `hearsay` and appear only as case notes. The comments carry two signals the organizers' narrative underplays: social inclusion in the evenings (L-1111) and professional expectations of business attendees (L-1075, landed at `community-and-speaker-expectations#case-notes`).
- **Public budget (S090).** Covers unavoidable against optional costs, up-front exposure, complimentary tickets and sponsorship tiers (L-1032, L-1035, L-1036, L-1038, L-1047). The budget lists videography at about USD 16,000 while the narrative says USD 15,000; the source does not explain the difference.

## Contradictions and tensions recorded

| Rows | Tension | Handling |
|---|---|---|
| L-1116 / L-1117 | Outsource Wi-Fi to an accountable provider, or run it yourself | Organizer rule as evidence; the opposite view is a single hearsay row. A team may record its own choice in its Tailoring Record. |
| L-1082 / L-1084 | 5–10 minute breaks recommended; 5 minutes found too short | Read L-1084 as the lower bound: allow at least 10 minutes where people change rooms. |
| L-1081 / L-1083 | End the day with lightning talks and BoFs; do not run them at the same time | Both hold; schedule them one after the other. |
| L-1042 / law as of 2026-11 | Opt-out sharing of attendee data | Aged; kept as a case note only. |
| L-1120 | Open, unencrypted Wi-Fi | Dropped as superseded. |
