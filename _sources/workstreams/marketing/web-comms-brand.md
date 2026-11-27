---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: mixed
myst:
  html_meta:
    "description lang=en": "How to run the website, email, social accounts and visual identity of a Plone Conference, including the naming rules and a quality gate."
    "keywords": "Plone, Plone Conference, website, email campaigns, brand, naming"
---

# Web, comms and brand

## Why it matters

For most people the conference is its website until they arrive.
Attendees look for the schedule and the hotel list there, sponsors check how their logo appears, and speakers check their own listing.
A site that is late, unclear or untested turns every question into an email to the organizers.

Public communication also carries rules.
The Foundation controls the use of the conference name and the claim of endorsement, and funded activities must say so.
Breaking these rules costs trust with the Foundation, and fixing a published mistake costs more than avoiding it.

The accounts, domains and mailing lists outlive each team.
A successor can only build on what was handed over, so a conference that keeps its assets in one person's name leaves the next team to start again.

Audience planning and outreach sit in [Marketing and outreach](marketing-and-outreach.md).
This chapter owns the website quality risk below, which has a direct effect on sales and on the first day.

## Applies when

- `all` Applies to every Plone conference, because every conference has a name, a site and a way of writing to its people.

## Decisions you must make

- {bdg-danger}`MUST` (req: R-001; as-of: 2026-11-02) **Has the Foundation approved the event name?** Only an approved event may be called "Plone Conference" with a year or "International Plone Conference". Get the approval in writing before public use. (decide-by: T-12m)
- {bdg-danger}`MUST` (req: R-002; as-of: 2026-11-02) **Does every public message present the event as primarily about Plone and avoid implying Foundation endorsement that the Foundation did not give?** Check site, emails, banners and sponsor material against the naming guidelines. (decide-by: T-12m)
- {bdg-danger}`MUST` (req: R-030; as-of: 2026-11-02) **Is any activity funded by the Foundation, and does each of its communications say so?** The rule applies only to Foundation-funded activities, for example a funded sprint. (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-3047, L-3123) **Which domain and accounts carry over from year to year, and who holds them?** Create accounts without the year in the name, record registrar, DNS host and owner role, and plan the transfer. (decide-by: T-12m)
- {bdg-primary}`DEFAULT` (basis: L-2074, L-4027) **When does the website launch, and what must it carry on the first day?** Launch with venue, hotels, registration and the code of conduct, and revise as questions arrive. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will the website and ticketing collect the attendee's agreement to be photographed?** The Foundation schedule asks for it (requirements register row R-014, as of 2026-11-02). The register proposes a DEFAULT, but only one source backs it, so it stays an OPTION. Counsel decides whether a notice suffices under privacy law. (decide-by: T-9m)
- {bdg-secondary}`OPTION` **Will one designer own the whole visual identity?** One designer gave a single look across logo, badges, posters and site. (decide-by: T-9m)
- {bdg-primary}`DEFAULT` (basis: L-1130, L-3079) **Which page is the one definitive web source, and does it include an FAQ?** Every email points back to it, and an early FAQ is estimated to cut incoming email. (decide-by: T-8m)
- {bdg-primary}`DEFAULT` (basis: L-2081, L-4134) **Will attendees get a mobile agenda?** Both app guides were used and could be updated, but filling them took effort. (decide-by: T-6m)
- {bdg-primary}`DEFAULT` (basis: L-3036, L-5045) **Which date freezes the website for quality assurance, and who tests the core attendee tasks?** Attendee-facing schedule problems surfaced late in both accounts. (decide-by: T-8w)

## How-to

### Foundations (T-12m to T-9m)

1. Request the Foundation's approval of the event name and file it. Done: the approval is in the shared folder.
2. Create the conference domain and accounts under year-free names. Done: an inventory lists each account, domain, DNS host, owner role and renewal date.
3. Fix the brand basics: logo, imagery, website theme, shirt and signage (L-4027, S004). Done: one brand kit holds logo files, colors and fonts with a system-font fallback.
4. Write the funded-by line for any Foundation-funded activity. Done: the line is part of every template for that activity.

### Website (T-9m to T-1w)

5. Launch the website with venue, hotels, registration and the code of conduct, and include the photo-consent notice if you decided to collect it (L-4027). Done: the launch checklist is signed off.
6. Publish an FAQ page early and link it from the home page and every email (L-3079, S034). Done: the FAQ is live.
7. Make one page the definitive source and point every email back to it. Done: no email carries facts that the page lacks.
8. Set the quality gate date several weeks before day one and test as an attendee (L-5046, S099). Cover finding a talk by speaker name, filtering by day and reading the venue directions. Done: a test log lists each task, tester and fix, and the site is frozen on the gate date.

