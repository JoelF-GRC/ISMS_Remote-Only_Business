# IT Security02 – Access Control & Identity Management Policy
(Annex A: A.5.15–A.5.23, A.8.2, A.8.3)

## Overview
CompanyX establishes identity and access management requirements to ensure that only authorized users, systems, and services can access CompanyX information assets across its remote-first, cloud-native environment. This policy consolidates Identity Lifecycle Management, Privileged Access Management (PIM/PAM), Separation of Duties (SoD), and authentication standards.

## Policy

### 1. Identity Lifecycle Management  
(Annex A: A.5.15, A.5.16)
- All user and service identities must be created, modified, and deprovisioned using standardized workflows.
- Identities must map to unique individuals or approved service principals.
- Shared accounts are prohibited unless formally approved with compensating controls.
- Offboarding actions must be completed within 24 hours of HR notification.
- Access rights must be reviewed at least quarterly.

### 2. Access Control Principles  
(Annex A: A.5.17, A.5.18)
- Access must follow least privilege and zero-trust principles.
- Access must be role-based (RBAC) or attribute-based (ABAC) where feasible.
- Default deny must be enforced across systems and networks.
- Access to production environments requires documented approval and logging.

### 3. Privileged Access Management (PIM/PAM)  
(Annex A: A.5.19, A.5.20)
- Administrative roles must use just-in-time elevation via Entra PIM or AWS IAM roles.
- Privileged actions must require MFA, session logging, and, where applicable, approval.
- Break-glass accounts must:
  - Be protected with MFA.
  - Be stored in a secure password vault.
  - Be reviewed monthly and tested at least twice per year.
- Standing administrative access is prohibited unless explicitly approved with documented justification and compensating controls.

### 4. Separation of Duties (SoD)  
(Annex A: A.5.21)
- No individual may deploy code to production without independent review.
- No individual may approve their own access requests or changes.
- Conflicts of duties must be identified, documented, and mitigated with evidence recorded in the risk register or access review records.
- SoD requirements apply across AWS, Entra, Jira, CI/CD pipelines, and administrative tools.

### 5. Authentication Requirements  
(Annex A: A.8.2, A.8.3)
- MFA is required for all user and administrator logins to Entra ID, AWS, VPN, and other critical systems.
- Passwords must meet CompanyX’s password standard (minimum length, complexity, and re-use restrictions) and must be changed if compromise is suspected.
- API keys and service account credentials must:
  - Be stored securely (e.g., in a secrets manager or vault).
  - Be rotated at least every 90 days, or more frequently where required.
- AWS IAM roles must be used instead of long-lived IAM users where possible.

### 6. Third-Party Access  
(Annex A: A.5.22)
- Third-party access must be limited to the minimum required, time bound, and contractually controlled.
- Vendors must use CompanyX-managed identities whenever technically feasible.
- All privileged third-party access must be monitored, logged, and periodically reviewed.

### 7. Monitoring and Detection  
(Annex A: A.5.23)
- Access logs must be collected and monitored for suspicious activity.
- Anomalous logins, privilege escalations, and geographic anomalies must generate alerts for investigation.
- Monitoring sources include, but are not limited to:
  - AWS CloudTrail
  - Entra ID sign-in and audit logs
  - CrowdStrike identity-related telemetry
  - Rapid7 detections and correlated alerts

## Policy Conflicts
This policy overrides any legacy access or account management procedures. Where conflicts exist between this policy and local procedures or guidelines, this policy is authoritative unless a more stringent requirement is documented elsewhere.

## Enforcement
Failure to follow this policy may result in revoked access, disciplinary action, or termination, subject to local laws and HR processes. Misuse of privileged access may trigger formal investigation and immediate credential suspension.

## Ownership
Security Department (Identity and Access Management Lead)

## Document Version History

| Version | Author             | Date       | Changes           | Approved By |
|---------|--------------------|------------|-------------------|-------------|
| 1.0     | Security Department| YYYY-MM-DD | Initial creation  | CISO / CTO  |
