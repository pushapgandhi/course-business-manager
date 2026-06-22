# Student Support Intake Form

Use this form for Google Forms, Google Sheets, pasted student questions, or email-style support requests.

## Recommended Google Form Fields

| Field | Type | Required |
|---|---|---|
| Student name | Short answer | Yes |
| Email address | Short answer | Yes |
| WhatsApp or preferred contact, if different | Short answer | No |
| Course or cohort | Short answer | Yes |
| Module or lesson | Short answer | Yes |
| What are you stuck on? | Paragraph | Yes |
| What have you already tried? | Paragraph | No |
| What outcome do you want from this answer? | Paragraph | Yes |
| How urgent is this? | Multiple choice: Low, Normal, High | Yes |
| Can this question be answered anonymously in the community? | Multiple choice: Yes, No | Yes |
| Upload or link to relevant work | File upload or short answer | No |

## Recommended Google Sheet Columns

| Column | Purpose |
|---|---|
| Timestamp | When the question arrived |
| Student name | Who needs help |
| Email | Reply destination |
| Preferred channel | Email, WhatsApp, LMS, community, or manual |
| Course/cohort | Relevant program |
| Module/lesson | Relevant content area |
| Question | Student's question or blocker |
| Tried already | Context for troubleshooting |
| Desired outcome | What success looks like |
| Urgency | Low, Normal, or High |
| Public/anonymized allowed | Whether a community version is allowed |
| Category | Question, blocker, motivation, complaint, feedback, testimonial, technical, admin |
| Status | New, Drafted, Approved, Sent, Waiting, Resolved, Escalated |
| Follow-up date | When to check back |
| Course-improvement note | Repeated confusion, missing example, unclear lesson, or new FAQ |

## Manual Intake Prompt

When the user copies a student question into chat, collect this:

```text
Student name:
Channel:
Course/cohort:
Module/lesson:
Student question:
What the student tried:
Desired outcome:
Urgency:
Can this be answered anonymously in the community?
```

## Minimal Intake Questions

If details are missing, ask only what is needed:

1. Which course, module, or lesson is this about?
2. What exactly did the student ask or submit?
3. Where should the approved reply go: email, WhatsApp, community, LMS, or manual copy?
4. Is this a private reply only, or can I also create an anonymized community answer?
