# IT Security05 – Asset Management & Information Classification Policy
(Annex A: A.5.9, A.5.12, A.5.13, A.8.10)

## Overview
CompanyX maintains an accurate inventory of information assets and classifies information according to its sensitivity. This policy ensures assets are protected throughout their lifecycle and that classification requirements dictate appropriate handling controls.

## Policy

### 1. Asset Inventory  
(Annex A: A.5.9)
- All information assets must be inventoried, including:
  - Cloud resources (AWS accounts, VPCs, EC2, RDS, Lambda, S3 buckets)
  - Endpoints (laptops, mobile devices)
  - SaaS platforms (Jira, GitHub, Google Workspace, Entra ID)
  - Data repositories and logs
- Each asset must have an **owner**, **classification**, and **protection requirements**.
- The inventory must be reviewed at least quarterly.

### 2. Information Classification  
(Annex A: A.5.12)
CompanyX uses four data classifications:
- **Public** – Approved for external disclosure
- **Internal** – Default classification; internal use only
- **Confidential** – Restricted to authorized users based on role
- **Highly Confidential** – Sensitive data requiring enhanced controls (e.g., encryption, strict access controls)

### 3. Handling Requirements  
(Annex A: A.5.13)
- Confidential and Highly Confidential data must be encrypted in transit and at rest.
- Transmission of sensitive data must occur through approved, encrypted channels.
- Data must not be stored on personal devices.
- Sensitive data must not be emailed externally without encryption.

### 4. Asset Handling and Lifecycle  
(Annex A: A.8.10, A.7.14)
- Asset onboarding must include tagging, ownership assignment, and classification.
- Asset changes (e.g., redeployment, migration) must preserve classification and security requirements.
- At end of life:
  - AWS resources must be securely deleted.
  - Endpoints must undergo secure wipe procedures.
  - Logs and data must be retained or destroyed according to retention schedules.

## Policy Conflicts
If conflicts arise between this policy and other operational procedures, the stricter handling requirement applies.

## Enforcement
Violations may result in disciplinary action, including termination. Mishandling sensitive data may result in immediate access revocation.

## Ownership
Security Department (Asset & Data Governance)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-------|----------|--------------|
| 1.0 | Security Department | YYYY-MM-DD | Initial creation | CISO / CTO |
