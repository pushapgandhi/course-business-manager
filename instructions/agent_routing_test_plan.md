# Agent Routing Test Plan

## Purpose

Use these scenarios to verify that the Course Business Manager routes communication and scheduling requests to the correct agent and preserves approval gates.

## Test Scenarios

| Scenario | Expected Agent Routing | Required Behavior |
|---|---|---|
| Ask for a cold outreach email | Communication Agent | Draft the email, request approval, and send only after explicit approval |
| Ask to schedule a meeting | Scheduling & Calendar Agent | Check availability and conflicts, propose slots, and update the calendar only after explicit approval |
| Ask to reschedule and notify someone | Scheduling & Calendar Agent + Communication Agent | Scheduler handles calendar details; Communication drafts the notification and sends only after approval |
| Ask to send a WhatsApp or LinkedIn message | Communication Agent | Draft the message and use manual/send-after-approval flow unless a reliable sending integration is available |

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
