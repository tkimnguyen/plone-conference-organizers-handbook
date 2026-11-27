---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to build an organizing team, name its roles, keep one tracker as the source of truth and stay within the Foundation's naming rules."
    "keywords": "Plone, Plone Conference, organizing team, governance, roles, issue board"
---

# Team and governance

## Why it matters

A Plone conference is run by a small group that also has other jobs.
The work is wide: money, venue, program, suppliers, volunteers, communication.
When the group is thin or its work is invisible, things are dropped without anyone deciding to drop them.

Three parties share the weight.
The Foundation approves the name and the location and, when asked, backs the money.
The Conference Committee, made up of past organizers, offers continuity.
The host body, whether a company or a volunteer group, supplies the people.
The conference competes with that host's daily work, and the host loses more than it plans for.

Without a written team, a named owner for each area and one place where all work is tracked, the team cannot tell finished work from forgotten work.
The cost shows up as late program publication, unclear contacts for sponsors and attendees, and a burned-out core.
Handing the work to the next team (see [Handover contract](handover-contract.md)) is only possible if the work was visible in the first place.

## Applies when

- `all` Every Plone conference has an organizing team, whatever its size, host body or country.

## Decisions you must make

- {bdg-danger}`MUST` (req: R-001; as-of: 2026-11-02) **Has the Foundation approved the event name and the location?** An event may carry the name "Plone Conference" and a year, or "International Plone Conference", only with the Foundation's approval, and the Foundation selects the location. Record the approval before any public announcement. (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-2056, L-2117, L-4066) **Who leads, who owns each functional area, and is the team big enough for the routine work?** Name a lead and one owner per area, and count the helpers who will do the routine work before and during the conference, not only the named leads. Publish the role split so sponsors and attendees know whom to contact. (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-2013, L-2073) **If a company hosts, how much staff time is reserved for the conference, and which business work is deferred?** Two company hosts found that the conference competed with running the business. Write the reserved time and the deferred work down before the bid. (decide-by: T-12m)
- {bdg-secondary}`OPTION` **Will all work live on one issue board?** One conference kept every task on a single board and treated it as the source of truth, and found a partial board useless for that purpose (L-5031). The evidence comes from one conference, so adopt it by judgment. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Flat task list or hierarchy of epics?** For a small team, consider a flat list with clear titles and regular triage, and add hierarchy only when the team can maintain it (L-5042). (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will the team hold a short stand-up after each conference day?** One host reviewed each day's problems that evening and fixed them for the next day (L-2092). (decide-by: T-1m)

## How-to

### Before the conference

1. Ask the Foundation to confirm the name and the location, and keep the answer with the team's records. Done when a dated written approval exists.
1. Write the roster: one lead and one owner for every functional area, each with a named deputy. Done when no area has an empty owner field.
1. Publish the role split, one owner per area, on the conference site. Done when a sponsor can find the right contact without asking (L-2117).
1. Put every task on one board as an issue with a clear title, an owner and a date. Done when nothing is tracked only in chat or in private lists.
1. Turn every MUST item of the handbook into an explicit completion gate on the board. Give optional local activation work and research an owner and a drop-by date in the Tailoring Record, so capacity decisions stay visible (L-5038).
1. Reserve capacity for tracker maintenance before on-site preparation speeds up. Done when someone owns the weekly triage in the last planning phase (L-5032).

### While planning

1. Close completed work as it happens and triage the queue every week through the final planning phase (L-5032).
1. Review the roster at each team meeting. When a role has been dropped or doubled, say so out loud and record it.

### After the conference

1. Close every issue whose work was done and give every unfinished issue a dated disposition: done, dropped with a reason, or handed over. Done when the open list means what it says.
1. Hand the roster, the board and the Tailoring Record to the next team. See [Handover contract](handover-contract.md).

## Principles and general lessons

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S015, S049 | ledger: L-2018, L-4066 | confidence: observed | status: active | basis: structural | reason: Conference work runs in parallel across money, suppliers and venue, so named leads alone cannot cover it.

A successful conference rests on planning and well coordinated teamwork.
Bid teams are asked whether they have enough people for the routine work before and during the conference, not only named leads.
```

```{note} [general]
:class: hb-lesson hb-general
lesson | scope: general | source: S098 | ledger: L-5031 | confidence: observed | status: active | basis: structural | reason: A tracker that omits some work cannot show what is open, whatever the tool.

Keep all conference work visible on one issue board.
A partial board cannot serve as the team's operational source of truth.
```

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6018 | confidence: observed | status: active

Organizing and logistics averaged 4.62 of 5 in the attendee survey, with fourteen top scores and a single 3 among 21 ratings.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5033 | confidence: reported | status: active

Completed on-site work stayed recorded as open after the conference.
Issue state could not tell unfinished work from missing closure.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5039 | confidence: reported | status: active

A proposed documentation toolchain never started.
A folder of Markdown files became the working organizing archive instead.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5041 | confidence: reported | status: active

The team stopped maintaining its epic layer and kept working in small focused issues.
The hierarchy added a coordination layer that this team did not sustain.
```

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6019 | confidence: reported | status: active

A respondent's keep-doing item was organizer approachability: the organizers were only an email away.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2073 | confidence: observed | status: active

The host company estimated more than 1,750 hours of organizing work.
Twelve of its staff worked full time during the conference days.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2092 | confidence: observed | status: active

The organizing team held a stand-up after each conference day.
It reviewed what to improve for the next day.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S037 | ledger: L-2110 | confidence: observed | status: active

The host company formed its task force while writing the bid.
It kept the main tasks in house and expected extra helpers to join later.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S037 | ledger: L-2117 | confidence: observed | status: active

The team published its role split, with one owner per functional area.
Attendees and sponsors knew whom to contact for which topic.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S034 | ledger: L-3072 | confidence: observed | status: active

Only two coordinators ran the conference.
They relied on two creative helpers for design and on the volunteer team during the event.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S015 | ledger: L-2013 | confidence: observed | status: active

Organizing as a company meant the conference competed with running the business.
Publishing the program fell behind schedule for that reason.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S017 | ledger: L-2047 | confidence: observed | status: active

Inside the host company, one colleague handled the hotel and all suppliers.
Another supported the Wi-Fi specialist, next to the lead organizer.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S019 | ledger: L-2056 | confidence: observed | status: active

The bid named four staff of the host company: a lead, an operations director in charge of finances, a business developer and an administration manager.
The last two spent most of their time on the event.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1006 | confidence: observed | status: active

Two staff of the host organization ran the conference as a project.
A colleague handled the money, another handled logistics, and staff of a partner nonprofit helped during conference week.
Organizing took over 350 staff hours.
```

## Risks

```{warning} A key organizer becomes unavailable
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Name a deputy for every area and keep the roster and the board current, so any area can be picked up by a second person | owner-role: lead organizer | playbook: key-person-loss

Small teams concentrate knowledge in two or three people.
When one of them falls ill or leaves, the work they held is invisible to everyone else.
```

```{warning} Conference work crowds out the host's own business
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Reserve named staff time and defer named business work in writing before the bid | owner-role: host company lead

Judged for a company host of medium size.
A volunteer host faces the same pressure from day jobs.
```

```{warning} The tracker no longer matches reality
:class: hb-risk hb-likelihood-high hb-impact-medium
risk | likelihood: high | impact: medium | mitigation: Close work as it is finished, triage weekly and give one person ownership of tracker maintenance in the last planning phase | owner-role: team lead

Stale issue state hides both finished work and forgotten work.
```

```{warning} Planned work is dropped without a decision
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Give every optional item an owner and a drop-by date in the Tailoring Record, and record a dated disposition when it is dropped | owner-role: team lead

Optional work that nobody owns fades away, and the team learns it was dropped only when the result is missing.
```

## Thin content

```{warning} Current bid and selection process
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: The Foundation's current process for receiving, qualifying and awarding hosting bids, including who must be named in a bid | who-might-know: Plone Foundation Board; Conference Committee; recent organizing teams | area: other

The archived process comes from calls for proposals up to 2020.
No later call was located, so the register rows on bid submission and on naming key people stay unverified.
```

```{warning} The issue board method rests on one conference
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Accounts from a second conference of how it kept all work on one board, and whether the close-as-you-go habit held | who-might-know: Teams that ran a shared tracker; Conference Committee | area: other

The board practice, the flat list and the completion gates all come from one organizing team.
```

```{warning} Team size and hours against conference size
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Comparable team sizes and staff hours from conferences of different attendance, to say what a small, medium or large conference needs | who-might-know: Past lead organizers; host company finance staff | area: other

Hours and team sizes exist for individual conferences but not in a comparable form.
```

## Sources and further reading

- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
- S015 Bristol 2010, host company blog, "An Organiser's View".
- S017 Bristol 2010, host company blog, "Wrapup".
- S019 Bristol 2010, official conference record and original proposal.
- S034 San Francisco 2011, organizer interview.
- S036 Arnhem 2012, organizer wrap-up account.
- S037 Arnhem 2012, organizing team and responsibilities.
- S049 Foundation call for proposals, 2016.
- S098 Maastricht 2026, facts and lessons for the handbook.
- S099 Maastricht 2026, GitHub issues and project board collaboration review.
- S110 Maastricht 2026 attendee survey analysis.