### Email and social (T-6m to T-0)

9. Keep each campaign's source, generated HTML and matching plain-text fallback together, and recompile after source changes instead of editing generated HTML (L-5064, S107). Done: each campaign folder has all three files and the plain text matches the source.
10. Preview every campaign with a credential-free dry run and give sending credentials through the environment (L-5065, S107). Done: a second person reviewed the dry run and a send without credentials fails clearly.
11. Keep an attendee list announce-only before the event, open it for discussion during the event, and return it to announce-only afterward for follow-up and surveys. Done: list settings changed on the planned dates.

### After the event

12. Publish a report news item that lists participants, thanks sponsors and links a curated photo folder (L-4052, S005). Done: the item is live. The Foundation's marketing team helps authors who write less confidently in English.
13. Publish the recordings and announce them on social media and by newsletter. Done: every talk has a public link.
14. Archive the year's site under a year address and keep the current year on the main domain. Done: an owner and a date are recorded.

## Principles and general lessons

No general lesson has passed the promotion rule yet.
Two suggestions rest on one account each and stay candidates.
Attendees praised the attendee mailing list and the wiki and asked that they become standard, and one asked that the wiki be frozen and archived afterward (L-1132).
An organizer advised using a mobile event app because it is easy to update and attendees like it (L-2106).

## Case notes

```{note} [specific · 2026 · Maastricht · 0 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2026 | place: Maastricht | org: Plone Conference 2026 organizing team | source: S099 | ledger: L-5045 | confidence: reported | status: active

A critical schedule-search defect was reported the day before the conference.
Search did not find speaker names or filter by day, so a core attendee task stayed untested until the last preparation window.
```

```{note} [specific · 2025 · Jyväskylä · 1 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2025 | place: Jyväskylä | org: University of Jyväskylä | source: S079 | ledger: L-4221 | confidence: reported | status: active

A photo competition during the event produced a shared set of conference pictures.
```

```{note} [specific · 2023 · Eibar · 3 y]
:class: hb-lesson hb-specific hb-age-recent
lesson | scope: specific | year: 2023 | place: Eibar | org: CodeSyntax | source: S070 | ledger: L-4187 | confidence: reported | status: active

Publishing the videos and announcing them on social media was well received.
```

```{note} [specific · 2016 · Boston · 10 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2016 | place: Boston | org: Plone Foundation | source: S051 | ledger: L-4134 | confidence: observed | status: active

A mobile guide app carried the schedule, speaker information and FAQs, and updated automatically.
```

```{note} [specific · 2014 · Bristol · 12 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2014 | place: Bristol | org: Netsight | source: S043 | ledger: L-4110 | confidence: reported | status: active

After the conference the communications team sent a special-edition newsletter collecting videos of all talks and keynotes, slides and notes.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2074 | confidence: observed | status: active

Launching the website early, with hotels, venue information and registration, let the team update information quickly as questions came in.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2081 | confidence: observed | status: active

A third-party mobile event app, chosen after comparing several, took considerable effort to fill with talks and speakers.
Most attendees used it.
```

```{note} [specific · 2012 · Arnhem · 14 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2012 | place: Arnhem | org: Four Digits | source: S036 | ledger: L-2109 | confidence: observed | status: active

One external designer produced the logo, badges, flyers, posters, award items and website design, giving the event a single visual identity.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S028 | ledger: L-3047 | confidence: observed | status: active

A social-network account was suspended because it had been created with the year in its name.
Conference accounts need names that can carry over from year to year.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S028 | ledger: L-3050 | confidence: observed | status: active

The team kept carefully maintained mailing lists segmented into speakers, attendees and sponsors, and told successors to start announcements there.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S031 | ledger: L-3062 | confidence: observed | status: active

The team planned to archive each year's site under a year subdomain and keep the current year on the main domain.
They did not finish it and offered to help the next team.
```

```{note} [specific · 2011 · San Francisco · 15 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2011 | place: San Francisco | org: Plone Conference 2011 organizing team | source: S031 | ledger: L-3064 | confidence: observed | status: active

The team published reusable site packages for successors: a content skeleton, a sponsor add-on and the site buildout, which needed maintenance.
```

```{note} [specific · 2010 · Bristol · 16 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2010 | place: Bristol | org: Netsight Internet Solutions | source: S015 | ledger: L-2005 | confidence: observed | status: active

The host company's designer insisted on a strong brand identity from the start, and a local illustrator was commissioned.
The website, treated as the main advertising channel, received significant development time.
```

