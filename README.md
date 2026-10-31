# Patients Know Best

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

Patients Know Best (PKB) is a UK health-technology company operating what it describes as the world's largest personal health record, with more than seven million registered patients across the NHS and other health systems. The platform lets patients hold, view and share their medical records, messages, test results, care plans and questionnaires with clinicians and carers across web, mobile and the NHS App. For integrators, PKB publishes a HL7 FHIR STU3 (3.0.2) API — the "Facade" FHIR server at my.patientsknowbest.com/fhir — that conforms to the NHS CareConnect profiles and exposes patient demographics, documents, observations, appointments, consent, questionnaires and read receipts, secured with OAuth 2.0 client-credentials. PKB was surfaced as a Seedcamp portfolio company and enriched into the API Evangelist network.

**Areas:** Company · Health · Healthcare · Electronic Health Records · Personal Health Record · FHIR · Interoperability · NHS · Patient Data · Medical Records

## Patients Know Best on APIs.io

Everything profiled for Patients Know Best is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/patients-know-best/](https://apis.io/providers/patients-know-best/)** — or go straight to one of the APIs or properties below.

### APIs (1)

- [PKB Facade FHIR API](https://apis.io/apis/patients-know-best/pkb-facade-fhir-api/) — HL7 FHIR STU3 (3.0.2) "Facade" server exposing Patients Know Best personal health record data — Patient, Appointment, Communication, Consent,…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [patients-know-best](https://apis.io/servers/patients-know-best/patients-know-best/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Patients Know Best Authentication](https://apis.io/security/patients-know-best/patients-know-best-authentication/)
- [Patients Know Best Domain Security](https://apis.io/security/patients-know-best/patients-know-best-domain-security/)
- [Patients Know Best Vulnerability Disclosure](https://apis.io/security/patients-know-best/patients-know-best-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://patientsknowbest.com)
- [Documentation](https://wiki.patientsknowbest.com/space/api/3363602489/FHIR%C2%AE+APIs)
- [API reference](https://pkbdev.atlassian.net/wiki/spaces/api/pages/3363602541/FHIR+Conformance)
- [Sign up](https://patientsknowbest.com/register/)
- [Support](https://manual.patientsknowbest.com/)
- [Changelog](https://wiki.patientsknowbest.com/space/REL)
- [Blog](https://patientsknowbest.com/news/)
- [Security](https://my.patientsknowbest.com/.well-known/security.txt)
- [Compliance](https://patientsknowbest.com)
- [Privacy policy](https://patientsknowbest.com/privacy-statement/)
- [Status](https://www.pkbstatus.com/)

## API Evangelist rating

**Kin Score 41.9** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 32.3 |
| Contract governance | 18.2 |
| Operational transparency | 47.4 |
| Developer ergonomics | 49.4 |
| Access clarity | 31.6 |

**Agent readiness 17.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | na |

**Regulatory alignment 25.0** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/patients-know-best/](https://apis.io/providers/patients-know-best/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Patients Know Best: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/patients-know-best/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
