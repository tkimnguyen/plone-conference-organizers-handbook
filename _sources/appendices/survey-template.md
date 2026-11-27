---
steward: unassigned
deputy: unassigned
review-by: 2027-11-01
maturity: draft
applies-to: [all]
diataxis: reference
myst:
  html_meta:
    "description lang=en": "A copyable attendee and non-attendee survey for a Plone conference, with the method, the redesigned question set and an analysis checklist."
    "keywords": "Plone, Plone Conference, survey, feedback form, template, post-conference"
---

# Template: attendee survey

Copy this page's blocks into your own form tool and edit the placeholders in angle brackets.
The method comes from the 2026 survey, and the question set is the redesign that survey asked for.
The 2026 findings themselves are in the [2026 case file](../conferences/2026-maastricht/conference-2026-maastricht.md).

The survey serves one purpose: to tell the next team what to keep, what to change and who it failed to reach.
Write the questions you want answered before you write the form, and name the decision each question feeds.

## Method

### How the 2026 survey ran

1. A web form on the community site collected the answers.
   Every submission arrived as an individual email, which is enough for structured ratings and free text (L-6001).
   It also means every submission is a private message that must be extracted before analysis (L-6001).
2. A deterministic script extracted each submission into structured data.
   A second script computed every rating and count, so a reviewer can rerun the numbers instead of trusting a hand tally (L-6003).
3. The analysis was written with respondents numbered, never named.
   The raw submissions stayed private and git-ignored, and no sanitized raw dataset was published.
4. The analyst reviewed the first reading against the data before publishing.
   The adversarial review is a deliberate step: in 2026 it caught readings that the data contradicted (L-6005).
5. The organizers filed the anonymized analysis as a handover item (see [Handover contract](../job/handover-contract.md)).

Plan for about one in five ticket holders to answer.
The 2026 survey drew 21 responses over about three weeks.
Set your success metrics so that a response count of that size can still answer them (see [Defining success](../job/defining-success.md)).

### Older precedents

The Seattle 2006 questionnaire had eight blocks that remain a usable skeleton: overall ratings, agreement with outcome statements, logistics ratings, more-or-fewer preferences per session format, prior experience, sector, factors in the decision to attend, and planned follow-up actions (L-1020).
The Brasília 2024 feedback form asked for 1-to-5 ratings of sessions plus free text, and made the email address optional so people could answer anonymously (L-4209).
Both ideas survive in the question battery below.

### Check the form before you read the data

Before you interpret a missing answer, check whether the form's skip logic ever showed the question to that respondent.
In 2026 a question census, one line per question with the number of respondents who saw it, showed that several low answer counts were properties of the form, not extraction errors (L-6006).
Keep that census as a file next to the analysis.

## What the 2026 form got wrong

The 2026 team and its analyst listed these defects.
Each one became a rule in the question set below.

| 2026 defect | Rule in this template |
|---|---|
| Free-text fields were too small to write in comfortably (L-6008). | Every free-text field is large, and the form tool is tested on a phone. |
| There was no general open comment field at the end (L-6009). | The last question is one open field with no topic. |
| Skip logic hid the relationship-to-the-community question from half the sample, so the one question that could profile the audience did not cover it (L-6010). | Profile questions are shown to everyone and never sit behind skip logic. |
| A value-for-money rating had no direct price-perception question, so low scores could not be explained (L-6011). | Ask about price directly, and ask what a fair price would have been. |
| The form did not ask what nearly stopped the respondent from coming (L-6012). | Ask which barriers came close to stopping each respondent. |
| The survey reached attendees only (L-6013). | Send a short non-attendee version to the same lists. |

The lesson behind the last row is the broadest.
An attendee-only survey is a community pulse, not a market signal, so design the survey to hear the people you failed to reach as well as the people who came (L-6014).

## Design rules

1. Keep the email address optional, and ask for no name.
2. Mark each conditional question in the form plan and keep the question census (L-6006).
3. Use one rating scale throughout, 1 to 5, and always offer "did not attend this" for area ratings.
4. Put the profile questions first, shown to all, and the open field last.
5. Tell respondents how their answers are stored, who reads them and that quoted text is never published.
6. Test the form on a phone and with a screen reader before the link goes out.
7. Open the survey within one week after the last conference day, close it after three weeks, and send one reminder.

## The attendee form

Copy the block, then drop the areas that did not exist at your conference.
Questions marked (all) are shown to every respondent.

