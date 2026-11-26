# Property Operations
### Maintenance coordination prototype · Chumbow Lab

A lightweight browser-based prototype exploring a clearer way for landlords and property managers in Kenya to receive, assign and track property maintenance work.

**Built by Paul Chumbow** · [Portfolio](https://paulchumbow254.lovable.app) · [Contact](mailto:paulchumbow254@gmail.com?subject=Property%20Operations%20enquiry)

<p align="center">
  <strong>Reported → Assigned → In Progress → Awaiting Approval → Completed</strong>
</p>

## At a glance

| | |
|---|---|
| **Status** | Functional prototype |
| **Stack** | HTML5 · CSS3 · Vanilla JavaScript |
| **Runtime** | Modern web browser |
| **Persistence** | Browser localStorage |
| **Exports** | CSV records · JSON backup |
| **Backend** | None; single-browser use only |

## The problem

Maintenance requests can become scattered across calls, messages and spreadsheets. That makes it harder to see who owns a job, what has happened, which work is waiting for approval and what it ultimately cost.

This prototype brings those details into one simple workspace.

## What is implemented?

- Create, edit, search, filter, sort and remove maintenance jobs.
- Record request details, urgency, due dates, trade, assignment and notes.
- Maintain a technician directory with trade and availability details.
- Move jobs through the defined status workflow.
- Record completion notes, dates and manager acceptance.
- Compare estimated and actual costs.
- Review activity history for important job changes.
- Export job records to CSV and create a JSON backup.
- Explore the interface using illustrative sample records.

## How to run it

1. Clone or download this repository.
2. Open `index.html` in a modern browser.
3. Explore the sample records and test the workflow.
4. Add non-sensitive test records and try the export and backup features.

No package installation or build process is required.

## Workflow decisions

- **Status and urgency are separate.** Status describes the job's stage; urgency helps prioritise attention.
- **Completion is a hand-off.** Completion notes are required before a job can be marked complete. The completion date and manager-acceptance state can be recorded separately.
- **Estimates are preserved.** Estimated and actual costs remain separate for comparison.
- **Verification is transparent.** Technician availability and verification are manually declared fields, not independent background checks.
- **Changes have context.** Activity history records important job updates.
- **Safety prompts are limited.** Urgent open work can surface a reminder, but the application is not a risk assessment or emergency-response service.

A reusable companion document is available in [Maintenance Workflow Template](./resources/MAINTENANCE-WORKFLOW-TEMPLATE.md).

## Data, privacy and limitations

This is an early single-browser prototype—not a production property-management service.

- Records are stored in the browser's localStorage.
- Data is not synchronised across users or devices.
- There is no server-side database, authentication, role-based access or managed backup service.
- Do not enter tenant personal data, access codes, payment details or other sensitive information.
- Technician verification fields are manual declarations.
- The application is not an emergency-response service.

Use the JSON backup feature to preserve test records. Clearing browser data may remove locally stored records.

## Roadmap

Potential next steps, subject to testing and user feedback:

- Secure backend, authentication and role-based permissions.
- Shared records and an audit trail.
- Evidence attachments and approval workflows.
- Notifications and escalation rules.
- Automated tests and accessibility review.
- Pilot feedback from property managers.

These are future possibilities, not implemented features.

## Feedback or collaboration

If you manage properties or coordinate maintenance and have feedback on this workflow, open a GitHub issue or [contact Paul](mailto:paulchumbow254@gmail.com?subject=Property%20Operations%20feedback).

---

<sub>Paul Chumbow · Chumbow Lab — Turning Ideas Into Systems That Work.</sub>
