---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to build a dated master timeline for a Plone conference, from the first team meeting to the freezes, and what compressed schedules teach."
    "keywords": "Plone, Plone Conference, master timeline, planning schedule, freezes, runway"
---

# Master timeline

## Why it matters

A conference has fixed dates and moving parts.
The venue, the suppliers, the speakers and the funders each run on their own lead times, and none of them waits for the organizers to be ready.
A team that starts late loses choices first and money second.

The timeline is the spine that every other chapter hangs on.
It tells each workstream when its work must be finished so that the next one can start.
It also tells the Foundation and the Committee when the team will ask for something.

The usual failure is not a missed deadline but a hidden one.
Funding requests, print orders and headcount all have dates after which a change costs money.
A master timeline makes those dates visible while there is still room to move.

## Applies when

- `all` Every Plone conference runs on a dated schedule, whatever its size or format.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-2070, L-4026) **When does the planning clock start, and who owns the schedule?** Start the venue search about a year ahead and hold the initial team meeting no later than November or December of the year before. Name one person who owns the dated schedule. (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Do you need Foundation funds, and have you asked before the board budget is drafted?** The board drafts its budget in December and publishes it in January, so a request made later in the year is less likely to find money left (L-4051). The evidence is one policy page, so confirm the cycle with the board. (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Which dates avoid major religious and national holidays?** A call for proposals advised checking, because several religious feasts move each year and can fall in October (L-4073). The register row that sets the season is unverified, so treat the advice as a prompt, not a rule. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Is your runway shorter than six months?** Two conferences ran on short runways, one of about six months and one that opened its website in May for an October event (L-1011, L-4175). Treat both as floors, not plans. (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Which freezes will you set, and what does each one lock?** One team froze the program, the headcount and the print and order list on separate dates before the final rehearsal (L-5047). The evidence comes from one conference. (decide-by: T-3m)

## How-to

### From T-12m to T-9m

1. Hold the initial team meeting and set a meeting cadence: monthly, then every two weeks from late spring, then weekly in the last month before the conference (L-4026). Done when the cadence is on every calendar.
1. Write the timeline backwards from the first conference day: list the final date, then what must be finished before it, then before that. Done when every workstream has dated milestones.
1. Copy the Conference Committee's month-by-month planning schedule (S004) into your tracker as dated issues, one per task, each with an owner. Done when every row of the schedule has a date or a reason it does not apply.
1. If you need Foundation funds, send the request before the board drafts its budget in December (L-4051).
1. Fix the dates and check them against major religious and national holidays (L-4073). Done when the dates are in the bid and confirmed with the venue.

### From T-9m to T-3m

1. Add slack for people you depend on. Vendors need follow-ups and much takes longer than planned (L-3074).
1. Review funding deadlines against the funder's own rules. The schedule's own funding line is inconsistent for a September conference, as the thin marker below shows.
1. Record actual dates against planned dates in the tracker each month. Done when the tracker shows where the plan slipped.

### From T-3m to the conference

1. Set a program freeze, a headcount freeze and a print-and-order freeze before the final operational rehearsal. Tie each freeze to the downstream commitments it locks, so late changes have a visible cost and owner (L-5047).
1. Schedule the final rehearsal after the last freeze. Done when the date is in the calendar and nobody can change the locked lists without naming the owner of the cost.

### After the conference

1. Deliver the actual milestone dates to the next team with the post-mortem. See [Handover contract](handover-contract.md).

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S009 | ledger: L-1009, L-1010 | confidence: observed | status: active | basis: structural | reason: Venues, suppliers and funders set their own lead times, so a late start removes choices.

Start the planning process early.
Starting late is one of the biggest mistakes an organizer can make.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S034 | ledger: L-3073 | confidence: observed | status: active | basis: structural | reason: Much conference work waits on people outside the team whose response time the team cannot control.

A plan of month-themed milestones in the software style does not fit conference work alone.
Add slack and follow-up time for the people the work depends on.
```

## Case notes

```{note} [specific · 2022 · Namur · 4 y]
:class: hb-lesson hb-specific hb-age-mid
lesson | scope: specific | year: 2022 | place: Namur | org: iMio and Affinitic | source: S067 | ledger: L-4175 | confidence: observed | status: active

For an October conference the website opened in May, the call for papers and ticket sales in June, venue information in August and the schedule in September.
The runway was compressed compared with a year-long plan.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2070 | confidence: observed | status: active

Preparation started about a year ahead with the venue search.
The venue confirmed availability within ten days, the bid was won about nine months before the event and the website went live about five weeks after that.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S034 | ledger: L-3071 | confidence: observed | status: active

The bid was accepted in early March and planning started the next day.
The conference took place in November, about eight months later.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S034 | ledger: L-3074 | confidence: observed | status: active

Just about everything took five times longer than expected.
Vendors needed pressure and many follow-ups.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1011 | confidence: observed | status: active

The conference ran from first idea to event in about six months.
The venue was reserved in mid-May, registration opened in mid-July after a three-week call for proposals, and print was ordered in early October.
```

## Risks

```{warning} Planning starts too late for venue and supplier lead times
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Hold the initial meeting by November or December of the preceding year and start the venue search about a year ahead | owner-role: team lead

Judged for a mid-size conference with an in-person venue.
A compressed runway has worked, but it leaves no room for a failed venue search.
```

```{warning} A funding request misses the Foundation's budget cycle
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Ask for Foundation funds before the board budget is drafted in December and confirm the cycle with the board | owner-role: treasurer

The cycle comes from one policy page and may have changed.
```

```{warning} Everything takes longer than planned
:class: hb-risk hb-likelihood-high hb-impact-medium
risk | likelihood: high | impact: medium | mitigation: Add slack to every dependency on outside parties and review planned against actual dates every month | owner-role: team lead

Suppliers and volunteers answer on their own time, and the plan has to carry that delay.
```

```{warning} Late changes after a freeze cause hidden costs
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Tie each freeze to the commitments it locks and name an owner for the cost of any later change | owner-role: team lead

Print orders and headcount commitments cannot be undone for free after the freeze.
```

## Thin content

```{warning} The planning schedule contradicts itself on funding dates
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A reconciled funding timeline that says which funder deadlines apply and when requests must be filed for a September conference | who-might-know: Conference Committee; Plone Foundation Treasurer role | area: other

The Committee's planning schedule (S004) asks for funding applications eight weeks before the event and recommends early June.
For a September conference those two dates fall in different months.
```

```{warning} Bid timeline after 2020
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: The Foundation's current bid dates and the season rule for conferences, since no hosting call after 2020 was located | who-might-know: Plone Foundation Board; Conference Committee | area: other

The season rule that the conference is held between mid-September and mid-November comes from calls up to 2020 and could not be verified.
The live schedule says only that the conference is held in the fall.
```

```{warning} The freeze pattern rests on one conference
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second conference's account of how it froze program, headcount and print, and what late changes cost | who-might-know: Past organizers; print and merchandise leads | area: other

No other source describes the freeze dates or their effect.
```

```{warning} No account of a compressed runway that failed
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Accounts of a conference that planned on a runway of under six months and what it dropped | who-might-know: Past organizers of the shortest schedules; Conference Committee | area: other

The two short schedules in the case notes both worked.
Nothing records what such a plan costs when it fails.
```

## Sources and further reading

- S004 Plone Conference Committee, "Conference Planning Schedule", live page (read as of 2026-11-02).
- S005 Plone Foundation, "Plone Event and Sprint Sponsorship Policy".
- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
- S034 San Francisco 2011, organizer interview.
- S036 Arnhem 2012, organizer wrap-up account.
- S049 Foundation call for proposals, 2016.
- S067 Namur 2022, official record with timeline.
