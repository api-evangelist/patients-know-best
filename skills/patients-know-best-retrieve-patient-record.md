---
name: Retrieve a patient's PKB health record
description: >-
  Authenticate to the Patients Know Best FHIR API and read a patient plus their
  clinical data (documents, observations, appointments) from the personal
  health record.
api: fhir/patients-know-best-facade-capabilitystatement.json
operations:
- Patient.read
- Patient.search
- Observation.search
- DocumentReference.search
- Appointment.search
---

# Retrieve a patient's PKB health record

Read a patient and their clinical data from the Patients Know Best (PKB) FHIR
STU3 (3.0.2) Facade API at `https://my.patientsknowbest.com/fhir`.

## Auth

1. Obtain an OAuth 2.0 access token with the **client-credentials** flow using
   the client id/secret provisioned for your integrating organisation.
2. Send `Authorization: Bearer <token>` on every request.
3. Use `Accept: application/fhir+json` (the server only returns
   `application/fhir+json`).

## Steps

1. **Find the patient.** Search `Patient` by NHS number identifier — this
   search *requires* the identifier parameter:
   `GET /fhir/Patient?identifier=https://fhir.nhs.uk/Id/nhs-number|<nhs-number>`.
   Every identifier must supply both a system and a value, or the request
   fails with an `OperationOutcome`. Read the returned patient id.
2. **Read observations/results.** `GET /fhir/Observation?patient=<id>&category=<code>&date=<range>`.
3. **Read documents.** `GET /fhir/DocumentReference?patient=<id>` (optionally
   filter by `created`, `document-status`, `source-organisation`).
4. **Read appointments.** `GET /fhir/Appointment?patient=<id>&date=<range>`.

## Rules

- Responses are FHIR `Bundle` (type `searchset`); page via `Bundle.link`
  (`next`/`previous`) with `_count`.
- Errors are FHIR `OperationOutcome` resources, not RFC 9457 problem+json —
  inspect `issue[].severity`, `issue[].code`, `issue[].diagnostics`
  (see `errors/patients-know-best-problem-types.yml`).
- Handle health data per GDPR / NHS DSP Toolkit obligations; only access
  records your consent scope permits.
