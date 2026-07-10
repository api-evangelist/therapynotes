# TherapyNotes (therapynotes)

TherapyNotes is a HIPAA-compliant practice management and electronic health record (EHR) platform built specifically for behavioral health - therapists, psychologists, psychiatrists, social workers, and group practices. It provides interactive clinical note templates and documentation, scheduling with appointment reminders, a client portal, telehealth, electronic insurance claims and ERA, integrated credit card processing, and TherapyFuel AI tooling.

## API Access: None (Honest Gated Stub)

**TherapyNotes does not expose a public or partner developer API.** There is no documented REST API, no webhooks, no WebSocket, no OpenAPI, and no self-serve developer program. Industry analysis describes this as "zero API" - an explicit architectural decision - meaning TherapyNotes cannot be connected directly to marketing tools, CRMs, billing platforms, data dashboards, or workflow automation (e.g., Zapier).

Client, appointment, clinical-note, and billing data live inside the authenticated, HIPAA-gated web application and manual exports. The only native "integrations" are one-way calendar sync to Google Calendar, Microsoft Outlook, and iCloud. Custom integration work, when available, is a paid TherapyNotes professional-services engagement, not an API.

Third parties such as **Supergood** and **Keragon** offer *unofficial* programmatic access to TherapyNotes data by automating the application. These are not TherapyNotes-published APIs and are outside TherapyNotes' support; their existence is itself evidence that no official API is available.

This catalog entry therefore documents TherapyNotes as an **honest gated stub**: the capability areas a behavioral-health EHR API would cover are *modeled* (`endpointsModeled: true`) for completeness, but **no endpoints are fabricated** and no OpenAPI, rate-limit, or FinOps artifacts are provided because there is no public API surface to describe.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/therapynotes/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/therapynotes/refs/heads/main/apis.yml)

## Tags

- Behavioral Health
- EHR
- Practice Management
- Mental Health
- Electronic Health Records
- Medical Billing
- HIPAA
- No Public API

## Timestamps

- **Created:** 2026-07-10
- **Modified:** 2026-07-10

## Modeled Capability Areas

These are the logical surfaces a behavioral-health EHR API would expose. They are modeled for completeness only - **TherapyNotes publishes no endpoints or base URL for any of them.**

### TherapyNotes Clients API (Modeled)

Client (patient) roster - demographics, contacts, insurance, and portal enrollment. Available only in the web application.

### TherapyNotes Scheduling API (Modeled)

Appointments, recurring schedules, and reminders. Native one-way calendar sync to Google Calendar, Outlook, and iCloud exists in-app, but there is no programmatic scheduling API.

### TherapyNotes Clinical Documentation API (Modeled)

Interactive clinical note templates - intake, progress notes, treatment plans, psychiatry documentation. PHI-bearing data available only inside the HIPAA-gated application.

### TherapyNotes Billing and Claims API (Modeled)

Medical billing - electronic insurance claims, ERA, superbills, and integrated card processing - run through an internal clearinghouse workflow in-app. No billing API is exposed.

## Pricing

TherapyNotes sells per-clinician platform subscriptions (not API plans). Captured 2026-07-10:

- **Solo:** $69 / clinician / month
- **Group:** $79 first clinician / month, $50 per additional clinician / month, unlimited non-clinical users
- **Enterprise:** Same rates as Group, minimum 30 users, dedicated account manager
- **Add-ons:** Electronic claims $0.14/claim, ERA $0.14/ERA, Premium Telehealth $15/clinician/month, TherapyFuel AI Scribe $40/provider/month
- **Free trial:** 30 days

See [plans/therapynotes-plans-pricing.yml](plans/therapynotes-plans-pricing.yml). Confirm current figures at [therapynotes.com/pricing](https://www.therapynotes.com/pricing/).

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/therapynotes-llc)
- [Website](https://www.therapynotes.com)
- [Documentation](https://support.therapynotes.com/hc/en-us)
- [Plans](plans/therapynotes-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
