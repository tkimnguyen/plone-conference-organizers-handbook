---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to choose keynotes and invited speakers, approach them without a speaker-fee budget and place them in the program."
    "keywords": "Plone, Plone Conference, keynotes, invited speakers, program"
---

# Keynotes and invited talks

## Why it matters

Keynotes set the tone of the conference and are the sessions the whole audience shares.
Invited talks fill the gaps an open call does not, such as evergreen teaching, a roadmap voice or a perspective from outside the community.

A team with no budget for speaker fees and few outside contacts tends to plan only the usual community keynotes.
That keeps the conference inward-looking and leaves the opening and closing slots to chance.

Foundation support, community tradition and sponsor expectations all touch this chapter.
See `community-and-speaker-expectations` for the State of Plone tradition and `speakers-and-speaker-care` for what a speaker can expect.
Invitations take weeks, so the decisions below come before the open call closes.

## Applies when

- `all` Every conference has opening and closing slots that someone has to fill.

## Decisions you must make

- {bdg-primary}`DEFAULT` (basis: L-1098, L-2014, L-4203) **Will at least one keynote come from outside the Plone community?**
  Outside keynotes became highlights at several conferences, and survey respondents valued some that were slightly off-topic.
  Check candidates by watching earlier talks online before inviting.
  (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Who delivers the State of Plone talk, and is it a keynote?**
  The community has a tradition on this; see `community-and-speaker-expectations`.
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **How many keynotes does the program carry?**
  Pick the number from the program goals, because each keynote takes the shared slot and the main room.
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Will you invite sessions beyond keynotes?**
  One team built a wish list with preferred speakers, approached about a dozen people and filled three tutorials, four talks and the panels within two weeks (L-1062).
  (decide-by: T-6m)
- {bdg-secondary}`OPTION` **What can you offer invited speakers without a fee budget?**
  An invitation letter from the Foundation was enough for one outside keynote (L-1098).
  Settle ticket, travel and fee terms before approaching anyone.
  (decide-by: T-6m)

## How-to

1. Write a ranked wish list of sessions and preferred speakers from the gaps found in [Programme portfolio](programme-portfolio.md).
   Done: a list with one line of reasoning per name.
2. Ask a well-connected community member for introductions to speakers outside the community.
   Done: introductions logged.
3. Watch earlier recordings of each candidate.
   Done: a one-line note per candidate.
4. Settle what the conference can offer: ticket, travel, fee and an invitation letter.
   Done: a written offer. See `speakers-and-speaker-care` and `visas-and-travel`.
5. Send the invitations, with a response date.
   The Foundation planning schedule places keynote speakers, the call for talks and the call for trainers in April (L-4036; S004, as of 2026-11).
   Done: every invitation has an answer or a follow-up date.
6. Place keynotes in the grid first, following [Scheduling](scheduling.md).
   Done: opening and closing slots are filled.
7. Agree a replacement route for each keynote, using the `speaker-dropout` playbook.
   Done: a named fallback per slot.
8. Publish the keynotes with an abstract and a biography that the speaker has checked.
   Done: the speaker has confirmed the text.

## Principles and general lessons

No general lesson has passed the promotion rule yet.
One piece of advice rests on a single conference and is tracked here until independent evidence arrives:

- Attendees asked for a strong opening keynote to set the mood, and for community leaders to frame the larger vision at the start or close (L-1099, S087).

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S110 | ledger: L-6039 | confidence: reported | status: active

The content mix drew an unresolved disagreement: one respondent asked to keep mind-broadening keynotes, another to stop keynotes unrelated to IT and a third to stop talks involving AI.
```

```{note} [specific · 2024 · Brasília · 2 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2024 | place: Brasília | org: Plone Conference 2024 organizing team | source: S074 | ledger: L-4203 | confidence: reported | status: active

Keynotes and talks averaged 4.4 out of 5 in the attendee survey, and some respondents valued slightly off-topic keynotes.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S015 | ledger: L-2014 | confidence: observed | status: active

Instead of the usual software-freedom keynote, the organizers invited an engineering-project leader whose struggle with an established industry paralleled open source. They chose the speaker after watching earlier talks online, and the audience responded strongly.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1062 | confidence: observed | status: active

The organizers brainstormed a wish list of sessions with preferred speakers and approached about a dozen people. Almost all agreed, and within two weeks three tutorials, four talks and the case-study panels were invited.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1098 | confidence: observed | status: active

With no budget for speaker fees and no strong connections, the organizers had planned only the usual community keynotes. An outside keynote came through a community member's contact, needed only an invitation letter from the Foundation, and became a highlight.
```

## Risks

```{warning} An invited keynote cancels close to the conference
:class: hb-risk hb-likelihood-low hb-impact-high
risk | likelihood: low | impact: high | mitigation: Agree a replacement route in advance, such as a community keynote or a panel that can fill the slot | owner-role: program lead | playbook: speaker-dropout

Judgment holds for a typical mid-size conference.
```

```{warning} A keynote candidate expects fees or travel the budget cannot meet
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Settle what the conference can offer, including an invitation letter, before approaching candidates | owner-role: program lead


```

## Thin content

```{warning} Approaching speakers without a fee budget
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Accounts from other conferences of recruiting outside keynotes with no speaker-fee budget | who-might-know: Past program chairs; Foundation Conference Committee

The only detailed account is one conference.
```

```{warning} Keynotes for remote and hybrid audiences
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Evidence on keynote format for remote attendees, including slot length and time zone | who-might-know: Organizers of online and hybrid conferences | area: hybrid-online

No archived source covers keynote choices for remote audiences.
```

```{warning} Keynote evidence is mostly old
:class: hb-thin hb-thin-stale
thin | kind: stale | needs: Attendee survey data on keynote reception from conferences within the last eight years | who-might-know: Past survey owners

Three of the four case notes come from conferences more than eight years before the 2026 pin.
```

## Sources and further reading

- S004 Conference Planning Schedule.
- S009 Things We Learned About Running a Plone Conference.
- S015 Plone Conference 2010: An Organiser's View.
- S074 Results from the 2024 Conference feedback survey.
- S087 Seattle 2006 agenda suggestions.
- S110 Maastricht 2026 attendee survey analysis.
