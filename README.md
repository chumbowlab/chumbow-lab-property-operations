# Property Operations | Maintenance Coordination Prototype

A lightweight property-maintenance coordination prototype for landlords and property managers in Kenya.

**Status:** Prototype · **Stack:** HTML, CSS, vanilla JavaScript

## What problem does it address?

Property maintenance requests are often spread across messages, calls and spreadsheets. This prototype brings request details, urgency, assignments, progress and costs into one browser-based workspace.

## How does it work?

The dashboard lets a user record and manage maintenance jobs, organise technician assignments and review work through a defined status flow.

- Create, edit, search, filter, sort and remove maintenance jobs.
- Track urgency, due dates, trades, assignments and job notes.
- Maintain a technician directory with trade and availability details.
- Record completion notes, dates, manager acceptance and activity history.
- Compare estimated and actual costs.
- Export job records as CSV and create a JSON backup.
- Explore the interface with sample data.

## What is it built with?

HTML5, CSS3 and vanilla JavaScript. The prototype uses browser localStorage for persistence and browser-generated files for exports. It requires no package installation or build process.

## How can you try it?

1. Clone or download this repository.
2. Open `index.html` in a modern browser.
3. Explore the sample records and test the workflow.
4. Add non-sensitive test records to understand how browser storage behaves.

There is no hosted public demo linked at present. The repository itself contains the runnable prototype.

## Workflow and design decisions

The prototype separates the **stage of a job** from its **urgency**. A request can move through Reported, Assigned, In progress, Awaiting approval and Completed, while urgency helps the manager decide what needs attention first. Cancelled jobs can also be recorded.

A few choices shape the workflow:

- **Completion has a hand-off.** Completion notes are required before a job can be marked complete; the completion date and manager-acceptance state can be recorded separately.
- **Costs remain comparable.** Estimated and actual costs are stored as separate fields rather than overwriting the original estimate.
- **Technician status is explicit.** Availability and verification are separate manual declarations. A verification flag is not an independent background check.
- **Changes have context.** Job activity history records important updates so a manager can review how a request progressed.
- **Urgent hazards are surfaced.** The interface displays a safety reminder for urgent open work. It is an administrative prompt, not a risk assessment or emergency-response service.

A reusable companion resource is available in [`resources/MAINTENANCE-WORKFLOW-TEMPLATE.md`](./resources/MAINTENANCE-WORKFLOW-TEMPLATE.md). It provides a request-record template, suggested hand-off checks and privacy reminders that can be adapted independently of the prototype.

## What should you know before using it?

This is an early, single-browser prototype—not a production property-management service. Records are stored locally and are not synchronised across users or devices. It has no server-side database, user authentication, role-based access, independent technician verification or managed backup service. Do not enter tenant personal data, access codes, payment details or other sensitive information. Technician verification flags are manual declarations. The application is not an emergency-response service.

## What comes next?

The roadmap includes a secure backend, authentication and roles, shared records, audit history, evidence attachments, approval workflows, notifications, automated tests and pilot feedback from property managers.

## Want to discuss a practical digital system?

**[Contact Paul Chumbow about a project or workflow challenge](mailto:paulchumbow254@gmail.com?subject=Chumbow%20Lab%20project%20enquiry).**

---

Built by **Paul Chumbow** · Chumbow Lab — *Turning Ideas Into Systems That Work.*