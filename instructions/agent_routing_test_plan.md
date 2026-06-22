# Agent Routing Test Plan

## Purpose

Use these scenarios to verify that the Course Business Manager routes communication and scheduling requests to the correct agent and preserves approval gates.

## Test Scenarios

| Scenario | Expected Agent Routing | Required Behavior |
|---|---|---|
| Ask for a cold outreach email | Communication Agent | Draft the email, request approval, and send only after explicit approval |
| Ask to schedule a meeting | Scheduling & Calendar Agent + Communication Agent | Check availability and conflicts, propose slots, update the calendar only after explicit approval, then send a separate recipient email with agenda and meeting link after approval |
| Ask to reschedule and notify someone | Scheduling & Calendar Agent + Communication Agent | Scheduler handles calendar details; Communication sends the approved notification with agenda and updated meeting link or location |
| Ask to send a WhatsApp or LinkedIn message | Communication Agent | Draft the message and use manual/send-after-approval flow unless a reliable sending integration is available |
| Ask for meeting prep notes | Scheduling & Calendar Agent | Prepare purpose, context, agenda, decisions needed, and open questions without changing the calendar |
| Ask to add a reminder to a meeting | Scheduling & Calendar Agent | Confirm event and reminder timing, request approval, then update the event only after approval |

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
