# IT Security09 – Secure Development & Change Management Policy
(Annex A: A.8.25, A.8.28, A.8.32, A.8.11, A.5.8, A.5.21)

## Overview
CompanyX implements secure software development practices and formal change management processes to ensure that applications, infrastructure, and configurations are deployed safely, reviewed appropriately, and monitored for unauthorized changes.

## Policy

### 1. Secure Development Requirements  
(Annex A: A.8.28)
- Developers must be trained in secure coding practices annually.
- Code must follow OWASP, CIS, and CompanyX secure coding standards.
- Secrets must not be stored in source code repositories.
- Automated static and dynamic analysis (SAST/DAST) must be integrated into CI/CD pipelines.

### 2. Code Review and Separation of Duties  
(Annex A: A.5.3)
- All production code must undergo peer review.
- Developers may not approve their own pull requests.
- Production deployments must be performed by authorized personnel via CI/CD pipelines.

### 3. Third-Party Libraries and Dependencies  
- Dependencies must be tracked using SCA (Software Composition Analysis).
- Known vulnerable libraries must be updated promptly based on severity.
- Only approved repositories and registries may be used.

### 4. Change Management Requirements  
(Annex A: A.8.32)
- All production changes must follow a documented change process.
- Changes must include:
  - Description
  - Risk assessment
  - Rollback plan
  - Testing evidence
  - Approval by authorized reviewers
- Emergency changes require retrospective review within 5 business days.

### 5. Infrastructure-as-Code (IaC)  
- IaC must be used for AWS where feasible.
- Templates must undergo:
  - Code scanning (Checkov, tfsec, cfn-nag)
  - Peer review
  - Version control in GitHub

### 6. Data Masking  
(Annex A: A.8.11)
- Production data containing PII or Confidential information must not be used in development, testing, or staging environments without prior masking or anonymization.
- Approved data masking techniques include tokenization, pseudonymization, data substitution, and format-preserving encryption.
- Masked datasets must be generated from production snapshots using approved tooling and must not be reversible without explicit authorization.
- Data masking requirements must be incorporated into the development lifecycle and validated as part of pre-production sign-off.

### 7. Secrets and Key Use in Development  
(Annex A: A.8.25)
- Secrets must be stored in secure vaults (AWS Secrets Manager, Parameter Store).
- Keys must be rotated regularly and must not appear in logs or repositories.

## Policy Conflicts
Where development velocity conflicts with security standards, security requirements take precedence unless an approved exception is documented.

## Enforcement
Unauthorized or undocumented production changes may result in disciplinary action up to termination.

## Ownership
Security Department (Application Security & DevOps)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|---------|-----------|--------------|--------------|
| 1.0 | Security Department | YYYY-MM-DD | Initial creation | CISO / CTO |
