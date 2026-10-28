# Chumbow Lab — Property Operations

A responsive, single-file HTML prototype for coordinating property maintenance requests for landlords and property managers in Kenya.

## Problem

Maintenance requests can become difficult to track when job details, technician assignments, urgency, costs, and completion updates are scattered across messages and spreadsheets. This prototype explores a clearer workflow for recording requests and following work through to completion.

## Features

- Dashboard metrics for total, open, urgent, and completed jobs
- Create, edit, search, filter, sort, and delete maintenance jobs
- Track urgency, status, due dates, technician assignments, and job notes
- Technician directory with trade, availability, and verification flags
- Warning when a technician's listed trade does not match a job
- Completion notes, completion date, manager acceptance, and activity history
- Separate estimated and actual cost reporting
- JSON backup and CSV job export
- Responsive dark interface with green Chumbow Lab accents
- Demo data to explore the prototype

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. The prototype uses browser `localStorage` to retain records in that browser.

No build step or package installation is required.

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Browser `localStorage` and Blob-based file export

## Important limitations

This is an early prototype, not a production-ready service. Records are stored locally in one browser and are not shared across users or devices. Browser storage is not a secure database. Do not enter sensitive tenant, property-access, or payment information. Technician verification flags are manual declarations and do not constitute independent verification. Safety-critical hazards require appropriate professional or emergency response; the app does not provide emergency services.

## Future improvements

- Backend database, authentication, and role-based access
- Shared records, audit logs, and reliable backups
- Evidence attachments and approval workflow
- Notifications and escalation rules
- Stronger automated validation and browser interaction tests
- Pilot testing with Kenyan landlords and property managers

## Project status

Prototype / learning project. Features and workflows are subject to testing and iteration.

## Author

Chumbow Lab
