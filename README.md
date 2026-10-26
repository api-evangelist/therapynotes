# TherapyNotes (therapynotes)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
