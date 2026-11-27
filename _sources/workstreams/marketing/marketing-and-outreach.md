---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to plan audience, outreach and promotion for a Plone Conference, from segments and local reach to permission-first contact."
    "keywords": "Plone, Plone Conference, marketing, outreach, audience, local audience"
---

# Marketing and outreach

## Why it matters

A conference sells nothing until the right people know it exists, see what is in it for them and can persuade their employer to pay.
Marketing turns a venue, a program and a ticket price into attendance.
When it is thin, the symptom is a sales curve that stays flat until the last weeks, when little can still be fixed.

The Foundation expects every hosting proposal to say how it will attract site builders who have not used Plone before.
It also expects reach into the traditional segments (nonprofits, education, government, intranets) and into emerging corporate users (L-4072, S049).
That makes marketing a plan with named audiences, not a general wish for visibility.

Marketing touches the Foundation, sponsors who expect reach, the Plone community, and other organizations whose audiences are not yours to use.
Outreach to those organizations adds a duty that advertising does not have.
A message nobody asked for costs trust, and a volunteer-run conference lives on trust.

This chapter feeds the low-ticket-sales playbook in Part 3, which starts from the audience plan written here.
The website, email and brand mechanics sit in [Web, comms and brand](web-comms-brand.md).

## Applies when

- `all` Applies to every Plone conference, because every conference has to find its audience.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-1100, L-4072) **Is there a written marketing plan that names the audience segments and one channel for each?** Hosting calls ask for such a plan (requirements register row R-027, unverified as of 2026-11-02, so not a MUST here). Treat the established community, the traditional sectors and corporate users as separate segments. (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-4109, L-5036) **Who owns local audience development, or is it explicitly dropped from scope?** Reaching local people is a scope decision, not a side effect of choosing a city. Name one owner and one dated first action, or record in the Tailoring Record that you are not pursuing it. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will you appear at other events, and as a speaker or as an exhibitor?** A talk or case study at another sector's conference costs far less than sponsoring it, and booth traffic mostly came from people already known. (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-1063, L-2012) **Which headline sessions will you confirm and announce before the program closes?** Early named sessions gave marketing something concrete to sell and allowed sector-specific invitations. (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Will you contact other organizations and communities directly?** If yes, work permission-first, as in the how-to. Consent rules differ by country and by kind of recipient, so check the rules with a qualified local adviser before the first campaign. (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Will you offer attendees a letter template for asking their employer to approve the trip?** One conference did, on its site. (decide-by: T-4m)

## How-to

### Plan (T-12m to T-9m)

1. Write the audience plan on one page: three segments, one channel and one measurable outcome each. Done: the plan is filed with your [Tailoring Record](../../start/tailor.md).
2. Decide the local audience question. Done: a named owner and a first action with a date, or a recorded decision to drop it.
3. Contact local Python groups to collaborate or to hold a joint event (L-4033, S004). Done: each group has answered, even if the answer is no.
4. Create one outreach dataset with one row per organization, role and route, never one row per scraped person (L-5059, S102). Done: columns for owner, permission, outcome, next action and suppression exist.
5. Regenerate every spreadsheet or print view from the dataset and never edit a view alone (L-5059). Done: the dataset is under version control and views carry a build date.

### Prepare (T-9m to T-4m)

6. Confirm headline sessions and keynotes as early as the speakers allow. Done: at least three session titles you may publish.
7. Prepare one one-page handout per product, for example the technical conference, a business track or trainings. Done: each handout is tagged with its product, and you send only the one the recipient asked about.
8. Record a promo video, either produced or simply organizers explaining why people should come (L-4035, S004). Done: the video is linked from the website.
9. Draft one covering message per route with one relevance sentence, one offer and one request. Done: a second person has read each draft.

### Run (T-6m to T-1w)

10. Verify each organization's current work and its own contact route before you write (L-5057, S102). Done: the row is marked verified with the date.
11. Recheck the matching session, ticket path and price before you attach any handout (L-5057). Done: the handout facts agree with the live site.
12. Contact permission-first and record objections or suppression in the dataset at once (L-5056, S102). A public contact route does not by itself give permission to send a campaign. Done: every contact has a recorded permission basis.
13. Ask for one permission at a time: an introduction, forwarding and access to an audience are separate, as the principle below says. Done: the dataset records which one was granted.
14. Release routes in waves, then pause and read the replies before releasing the next wave. Done: the second wave contains only routes supported by replies, introductions or attributed registrations.
15. Record the result and next action in the dataset after each permitted contact (L-5059). Done: no follow-up lives only in a mailbox.
16. Measure outcomes, not reach: positive replies, completed introductions, activated advocates and attributed registrations. Done: a weekly count of those four, with list size and opens left out.

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S103 | ledger: L-5058 | confidence: observed | status: active | basis: structural | reason: Consent to one kind of contact does not extend to a different act, so each act needs its own permission.

Treat introductions, forwarding and access to another organization's audience as separate permissions.
A relationship or a directory entry grants none of them automatically.
```

Two more pieces of advice rest on one account each and stay candidates until a second conference confirms them.
An early organizer team advised considering a public relations committee with technology-sector marketing experience (L-1101).
The same team advised seeking channels that reach technologists in higher education and in city and state government (L-1103).

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S082 | ledger: L-4228 | confidence: observed | status: active

The site offered a "convince your boss" letter template for attendees who needed employer approval.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5036 | confidence: reported | status: active

University outreach planned for local audience development was never executed.
Its expected audience contribution stayed unsupported.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5037 | confidence: reported | status: active

A decision-maker research program reached written interview and survey scripts but was never run.
Preparing the materials did not validate the audience.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6050 | confidence: reported | status: active

A survey respondent asked to invite students and younger developers to the training days, corroborating the planned university outreach that was dropped before execution (L-5036, L-5037).
```

