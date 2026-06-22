# Google Form And Sheet Setup

## Purpose

Use this setup to receive student support questions without needing a custom app or helpdesk.

## Student-Facing Form

Create a Google Form named:

```text
[Course Name] Student Support Request
```

Add these fields:

| Question | Type | Required |
|---|---|---|
| Your name | Short answer | Yes |
| Email address | Short answer | Yes |
| Preferred reply channel | Multiple choice: Email, WhatsApp, LMS/community, Other | Yes |
| Course or cohort | Short answer | Yes |
| Module or lesson | Short answer | Yes |
| What are you stuck on? | Paragraph | Yes |
| What have you already tried? | Paragraph | No |
| What outcome do you want from this answer? | Paragraph | Yes |
| How urgent is this? | Multiple choice: Low, Normal, High | Yes |
| Can we answer this anonymously in the community if it helps other students? | Multiple choice: Yes, No | Yes |
| Relevant link, screenshot, or file | File upload or short answer | No |

## Response Sheet

Connect the form to a Google Sheet named:

```text
[Course Name] Student Support Tracker
```

Add these support-management columns after the form response columns:

| Column | Values Or Notes |
|---|---|
| Category | Question, blocker, motivation, complaint, feedback, testimonial, technical, admin |
| Status | New, Drafted, Approved, Sent, Waiting, Resolved, Escalated |
| Assigned owner | User, Course Business Manager, assistant, instructor |
| Draft reply | Paste the drafted reply here if useful |
| Follow-up date | Date to check back |
| Course-improvement note | Repeated confusion, missing example, unclear lesson, FAQ need |
| Testimonial candidate | Yes/No |

## Operating Flow

1. Student submits the Google Form.
2. The response appears in the Google Sheet.
3. User copies the row or question into the Course Business Manager chat.
4. Student Support Agent drafts:
   - private student reply
   - optional anonymized community answer
   - tracking note
   - course-improvement insight
5. User approves or edits the reply.
6. Reply is sent manually by copy-paste, or through Gmail using the Communication Agent approval flow.
7. User updates the Sheet status.

## Student Instructions

Share this with students:

```text
If you need help, submit your question through the support form: [form link]

Please include the module or lesson, what you are stuck on, and what you have already tried. This helps me give you a more useful answer.

For urgent access or payment issues, mention "High" urgency in the form.
```

## Default Reply SLA

Use this simple service level unless the user chooses another:

| Urgency | Target Reply |
|---|---|
| High | 1 business day |
| Normal | 2 business days |
| Low | 3 business days |

## Later Automation Options

Keep v1 manual. Later upgrades can include:

- Gmail drafts created from new Sheet rows
- Google Apps Script notifications when urgent questions arrive
- Slack, Discord, Circle, or LMS integration
- helpdesk migration when support volume grows
