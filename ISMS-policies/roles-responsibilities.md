# ISMS Roles & Responsibilities (RACI Matrix)
ISO/IEC 27001:2022 Clause 5.3, Annex A: A.5.2
Last Updated: 2025-02-15

## Purpose
Define and communicate roles, responsibilities, and authorities for the ISMS, satisfying Clause 5.3 (Organizational roles, responsibilities and authorities) and A.5.2 (Information security roles and responsibilities). This matrix complements the individual policies, which describe *what* must be done — this document clarifies *who* is accountable for ensuring it happens.

## RACI Legend
- **R** – Responsible: performs the work
- **A** – Accountable: ultimately answerable for correctness and completion (one per activity)
- **C** – Consulted: provides input before/during the activity
- **I** – Informed: kept up to date on progress or outcomes

## Roles Referenced
- **Leadership** – CISO / CTO
- **Security** – Security Department / ISMS Manager
- **IAM** – Identity & Access Management Lead
- **Cloud** – Cloud/Infrastructure Team
- **Engineering** – Product Engineering
- **SecOps** – Security Operations
- **GRC** – Governance, Risk & Compliance
- **IT** – IT/Helpdesk
- **DevOps** – DevOps/CI-CD
- **HR** – Human Resources

---

## RACI Matrix

| ISMS Activity | Leadership | Security | IAM | Cloud | Engineering | SecOps | GRC | IT | DevOps | HR |
|----------------|------------|----------|-----|-------|-------------|--------|-----|----|--------|----|
| ISMS scope, policy approval (Clause 4–5) | A | R | I | I | I | I | C | I | I | I |
| Risk assessment & methodology (Clause 6.1) | I | A/R | C | C | C | C | R | I | I | I |
| Risk register maintenance | I | A | C | C | C | C | R | I | I | I |
| Risk treatment plan execution | I | A | R | R | R | R | C | R | R | I |
| Statement of Applicability maintenance | A | R | I | I | I | I | C | I | I | I |
| Information security objectives & KPIs | A | R | I | I | I | C | C | I | I | I |
| Internal audit program | A | R | C | C | C | C | C | I | I | I |
| Management review | A | R | I | I | I | I | C | I | I | I |
| Corrective actions / nonconformities | I | A | C | C | C | C | R | I | I | I |
| Access control & identity lifecycle | I | A | R | C | C | I | I | C | I | C |
| Privileged access management (PIM/PAM) | I | A | R | C | I | I | I | I | C | I |
| Asset inventory & classification | I | A | I | R | R | I | C | C | I | I |
| Vendor / third-party risk management | C | A | I | C | I | I | R | I | I | I |
| Cryptography & key management | I | A | C | R | R | I | I | I | C | I |
| Network & infrastructure security | I | A | I | R | C | C | I | C | C | I |
| Secure configuration & hardening | I | A | I | R | R | C | I | C | C | I |
| Logging, monitoring & SIEM | I | A | C | R | C | R | I | I | C | I |
| Vulnerability & patch management | I | A | I | R | R | C | I | C | C | I |
| Secure development & change management | I | C | I | C | A/R | I | I | I | R | I |
| Backup & recovery | I | A | I | R | C | I | I | C | C | I |
| Malware protection & endpoint security | I | A | C | I | I | R | I | R | I | I |
| Cloud security configuration | I | A | C | R | C | C | I | I | C | I |
| Incident response | I | A | C | R | C | R | C | R | C | I |
| Business continuity & disaster recovery | A | R | C | R | C | C | C | C | C | C |
| Compliance, audit & legal/regulatory tracking | C | A | I | I | I | I | R | I | I | I |
| Physical & remote workspace security | I | A | I | I | I | I | I | R | I | C |
| Security awareness training | A | R | I | I | I | I | C | I | I | R |
| Onboarding / offboarding (account lifecycle) | I | C | R | I | I | I | I | C | I | A/R |
| Document control & version management | I | A/R | I | I | I | I | C | I | I | I |
| Climate/environmental risk review (BCDR input) | A | R | I | C | I | I | C | I | I | C |

---

## Review
This matrix must be reviewed annually, after significant organizational changes, or following any restructuring of the Security Department. Updates require Leadership approval.

## Ownership
Security Department (ISMS Manager)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|---------|---------|------------|----------------|--------------|
| 1.0 | Security Department | 2025-02-15 | Initial creation | CISO / CTO |