```{note} [specific · 2018 · Tokyo · 8 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2018 | place: Tokyo | org: Plone Conference 2018 Steering Committee | source: S095 | ledger: L-4151 | confidence: observed | status: active

To draw local participants, the bid planned day tickets, a Japanese-language track and simultaneous interpretation of keynotes.
```

```{note} [specific · 2018 · Tokyo · 8 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2018 | place: Tokyo | org: Plone Conference 2018 Steering Committee | source: S095 | ledger: L-4155 | confidence: observed | status: active

The convention bureau offered to promote the event through brochures, its events calendar and visitor guides once the city won the bid.
```

```{note} [specific · 2015 · State College · 11 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2015 | place: State College | org: Plone Foundation | source: S046 | ledger: L-4121 | confidence: reported | status: active

At a university web conference of about 500 people, almost all booth traffic for Plone providers came from people they already knew.
```

```{note} [specific · 2015 · n/a · 11 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2015 | place: n/a | org: Plone Foundation | source: S046 | ledger: L-4122 | confidence: reported | status: active

Board members noted that submitting a talk or case study to another sector's conference costs far less than sponsoring it.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S094 | ledger: L-3123 | confidence: observed | status: active

The organizers planned to attend other conferences and sprints during the year to publicize the event and look for sponsors.
They also planned to reuse the established conference domain and social account.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S094 | ledger: L-3124 | confidence: observed | status: active

In the months before the conference the organizers planned talks at local universities and other organizations to involve students.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2095 | confidence: observed | status: active

Local marketing used four large banners and 300 A0 posters.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S015 | ledger: L-2012 | confidence: observed | status: active

Feedback gathered while promoting at EuroPython showed that registrations depend on announcing talks and speakers early.
The organizers published them later than they wanted.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S019 | ledger: L-2061 | confidence: observed | status: active

The bid planned local press outreach and promotion to local government.
It also asked other national Plone companies to bring clients and prospects.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S086 | ledger: L-1021 | confidence: observed | status: active

Asked what drove their decision to attend, respondents rated the agenda highest (3.52 of 5), then location (3.06) and cost (3.01).
Trainings (2.34) and the sprint (1.86) were decisive for smaller groups.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1063 | confidence: observed | status: active

Confirming well-known invited sessions early let the team market concrete headline sessions before the agenda was complete.
The organizers believe this led directly to the sold-out conference.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1100 | confidence: observed | status: active

Thorough outreach within the Plone community and the U.S. nonprofit technology sector sold out the conference at 350 attendees.
Much room remained to reach the wider technology, education and government sectors.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1102 | confidence: observed | status: active

Because invited sessions and sector panels were confirmed early, the organizers could send sector-specific invitations naming the sessions most relevant to each sector.
```

## Risks

```{warning} Planned local outreach is never executed
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Give local audience development one named owner and one dated first action, or record in the Tailoring Record that it is out of scope | owner-role: marketing lead | playbook: low-ticket-sales

Planning a local channel does not produce attendance until someone runs it.
```

```{warning} Headline sessions are announced after sales have stalled
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Fix a date for confirming and publishing headline sessions before the program closes, and review the sales curve against it | owner-role: program chair | playbook: low-ticket-sales

Judged for a typical mid-size conference.
```

```{warning} An outreach message reaches recipients who gave no permission
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Contact organizations only through verified organization-owned routes, record permission and suppression in the dataset, and have a qualified local adviser review the rules first | owner-role: outreach lead

A public contact route does not establish permission to send a campaign.
```

## Thin content

```{warning} No measured outreach results
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Counts of replies, introductions and attributed registrations from at least one completed outreach campaign, with the attribution method | who-might-know: Past marketing leads; Foundation marketing team | area: other

The archive holds no outcome figures that show which outreach routes produced attendees.
```

```{warning} Permission-first method rests on one conference
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second organizing team's account of consent-based outreach, plus consent notes for organization contact in more than one jurisdiction | who-might-know: Foundation legal adviser; past organizers outside the Netherlands | area: jurisdiction-annexes

The method and the consent boundary come from one team's operating notes.
```

```{warning} No data on partner events and reduced local prices
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Attendance split by route (partner event, reduced local ticket, existing community) from past conferences | who-might-know: Past treasurers and ticketing leads | area: pricing-elasticity

Only an unverified debrief remark links extra audiences to a joint Python event and reduced local prices.
```

```{warning} Channel advice predates current platforms
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: Channel and print advice rechecked against platforms in use as of the next review | who-might-know: Foundation marketing team; organizers of the latest editions | area: other

Posters, banners and mailing-list outreach come from conferences held in 2012 and earlier.
```

## Sources and further reading

- S004 Conference Planning Schedule, Plone Foundation conference team, plone.org.
- S009 "Things We Learned About Running a Plone Conference", Seattle 2006 evaluation, plone.org.
- S015 "Plone Conference 2010: An Organiser's View", Netsight, archived copy.
- S019 Bristol 2010 conference record and original proposal, plone.org.
- S036 "Plone Conference 2012 Wrap-up", organizer account, Four Digits.
- S046 Foundation board minutes, 2015, on the conference's included-training model.
- S049 2016 call for proposals, codified requirements and recommended earlier reports, plone.org.
- S082 Maastricht 2026 post-conference home page.
- S086 Seattle 2006 overall conference evaluation, plone.org.
- S094 Brasília 2013 conference proposal.
- S095 Tokyo 2018 winning proposal.
- S099 GitHub issues and project board collaboration review, 2026 organizing team.
- S102 Making contact: operator cheat sheet, 2026 organizing team.
- S103 Contact kit, 2026 organizing team.
- S110 Maastricht 2026 attendee survey analysis.
