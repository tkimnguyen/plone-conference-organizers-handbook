---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How a Plone conference publishes the Code of Conduct, makes participants agree to it and gets a response contact in front of everyone."
    "keywords": "Plone, Plone Conference, Code of Conduct, response team, reporting"
---

# Code of Conduct operations

## Why it matters

A Code of Conduct on paper protects nobody until participants know it exists, have agreed to it and know whom to tell when something goes wrong.
The Foundation expects every Plone conference to adhere to the Plone Code of Conduct.
Sponsors and partner organizations may also make it a condition of their support.

Without a reachable response contact, a participant who feels unsafe has no step to take.
Volunteers who receive a report without a procedure either improvise or do nothing, and both damage trust in the whole event.

This chapter covers the operational side: publication, agreement, the response contact and the briefing.
It does not restate the incident steps, which belong in the Part 3 playbook for a Code of Conduct incident.
The wider work of preparing the volunteers who may receive a report is in [Volunteers and roles](volunteers-and-roles.md).

## Applies when

- `all` Every Plone conference adheres to the Code of Conduct, in person, hybrid or online.

## Decisions you must make

- {bdg-danger}`MUST` (req: R-013; as-of: 2026-11-02) **Does the website publish the Plone Code of Conduct, and does every ticket buyer agree to abide by it?** Put the code on the conference website and in the ticketing agreement. (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-3102, L-4135) **How do you make the code binding and visible to every participant group?** Extend the acknowledgement to speakers and exhibitors, and open the pre-arrival briefing with the response contact and the emergency number. (decide-by: T-3m)
- {bdg-secondary}`OPTION` **Who staffs the response team, and how many people does it need?** Choose people who are not also running the registration desk or the main stage. Size and composition depend on the conference. (decide-by: T-3m)
- {bdg-secondary}`OPTION` **Which reporting channels do you offer?** A monitored email address, an in-person contact and a named backup are common. No located source compares channels. (decide-by: T-3m)

## How-to

1. Publish the Plone Code of Conduct on the conference website, linked from the footer and from the registration page. Done when the link works from every page of the ticket flow.
1. Add the agreement to ticketing, so a buyer cannot complete checkout without accepting it. Done when a test purchase shows the agreement before payment.
1. Add the acknowledgement to the speaker and sponsor or exhibitor agreements. Done when each template carries the same wording as the ticket flow.
1. Name the response team and one contact route that is monitored during the whole conference. Done when two people can confirm they will answer.
1. Put the response contact and the local emergency number at the top of the pre-arrival briefing, before logistics.
1. Brief volunteers and staff on what to do when a report reaches them: listen, write down what was said, pass it to the response team, and do not investigate. Done when each volunteer can name the route.
1. Agree before the event where incident records are kept and who may read them. Done when the answer is written in the team's private files, not in public material.
1. Rehearse the first hour with the Part 3 playbook for a Code of Conduct incident. Done when the response team has walked through one example case.

## Principles and general lessons

No general lesson has passed the promotion rule yet.

## Case notes

```{note} [specific · 2016 · Boston · 10 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2016 | place: Boston | org: Plone Foundation | source: S051 | ledger: L-4135 | confidence: observed | status: active

The pre-arrival briefing for attendees put the Code of Conduct response contact and the emergency number at the top.
```

```{note} [specific · 2013 · Brasília · 13 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2013 | place: Brasília | org: PloneGov-BR and APyB | source: S093 | ledger: L-3102 | confidence: observed | status: active

Acknowledging the code was mandatory for attendees, speakers and exhibitors for the first time.
The Python Software Foundation required it as a condition of its sponsorship.
```

## Risks

```{warning} A report reaches a team with no agreed procedure
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Name the response team and rehearse the first hour before the conference opens | owner-role: Code of Conduct response lead | playbook: coc-incident

Volunteers improvise, the reporter loses confidence, and the team has no record of what was decided.
Judged for a mid-size conference.
```

```{warning} The code is published but missing from ticketing
:class: hb-risk hb-likelihood-low hb-impact-medium
risk | likelihood: low | impact: medium | mitigation: Complete a test purchase as a buyer before sales open and check that the agreement appears before payment | owner-role: ticketing lead

The Foundation expects the agreement in the ticketing flow, and a gap there is easy to miss.
```

```{warning} The response contact is the same person who runs the venue
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Assign response duties to people without a fixed on-site operations post and name a backup | owner-role: conference chair | playbook: key-person-loss

A contact who is busy on stage or at the desk cannot take a report in time.
```

## Thin content

```{warning} Incident handling procedure
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Anonymized accounts of how past response teams received, triaged, decided and recorded reports | who-might-know: Past response team members; the Foundation's Code of Conduct contacts | area: other

No located source describes an actual incident or the decision steps of a response team.
```

```{warning} Training and independence of the response team
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Practice on how responders are chosen, briefed and kept independent of the organizing team | who-might-know: Foundation Code of Conduct contacts; organizers of other open source conferences | area: other

The chapter names the roles but gives no evidence for team size or training.
```

```{warning} Online and hybrid reporting
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Reporting routes and moderation practice for chat channels and streamed sessions | who-might-know: Organizers of online and hybrid Plone conferences; community moderators | area: hybrid-online

No located source covers reports that arise in chat rooms or video sessions.
```

## Sources and further reading

- S004 Plone Foundation, Conference Planning Schedule (the Committee schedule that lists the code on the website and in the ticketing agreement).
- S049 Plone Foundation, 2016 call for proposals (codified requirements).
- S052 Plone Foundation, 2017 call for proposals.
- S051 Boston 2016, detailed attendee logistics.
- S093 Brasília 2013, PythonBrasil organizer manual, operational record.
