# Operations Workflow

## Purpose

This workflow keeps the Course Business Manager project organized without adding a database, app framework, or external project-management tool.

Use `operations/task_board.md` as the source of truth. Use `operations/dashboard.html` as the visual summary.

## Weekly Review Checklist

Review this project once per week or before starting a new work stream.

1. Check the active work stream.
2. Confirm the next recommended task.
3. Update task statuses.
4. Add any blockers to Risks & Dependencies.
5. Add any user decisions to Decisions / Approvals Needed.
6. Record the most important change in Recent Updates.
7. Confirm the dashboard still matches the task board.

## Status Rules

Use only these statuses:

- Not started: work has not begun.
- In progress: this is actively being built or planned.
- Waiting: work is blocked by a decision, dependency, or missing input.
- Done: the expected output exists and is ready to use.

Only one major work stream should be In progress at a time unless there is a clear reason to split focus.

## Priority Rules

Use only these priorities:

- High: needed before other tasks can move forward.
- Medium: useful soon, but not blocking immediate progress.
- Low: helpful later, but not urgent.

When choosing the next task, prefer the highest-priority unfinished task unless a dependency blocks it.

## Approval Rules

Add an item to Decisions / Approvals Needed when work requires user confirmation before moving forward.

Examples:

- choosing the next work stream
- approving public dashboard content
- publishing to GitHub Pages
- changing the project structure
- marking a major work stream as Done

Do not send messages, update calendar events, publish sensitive data, or make business decisions without user approval.

Communication tasks may send through an available channel only after the user approves the final draft, recipient, channel, and sending method.

Scheduling tasks may create, update, reschedule, or cancel calendar events only after the user approves the final meeting details. Scheduled or rescheduled meetings with recipients must also send a separate recipient email that includes the agenda and meeting link or location.

## Risk and Dependency Rules

Track risks and dependencies only when they affect next actions.

Use short entries with:

- item
- impact
- owner
- next action
- status

Keep this section small. Remove resolved items during the weekly review.

## Update Process

When project progress changes:

1. Update `operations/task_board.md`.
2. Update the matching summary values in `operations/dashboard.html`.
3. Add a Recent Updates entry.
4. Check the dashboard in a browser.
5. Commit and push when the update is ready to publish.

## Current Operating Default

Operations v1 is approved and complete.

Communication Agent v1 is complete.

Scheduling & Calendar Agent is complete.

Student Support & Community Agent is complete.

Curriculum & Course Planning Agent is complete.

Lesson Content & Teaching Scripts Agent is complete.

Learning Materials & Assessment Agent is complete.

Marketing & Content Repurposing Agent is complete.

Sales Funnel & Offer Agent is complete.

The next recommended work stream is Course Strategy & Market Research.

Operations v1 remains complete as long as:

- the workflow exists
- the task board has active focus, risks, approvals, and update sections
- the dashboard summarizes the same information
- the next work stream is clear