```text
ATTENDEE SURVEY: <Conference name and year>

Introduction (all)
Thank you for coming. This survey takes about <N> minutes.
Answers are stored privately and read by <role, for example the organizing team and the survey analyst>.
We publish only anonymized aggregates. We never publish quoted text.
Email address (optional, for follow-up only): ____

Section 1: About you (all)
1.1  What is your relationship to Plone? (choose all that apply)
     [ ] I contribute code, documentation or translations
     [ ] I earn my living providing Plone services
     [ ] I use Plone in my organization
     [ ] I evaluate Plone
     [ ] I am a student or researcher
     [ ] None of these
     [ ] Other: ____
1.2  Is this your first Plone conference?  [ ] Yes  [ ] No, I attended <N> before
1.3  Which days did you attend? (trainings, talks, business track, sprints)
1.4  Who paid for your ticket?  [ ] Myself  [ ] My employer  [ ] A scholarship or grant  [ ] Other
1.5  What is your sector? [ ] Public sector [ ] Education [ ] Service provider [ ] Industry [ ] Other
1.6  Where did you travel from? (country)

Section 2: Ratings, 1 (poor) to 5 (excellent), or "did not attend this" (all)
2.1  The conference overall
2.2  Talks and program
2.3  Trainings
2.4  Business or side tracks
2.5  Sprints
2.6  Venue and rooms
2.7  Food and catering
2.8  Organizing and logistics
2.9  Social events and party
2.10 Accessibility and inclusion
2.11 Communication before the event (website, email, schedule)
2.12 Value for money

Section 3: Price and barriers (all)
3.1  The ticket price felt:  [ ] Too low  [ ] Fair  [ ] Somewhat high  [ ] Too high
3.2  In your own words: what would have been a fair price for what you got?
3.3  Which of these nearly stopped you from coming? (choose all that apply)
     [ ] Ticket price  [ ] Travel cost  [ ] Time away from work  [ ] Employer approval
     [ ] Visa or border rules  [ ] Location  [ ] Program  [ ] Date
     [ ] Nothing came close  [ ] Other: ____
3.4  Tell us more about the item you ticked first.

Section 4: Choosing and changing (all)
4.1  Agreement, 1 (disagree) to 5 (agree):
     - I learned something I can use in my work.
     - I met people I wanted to meet.
     - I would recommend this conference to a colleague.
4.2  For each format, would you like more, the same or fewer?
     [ ] Talks  [ ] Trainings  [ ] Lightning talks  [ ] Open spaces  [ ] Panels  [ ] Sprints
4.3  What was the main reason you decided to attend?
4.4  What did you plan to do as a result? (choose all that apply)
     [ ] Start a project  [ ] Join a sprint topic  [ ] Contribute  [ ] Write or talk about it
     [ ] Change how we use Plone  [ ] Nothing specific
4.5  Will you attend the next edition?  [ ] Yes  [ ] Perhaps  [ ] Probably not
     If probably not, what would change your mind?

Section 5: In your words (all)
5.1  What should the organizers keep doing?
5.2  What should they stop doing?
5.3  What should they start doing?
5.4  Anything else? (one open field, any topic)
```

## The non-attendee form

Send it to the same mailing lists and channels, and to people who registered but did not come.
Keep it short enough to finish in two minutes, and never lead with the attendees' results.

```text
SHORT SURVEY FOR PEOPLE WHO DID NOT ATTEND: <Conference name and year>

1.  What is your relationship to Plone? (same choices as the attendee form, question 1.1)
2.  Did you consider coming?  [ ] Yes  [ ] No
3.  Which of these kept you from coming? (choose all that apply)
    [ ] Ticket price  [ ] Travel cost  [ ] Time away from work  [ ] Employer approval
    [ ] Visa or border rules  [ ] Location  [ ] Program  [ ] Date  [ ] I did not know about it
    [ ] Other: ____
4.  How did you hear about the conference, if you did?
5.  What would make you come to the next edition?
6.  Anything else? (one open field, any topic)
```

## Analysis checklist

1. Write the question census first: each question and how many respondents saw it (L-6006).
2. Extract and aggregate by script, and keep the scripts with the analysis (L-6003).
3. Report the sample honestly.
   Say who answered, who did not, and which group is missing (L-6010, L-6014).
4. Write each interpretation as a claim, then try to contradict it with the data before it stays.
5. Label every finding observed (counts and ratings) or reported (free text and your own reading).
6. Strip names, employers and any detail that lets an insider recognize a respondent.
   Keep raw submissions out of version control.
7. File the anonymized analysis under the conference record, and cite it in the post-mortem (see [Template: post-mortem](post-mortem-template.md)).
