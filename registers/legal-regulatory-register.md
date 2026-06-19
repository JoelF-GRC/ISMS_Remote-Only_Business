# CompanyX Legal & Regulatory Compliance Register
ISO/IEC 27001:2022 Annex A: A.5.31, A.5.32, A.5.34
Last Updated: 2025-05-01

## Purpose
Maintain a living inventory of legal, regulatory, and contractual obligations relevant to information security, satisfying A.5.31 (Legal, statutory, regulatory and contractual requirements), A.5.32 (Intellectual property rights), and A.5.34 (Privacy and protection of PII).

## Register

| Obligation | Source | Applicable To | Requirement Summary | Compliance Status | Evidence / Control Reference | Owner | Review Date |
|------------|--------|----------------|------------------------|----------------------|---------------------------------|-------|--------------|
| GDPR | EU Regulation 2016/679 | EU customer/employee personal data | Lawful basis for processing, data subject rights, breach notification within 72 hours | Compliant | IT Security05, IT Security16, Vendor DPAs | GRC | |
| CCPA/CPRA | California state law | California consumer personal data (if applicable) | Consumer rights to access/delete data, opt-out of sale | Compliant | IT Security05, Privacy Policy | GRC | |
| SOC 2 customer commitments | Customer contracts | All production systems | Security, availability, confidentiality criteria per contractual commitments | Compliant | soa.md, IT Security07/08/15 | GRC | |
| Employment & data protection law (jurisdiction-specific) | Local labor/privacy law per employee location | Employee personal data (remote workforce) | Lawful handling of employee data across jurisdictions | Compliant | HR Policy, IT Security05 | HR/GRC | |
| Breach notification laws | Applicable national/state law | All systems processing personal data | Notify regulators/affected individuals within statutory timeframes | Compliant | IT Security16 (Incident Response) | GRC/Legal | |
| Cloud provider terms (AWS) | AWS Customer Agreement | AWS-hosted infrastructure | Shared responsibility model compliance | Compliant | scope.md, asset-register.md | Cloud/GRC | |
| Intellectual property licensing | Software vendor licenses (GitHub, Jira, etc.) | All licensed software/SaaS | Compliance with license terms and seat counts | Compliant | vendor-register.md | IT/GRC | |

---

## Review
This register must be reviewed at least annually, and immediately upon entry into new jurisdictions, new customer contracts with security/compliance clauses, or new regulatory developments affecting the business.

## Ownership
GRC, with Legal counsel input where applicable.
