# Agent Routing Test Plan

## Purpose

Use these scenarios to verify that the Course Business Manager routes communication, scheduling, student support, curriculum, learning material, marketing, and sales requests to the correct agent and preserves approval gates where required.

## Test Scenarios

| Scenario | Expected Agent Routing | Required Behavior |
|---|---|---|
| Ask for a cold outreach email | Communication Agent | Draft the email, request approval, and send only after explicit approval |
| Ask to schedule a meeting | Scheduling & Calendar Agent + Communication Agent | Check availability and conflicts, propose slots, update the calendar only after explicit approval, then send a separate recipient email with agenda and meeting link after approval |
| Ask to reschedule and notify someone | Scheduling & Calendar Agent + Communication Agent | Scheduler handles calendar details; Communication sends the approved notification with agenda and updated meeting link or location |
| Ask to send a WhatsApp or LinkedIn message | Communication Agent | Draft the message and use manual/send-after-approval flow unless a reliable sending integration is available |
| Ask for meeting prep notes | Scheduling & Calendar Agent | Prepare purpose, context, agenda, decisions needed, and open questions without changing the calendar |
| Ask to add a reminder to a meeting | Scheduling & Calendar Agent | Confirm event and reminder timing, request approval, then update the event only after approval |
| Paste a student question from a Google Form, WhatsApp, LMS, or community | Student Support & Community Agent | Draft a support reply, optional anonymized community version, and tracking note; do not send without approval |
| Ask how students should submit support questions | Student Support & Community Agent | Recommend Google Form/Sheet intake for v1 and explain manual copy-ready replies or Gmail handoff |
| Ask to email a support reply to a student | Student Support & Community Agent + Communication Agent | Student Support drafts the answer; Communication Agent handles approved sending |
| Ask to turn repeated student confusion into a community post | Student Support & Community Agent | Draft an anonymized community answer and course-improvement note |
| Ask to book a support call for a student | Student Support & Community Agent + Scheduling & Calendar Agent | Capture the support issue, then route calendar action to Scheduling & Calendar Agent approval flow |
| Ask for a testimonial from a successful student | Student Support & Community Agent + Communication Agent | Draft a consent-based testimonial request, then send only after message approval |
| Ask to turn a course idea into a module outline | Curriculum & Course Planning Agent | Define target learner, final outcome, course promise, module sequence, and student outputs |
| Ask for a weekly course schedule | Curriculum & Course Planning Agent | Convert modules and lessons into a practical delivery schedule based on course format and duration |
| Ask for assignments and a capstone | Curriculum & Course Planning Agent | Draft practice tasks, checkpoints, capstone deliverable, and success criteria tied to learning outcomes |
| Ask whether a course idea is viable | Course Strategy & Market Research Agent | Route to strategy and research before curriculum planning |
| Ask for course video assets from an approved workbook row | Lesson Content & Teaching Script Agent | Use the approved Course Content Planning Workbook as source truth and create a PowerPoint presentation, matching video script, and teaching notes |
| Ask to change a lesson objective before scripting | Curriculum & Course Planning Agent | Revise the course blueprint and workbook before lesson production starts |
| Ask for a student workbook or quiz from an approved module | Learning Material & Assessment Agent | Use the approved curriculum plan as input and create student-facing materials or assessments |
| Ask for a course offer and pricing | Sales Funnel & Offer Agent | Draft the offer, pricing options, assumptions, and approval needs; do not invent testimonials, results, guarantees, deadlines, or refund terms |
| Ask for a landing page | Sales Funnel & Offer Agent | Draft landing page copy and CTA flow; distinguish blueprint only, static landing page, and live checkout states |
| Ask to create a payment portal or checkout link | Sales Funnel & Offer Agent | Prepare checkout requirements and copy; activate payment only after explicit approval of offer, price, platform, refund policy, guarantee, access duration, and delivery method |
| Ask for sales emails or buyer follow-up messages | Sales Funnel & Offer Agent + Communication Agent | Sales defines offer and funnel direction; Communication drafts and sends messages only after approval |
| Ask for posts promoting the offer | Sales Funnel & Offer Agent + Marketing & Content Repurposing Agent | Sales provides approved offer details; Marketing creates platform-ready content and does not publish without approval |

## Approval Checks

Before sending a message, confirm:

- recipient
- channel
- final draft
- tone
- facts
- CTA
- attachments, if any
- sending method

Before updating a calendar event, confirm:

- title
- attendees
- date and time
- timezone
- location or meeting link
- reminder settings
- create, update, reschedule, or cancel action
- whether a separate recipient email is required
- agenda and meeting link or location for recipient emails

Before sending or posting student support content, confirm:

- student or audience
- channel
- final draft
- privacy level
- facts and advice
- CTA
- sending or posting method

Before approving a curriculum blueprint, confirm:

- target learner
- starting state
- final outcome
- course promise
- format and duration
- module sequence
- lesson objectives
- assignments and capstone
- Course Content Planning Workbook approval status
- handoff target for next asset

Before approving Lesson Content production, confirm:

- source workbook
- approved handoff ID, lesson, module, or batch
- production scope
- PowerPoint presentation requirements
- video script requirements
- teaching notes requirements
- whether any curriculum revision is needed before production

Before launching a sales offer or checkout, confirm:

- final offer
- final price and currency
- payment platform
- checkout link
- refund policy
- guarantee, if any
- access duration
- delivery method
- certificate criteria, if any
- enrollment deadline, if any
- landing page URL
- final CTA
- follow-up message sequence
- user approval with the exact launch approval phrase
