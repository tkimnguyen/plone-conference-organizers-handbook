---
steward: unassigned
deputy: unassigned
review-by: 2028-11-02
maturity: draft
applies-to: [all]
diataxis: how-to
myst:
  html_meta:
    "description lang=en": "First-hour actions when the conference network fails or saturates, with the roles that own the response."
    "keywords": "Plone, Plone Conference, Wi-Fi, network failure, incident playbook"
---

# Playbook: Wi-Fi failure

Open this playbook when attendees cannot get online at the venue.
It covers the first hour; the network plan itself is in `av-recording-internet`.

## Triggers

- Attendees in several rooms report no connection at the same moment, most often on the opening morning, when every device connects at once (L-4097).
- Devices join the network but get no address, which points to an exhausted address pool.
- The network is not live when doors open, because the provider is still installing.
- Pages load but specific tools fail, which points to ports blocked upstream.
- The live stream or the live coverage stops because the uplink is down.
- The person who runs the network cannot be reached; open [Playbook: key-person loss](key-person-loss.md) as well.

## First-hour actions

1. Establish the scope within five minutes: test with two devices in two rooms and write down which rooms, which symptom and the time.
2. Call the upstream network administrators on the direct number agreed before the event, not the venue's general desk (L-1122).
   Done looks like a named contact at the provider who has acknowledged the fault.
3. Ask the network owner to classify the fault as one of: no uplink, no addresses, saturation, blocked ports, or local hardware.
   Each class has a different fix and a different time to repair.
4. Protect the stage: presenters switch to local copies of their slides, and the recording team keeps recording to local disk.
5. Move the registration desk and the stream to the wired or mobile backup, if one exists.
   Registration works from an offline attendee list until the network returns.
6. Tell the room hosts and the information desk one sentence: what is down, what still works, and when the next update comes.
   Announce the same sentence at the next session change, because a chat message cannot reach people without a network.
7. If no fix is in sight after 30 minutes, ask attendees to connect one device each and to pause large downloads and video calls.
8. Keep a timestamped log of the fault, the calls and the fixes for the post-mortem.

## Owner roles

| Role | Responsibility | Full advice in |
|---|---|---|
| Network owner | Diagnoses the fault, works with the provider, and decides on the backup. | `av-recording-internet` |
| Venue liaison | Reaches the venue's technical staff and the provider when the direct line fails. | `venue` |
| Recording lead | Keeps recording to local disk and decides whether the stream pauses. | `av-recording-internet` |
| Registration lead | Runs check-in from the offline attendee list. | `ticketing-and-registration` |
| On-site lead | Briefs the room hosts and the information desk, and sets the update rhythm. | `signage-and-showtime` |
| Communications lead | Publishes the status on the website and social channels once a channel works. | `web-comms-brand` |

## Related chapters

- [The risk register method](../risk-method.md) explains how this playbook relates to the chapter risks.
- [Playbook: key-person loss](key-person-loss.md) covers the case where the network owner drops out.
- [Risk register](../../generated/risk-register.md) lists the network risks of every chapter.
- The full advice is in `av-recording-internet`, with venue selection in `venue`.

### What history says

- In 2006 the provider read the installation time as the time to start work, so the network was down until after lunch on the first training day, and the address pool ran out on the first conference day (L-1114, L-1115 in `av-recording-internet#case-notes`).
- The same organizers concluded that every attendee will connect at once, that providers will not believe it, and that a provider accountable to the organizers should run the network (L-1116, L-1118 in `av-recording-internet#principles-and-general-lessons`).
  One attendee argued the opposite, for a dedicated line and the organizers' own routers (L-1117, hearsay).
- Internet access was the lowest-rated logistics item of that year (L-1123).
- In 2008 the opening-morning load took the venue network down for most of the day, and live coverage of the keynote waited for the fix (L-4097, L-4098).
- In 2010 the returning Wi-Fi specialist's equipment was stolen before the event, and a last-minute order of access points from a local stockist saved the setup (L-2036).
- In 2011 the person responsible for the Wi-Fi was hospitalized two weeks before the conference, with no backup plan (L-3075).
- In 2012 the venue sat on a government network that blocked non-work use, so the organizers paid for a dedicated fiber line that was ready a month before the event (L-2076).
- The requirements register records a venue standard of reliable wireless access for all attendees at once, unverifiable as a binding rule as of 2026-11-02 (R-022 in `requirements-register`).
