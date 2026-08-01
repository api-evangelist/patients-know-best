---
name: Send a questionnaire and collect responses
description: >-
  Send a PKB questionnaire request to a patient and retrieve their submitted
  questionnaire responses via the Patients Know Best FHIR API.
api: fhir/patients-know-best-facade-capabilitystatement.json
operations:
- Questionnaire.search
- Questionnaire.$send-questionnaire-request
- QuestionnaireResponse.search
---

# Send a questionnaire and collect responses

Use the Patients Know Best (PKB) FHIR STU3 Facade API to push a questionnaire
to a patient and read their answers.

## Auth

Obtain an OAuth 2.0 client-credentials bearer token and send it as
`Authorization: Bearer <token>` with `Accept: application/fhir+json`.

## Steps

1. **Find the questionnaire.** `GET /fhir/Questionnaire?publisher-reference=<org>`
   or read one by id.
2. **Send the request to the patient.** Invoke the custom operation
   `send-questionnaire-request` on the `Questionnaire` resource
   (`POST /fhir/Questionnaire/<id>/$send-questionnaire-request`) with the
   target patient in the operation parameters.
3. **Collect responses.** Search `QuestionnaireResponse` for the patient:
   `GET /fhir/QuestionnaireResponse?patient=<id>&questionnaire=<id>&authored=<range>`.

## Rules

- All identifiers require both a system and a value.
- Results come back as a FHIR `Bundle`; page with `Bundle.link`.
- On error, read the `OperationOutcome`
  (`errors/patients-know-best-problem-types.yml`).
- See `conventions/patients-know-best-conventions.yml` for search/paging rules.
