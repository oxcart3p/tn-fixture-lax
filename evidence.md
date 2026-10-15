# Synthetic Test Evidence — CIS AWS Foundations Benchmark v1.2.0 Control 1.17

> **Test fixture only.** This document contains fictional contact details for validating the AWS Assurance GitHub-evidence and assessment workflow. It is not an attestation about a production AWS account and must not be used as real compliance evidence.


### 1.17-R1 — Contact details are current and up to date

**Synthetic test result: satisfied.** The account email, telephone number, contact name, and postal address were reviewed in AWS Account Settings on 2026-09-23. They matched the team-maintained account-contact record, and the next review date was scheduled.

### 1.17-R2 — Contact details map to more than one individual

**Synthetic test result: satisfied.** The email is a distribution alias with three organizational recipient groups. The telephone number is a PBX hunt group with primary, secondary, and security escalation routes. No contact path depends on one person.

### 1.17-R3 — Contact information was reviewed in the AWS Management Console

**Synthetic test result: satisfied.** An authorized Billing Administrator test role reviewed **Account Settings → Contact Information** and verified the displayed values against this record.

## Review and maintenance procedure

- Review frequency: quarterly and after any ownership, on-call, alias, PBX, or corporate-address change.
- Responsible function: Cloud Platform Operations.
- Secondary reviewer: Cloud Security Operations.
- Exceptions: stale recipients, failed alias delivery, failed PBX routing, or mismatched AWS Account Settings values require correction before the review can be marked complete.
- Evidence retention: retain the review record and supporting delivery/call-test artifacts according to the test environment's evidence-retention policy.

## Synthetic-fixture limitation

The domains, telephone number, reviewer role, delivery result, and call result in this file are fictional. A real assessment requires actual AWS Account Settings output and verifiable organizational routing records. This fixture exists only to test whether Assurance can retrieve a GitHub file, link it to CIS control 1.17, evaluate requirements R1–R3, and produce assessment journal entries, annotations, and tasks.
