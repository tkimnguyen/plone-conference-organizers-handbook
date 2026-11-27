---
steward: unassigned
deputy: unassigned
review-by: 2027-11-02
maturity: stub
applies-to: [jurisdiction]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How a Plone conference handles attendee data, photo consent and sponsor contact sharing, with EU data protection law as the reference point."
    "keywords": "Plone, Plone Conference, privacy, GDPR, consent, photographs, attendee data"
---

# Privacy and GDPR

## Why it matters

This chapter is general information, not legal advice.
Check current rules with a qualified local adviser.

A conference collects names, e-mail addresses, dietary needs, payment details, travel documents and photographs.
Different teams hold the data in different years, in ticket platforms, mailing lists, spreadsheets and chat tools.
When a team hands over to the next one, the lists often go with it.

EU data protection law applies to many Plone conferences, and its rules were different when the early accounts in this handbook were written.
Mistakes cost trust first, and fines are a risk when a team shares data without a lawful basis.
The steps are in the How-to section.

## Applies when

- `jurisdiction` Data protection rules depend on where the organizer is established and where attendees live, and EU rules are the reference point here.

## Decisions you must make

- {bdg-secondary}`OPTION` **Will the website and the ticket flow collect an agreement to be photographed?** The Foundation's planning schedule lists it twice (R-014, S004). Legal sufficiency under data protection law is a separate question for counsel. (decide-by: T-6m)
- {bdg-secondary}`OPTION` **Will you share attendee contact data with sponsors?** If you do, ask for opt-in consent and say with whom you share (L-1042). One conference wanted to share and had no permission mechanism in time (L-1041). (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Who answers privacy questions and deletion requests?** Name a role and publish a role address on the site. (decide-by: T-6m)
- {bdg-secondary}`OPTION` **What happens to attendee, speaker and volunteer lists after the conference?** Decide retention and handover with an adviser, because a list is personal data. (decide-by: T-3m)

## How-to

1. List every kind of personal data you collect and where it lives: registration, per-attendee e-mail, volunteer and speaker lists, visa letter requests, photographs and surveys.
   Done when each item has an owner and a tool.
1. Ask an adviser which lawful basis fits each item and which tools process the data for you.
   Done when the answer is written down.
1. Write the registration notice: what you collect, why, how long you keep it and who receives it.
   Done when the notice appears before the buyer pays.
1. Add the photo agreement to the website and the ticket flow, as the planning schedule lists it (S004).
   Done when a test purchase shows the agreement.
1. Share attendee contact data with sponsors only after documented opt-in consent (L-1042).
   Done when the consent record exists for every shared contact.
1. Decide what to delete, archive or hand over when the conference ends, and tell the next team what they may keep.
   Done when the decision is in the decision log.

## Principles and general lessons

No general lesson has passed the promotion rule yet.

## Case notes

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1041, L-1042 | confidence: observed | status: active

The organizers wished they had offered registrant contact data to top sponsors, and had no permission mechanism in time.
They recommended a notice naming the recipients, with an opt-out checkbox.
Under EU data protection law as of 2026-11, sharing with sponsors needs opt-in consent instead.
```

## Risks

```{warning} Attendee data is shared without a lawful basis
:class: hb-risk hb-likelihood-low hb-impact-high
risk | likelihood: low | impact: high | mitigation: Share contact data only with documented opt-in consent and record who received it | owner-role: privacy lead

Sponsors ask for contact lists as a benefit.
```

```{warning} Lists pass to the next team without a basis
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Agree with an adviser what may be handed over and delete the rest at the end of the conference | owner-role: privacy lead

Judged for a conference with a rotating team.
```

```{warning} The photo agreement is judged insufficient
:class: hb-risk hb-likelihood-low hb-impact-medium
risk | likelihood: low | impact: medium | mitigation: Ask counsel to review the wording and give attendees a way to say they do not want to be photographed | owner-role: privacy lead

The Foundation's schedule lists the agreement and does not rule on its legal sufficiency.
```

## Thin content

```{warning} Counsel-reviewed consent wording
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Wording for registration notices and photo agreements reviewed by counsel | who-might-know: Foundation counsel; data protection advisers

No located source gives reviewed wording.
```

```{warning} Handover of lists between organizers
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: A reviewed practice for what mailing lists and volunteer lists may pass to the next team | who-might-know: Past organizers; data protection advisers

No located source records how the lists passed between organizers.
```

```{warning} Sponsor data sharing
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: A second account of sponsor contact sharing and the consent used | who-might-know: Sponsor owners of past conferences

One conference reports the practice, and its recommendation predates EU rules on consent.
```

```{warning} Privacy law outside the EU
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Dated notes on privacy rules for hosts outside the EU | who-might-know: Past organizers in the United States, Brazil and Japan | area: non-eu-legal-tax-visa

The handbook holds no account from such a host.
```

## Sources and further reading

- S004 Plone Foundation, Conference Planning Schedule.
- S009 Seattle 2006, "Things We Learned About Running a Plone Conference".
