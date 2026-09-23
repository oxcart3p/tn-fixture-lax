# Synthetic Test Evidence — CIS AWS Foundations Benchmark v1.2.0 Control 1.17

> **Test fixture only.** This document contains fictional contact details for validating the AWS Assurance GitHub-evidence and assessment workflow. It is not an attestation about a production AWS account and must not be used as real compliance evidence.

## Evidence record

| Field | Recorded value |
|---|---|
| AWS account | `127802951958` (Assurance test account) |
| Control | CIS AWS Foundations Benchmark v1.2.0 — 1.17 |
| Review date | 2026-09-23 |
| Reviewer role | Authorized Billing Administrator (synthetic test role) |
| Review location | AWS Management Console → Account → Account Settings → Contact Information |
| Review result | Contact information present, current, and mapped to multiple organizational recipients |
| Next scheduled review | 2026-12-23 |
| Test record ID | `TEST-CIS-1.17-20260923` |

## Current account contact configuration

The account contact record was reviewed in the AWS Management Console by a test operator representing a principal with permission to read and write Billing information.

| Contact field | Configured test value | Organizational routing |
|---|---|---|
| Account contact name | Example Corporation Cloud Operations | Team-owned function, not an individual |
| Email | `aws-account-contacts@example.com` | Distribution alias forwarding to Cloud Security Operations, Cloud Platform Operations, and Compliance Operations; at least three active recipients |
| Telephone | `+1-202-555-0100` | PBX hunt group that simultaneously routes to the primary and secondary cloud-operations on-call rotations, then escalates to the security duty manager |
| Postal address | Example Corporation, 100 Example Avenue, Seattle, WA 98101, US | Corporate operations address maintained by the account administration team |

The email alias and telephone hunt group are organizational resources. Neither depends on one individual being available.

## Verification performed

1. The reviewer opened **AWS Management Console → Account → Account Settings → Contact Information** for account `127802951958`.
2. The reviewer confirmed the displayed email address, telephone number, contact name, and postal address matched the configuration recorded above.
3. The reviewer confirmed the review session represented a role permitted to read and write AWS Billing account information.
4. A test message to `aws-account-contacts@example.com` was recorded as delivered to the Cloud Security Operations, Cloud Platform Operations, and Compliance Operations recipient groups.
5. A test call to `+1-202-555-0100` was recorded as reaching more than one on-call route through the PBX hunt group.
6. The reviewer confirmed the recipient groups have current membership owners and quarterly review schedules.
7. The next account-contact review was scheduled for 2026-12-23.

## Requirement mapping

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
