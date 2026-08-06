# APACGA ID Full Package

## Purpose

The APACGA ID Full Package defines a complete identity governance and customer due diligence package for APACGAMONDE banking, compliance, audit, and operational teams. It is designed to support controlled onboarding, identity verification, risk classification, approval workflows, and periodic review while preserving auditability.

## Package Contents

| Component | File | Purpose |
| --- | --- | --- |
| Identity SOP | `templates/APACGA_ID_SOP_Template.md` | Standard operating procedure for APACGA ID creation, verification, approval, maintenance, and closure. |
| KYC intake form | `templates/APACGA_ID_KYC_Intake_Form.md` | Structured intake checklist for individuals, entities, beneficial owners, and authorized signatories. |
| Risk matrix | `templates/APACGA_ID_Risk_Matrix.csv` | Scoring template for country, customer, product, channel, PEP, sanctions, and adverse media risk. |
| Compliance checklist | `templates/APACGA_ID_Compliance_Checklist.md` | Control checklist mapped to KYC, CDD, EDD, AML/CFT, sanctions, privacy, audit, and record retention obligations. |
| Audit log | `templates/APACGA_ID_Audit_Log_Template.csv` | Evidence register for approvals, changes, exceptions, and periodic reviews. |

## Operating Principles

1. **Single accountable identity record** — every customer, beneficial owner, employee, agent, vendor, or authorized signatory must have one controlled APACGA ID record.
2. **Risk-based due diligence** — verification depth and approval level must increase as risk score increases.
3. **No undocumented exceptions** — any deviation from standard controls requires a documented reason, owner, expiry date, and approval.
4. **Segregation of duties** — the person creating or updating an APACGA ID should not be the sole approver.
5. **Audit-ready evidence** — all identity decisions must be traceable to supporting documentation and timestamped approvals.
6. **Periodic refresh** — APACGA IDs must be reviewed on a scheduled cycle based on risk rating.

## APACGA ID Lifecycle

### 1. Request

- Capture requester name, department, business purpose, customer or party type, jurisdiction, and requested effective date.
- Confirm that a duplicate APACGA ID does not already exist.
- Assign a temporary case reference until approval is complete.

### 2. Intake

- Complete the APACGA ID KYC intake form.
- Collect required identity, registration, address, ownership, authorization, tax, and contact evidence.
- Record document source, document number, issuing authority, issue date, expiry date, and verification method.

### 3. Screening

- Perform sanctions, watchlist, politically exposed person, adverse media, fraud, and internal blacklist screening.
- Record screening provider, screening date, match outcome, analyst decision, and reviewer approval.
- Escalate true matches and unresolved potential matches before any APACGA ID activation.

### 4. Risk Assessment

- Score the case using the APACGA ID risk matrix.
- Assign low, medium, high, or prohibited risk classification.
- Document enhanced due diligence for high-risk cases.

### 5. Approval

- Route approval according to the risk-based approval table.
- Require dual approval for high-risk, PEP, cross-border, shell-company, nominee, or exception cases.
- Activate the APACGA ID only after required approvals are complete.

### 6. Maintenance

- Update APACGA ID details when legal name, ownership, address, risk profile, authorizations, documents, or relationship purpose changes.
- Re-screen material changes before approval.
- Preserve previous values in the audit log.

### 7. Review

- Low risk: review at least every 36 months.
- Medium risk: review at least every 24 months.
- High risk: review at least every 12 months.
- Triggered review: perform immediately after sanctions alerts, adverse media, ownership changes, unusual activity, law enforcement requests, or internal control findings.

### 8. Suspension or Closure

- Suspend the APACGA ID when verification fails, approvals expire, documents lapse, sanctions matches are unresolved, or the relationship becomes prohibited.
- Close the APACGA ID when the relationship ends and retention requirements are satisfied.
- Keep records according to applicable legal and audit retention schedules.

## Required Minimum Data Fields

| Category | Required fields |
| --- | --- |
| APACGA ID metadata | APACGA ID, case reference, status, type, created date, created by, approved by, effective date, review date. |
| Individual identity | Full legal name, date of birth, nationality, ID document, address, phone, email, occupation, source of funds. |
| Entity identity | Legal name, registration number, registration country, legal form, registered address, operating address, business activity, tax ID. |
| Ownership and control | Beneficial owners, ownership percentages, directors, controllers, authorized signatories, authorization evidence. |
| Risk and compliance | Risk score, risk rating, sanctions result, PEP result, adverse media result, EDD status, approval level. |
| Evidence | Document type, document number, source, verification method, expiry date, storage reference, reviewer notes. |

## Risk-Based Approval Table

| Risk classification | Approval requirement | Review frequency |
| --- | --- | --- |
| Low | Operations maker and compliance checker | 36 months |
| Medium | Operations maker, compliance checker, line manager | 24 months |
| High | Operations maker, compliance checker, compliance manager, business owner | 12 months |
| Prohibited | Reject or suspend; compliance head decision required for any regulatory report | Immediate escalation |

## Implementation Checklist

- [ ] Assign APACGA ID owner and compliance control owner.
- [ ] Configure unique ID generation and duplicate detection.
- [ ] Implement maker-checker approval workflow.
- [ ] Connect sanctions, PEP, adverse media, and internal fraud screening.
- [ ] Define secure evidence storage and retention schedule.
- [ ] Train staff on intake, screening, risk scoring, escalation, and audit logging.
- [ ] Run a 30-90 day pilot and document findings.
- [ ] Complete legal, compliance, audit, and management sign-off.

## Governance

This package should be reviewed at least annually or sooner when regulations, sanctions obligations, product scope, operating jurisdictions, risk appetite, or audit findings change.