```{note} [specific · 2008 · Washington, D.C. · 18 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2008 | place: Washington, D.C. | org: ZPUGDC | source: S012 | ledger: L-4098 | confidence: observed | status: active

Live coverage of the opening keynote could only start once the network was fixed.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1130 | confidence: observed | status: active

The conference pages on plone.org were the definitive public source.
Emails pointed back to them, pages went up as early as possible and were revised constantly, and announcements were also posted as news items for feeds.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1131 | confidence: observed | status: active

An attendee mailing list, filled as people registered, was announce-only before the event, opened for discussion during it and returned to announce-only afterward for follow-up and surveys.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1133 | confidence: observed | status: active

A short-lived wiki held attendee bios and impromptu events, and offered space for session notes, which were little used.
It was chosen because editing needed no account and was much faster.
```

```{note} [specific · 2006 · Seattle · 20 y] stale-prone
:class: hb-lesson hb-specific hb-age-old hb-stale-prone
lesson | scope: specific | year: 2006 | place: Seattle | org: ONE/Northwest | source: S009 | ledger: L-1134 | confidence: observed | status: active

A volunteer sent attendees shared tags for blog posts, photos and bookmarks, and a map of where attendees came from.
```

## Risks

```{warning} A critical website defect is found in the last days before the conference
:class: hb-risk hb-likelihood-medium hb-impact-high
risk | likelihood: medium | impact: high | mitigation: Hold a website quality gate several weeks before day one, test the core attendee tasks as an attendee, and freeze content after the fixes | owner-role: web lead | playbook: low-ticket-sales

Judged for a typical mid-size conference.
```

```{warning} Conference accounts or the domain are lost at the handover
:class: hb-risk hb-likelihood-medium hb-impact-medium
risk | likelihood: medium | impact: medium | mitigation: Use year-free account names, record every account, domain and DNS host with an owner role, and transfer ownership to the next team on a dated checklist | owner-role: web lead

A suspended account or an unclear domain owner stops the next team from building on the last.
```

```{warning} A public message breaks the naming or endorsement rules
:class: hb-risk hb-likelihood-low hb-impact-medium
risk | likelihood: low | impact: medium | mitigation: Get written name approval first and have one named person check every public template against the naming guidelines before first use | owner-role: communications lead

The rules are short, and a late correction means reissuing material that already circulated.
```

## Thin content

```{warning} Photo-consent practice has one source
:class: hb-thin hb-thin-single-source
thin | kind: single-source | needs: Photo-consent notices and policies from at least one more conference, with counsel's view of their sufficiency | who-might-know: Foundation legal adviser; past ticketing leads | area: other

The Foundation schedule is the only archived source for collecting photo consent.
```

```{warning} Accessibility of the website is not covered
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: Accessibility checks for the schedule, registration and mail templates, with the method used and the findings | who-might-know: Accessibility reviewers in the community; past web leads | area: accessibility

No archived account tests the conference site or emails for accessibility.
```

```{warning} Hybrid and online communication is not covered
:class: hb-thin hb-thin-gap
thin | kind: gap | needs: How to publish stream links, chat channels and remote schedules for a hybrid or online edition | who-might-know: Organizers of the online and hybrid editions | area: hybrid-online

Only live-coverage and video-publishing notes from in-person events are recorded here.
```

## Sources and further reading

- S004 Conference Planning Schedule, Plone Foundation conference team, plone.org.
- S005 Plone Event and Sprint Sponsorship Policy, Plone Foundation.
- S009 "Things We Learned About Running a Plone Conference", Seattle 2006 evaluation, plone.org.
- S012 Contemporary report noting the first-day Wi-Fi failure, Washington, D.C. 2008.
- S015 "Plone Conference 2010: An Organiser's View", Netsight, archived copy.
- S028 Wiki page "Virtual Resources", San Francisco 2011 organizers.
- S031 Wiki page "Ploneconf.org handover", San Francisco 2011 organizers.
- S034 Interview with a San Francisco 2011 organizer, Four Digits blog.
- S036 "Plone Conference 2012 Wrap-up", organizer account, Four Digits.
- S043 Special-edition post-conference newsletter, Bristol 2014, plone.org.
- S051 Detailed attendee logistics, Boston 2016.
- S070 Foundation board minutes with the organizer's report, Eibar 2023.
- S079 Feedback, videos and photos from Plone Conference 2025, plone.org.
- S099 GitHub issues and project board collaboration review, 2026 organizing team.
- S107 Email campaigns README, 2026 organizing team.
