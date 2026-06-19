# IT Security15 – Cloud Security Policy
(Annex A: A.5.23, A.8.20–A.8.23)

## Overview
CompanyX operates primarily in AWS and Entra ID. This policy governs secure use, configuration, monitoring, and administration of cloud services to ensure confidentiality, integrity, and availability of cloud resources.

## Policy

### 1. Identity & Access in Cloud Environments  
(Annex A: A.5.15–A.5.18, A.5.23)
- MFA is required for all cloud administrative access.
- AWS IAM users are prohibited except for break-glass accounts.
- Entra ID roles and AWS IAM roles must follow least privilege principles.
- Access reviews must be conducted quarterly.

### 2. AWS Security Controls  
(Annex A: A.8.20–A.8.23)
- Mandatory configurations include:
  - CloudTrail enabled organization-wide
  - GuardDuty enabled for all accounts
  - VPC Flow Logs enabled
  - S3 buckets encrypted and block-public-access enabled
  - KMS encryption for data stores (RDS, EBS, S3, DynamoDB)
- Publicly accessible resources require Security approval.

### 3. Entra ID Security Controls  
- Conditional Access must be enabled for all users.
- Risky logins must trigger MFA, identity risk policies, or account review.
- Applications must use:
  - SSO where possible
  - OAuth/OIDC with approved security settings

### 4. Cloud Monitoring & Telemetry  
- Logs must be sent to central SIEM (Rapid7).
- AWS logs must be immutable where possible.
- Anomalous activity (privilege escalation, unusual API calls, geolocation anomalies) must trigger alerts.

### 5. Secure Cloud Architecture Requirements  
- Workloads must use:
  - Private subnets
  - Security groups enforcing least privilege
  - Autoscaling and load balancing best practices
  - Multi-AZ deployments for resilience
- Containers and serverless functions must undergo:
  - Dependency scanning
  - IAM privilege review
  - Environment variable protection

### 6. Cloud Resource Lifecycle  
- Provisioning must occur through IaC where feasible.
- Decommissioned resources must be securely deleted.
- Tags must include ownership, environment, and classification metadata.

## Policy Conflicts
This policy supersedes team-specific cloud configuration exceptions unless formally approved.

## Enforcement
Unauthorised cloud modifications may result in access removal, investigation, or disciplinary action.

## Ownership
Security Department (Cloud Security & Architecture)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-----------|--------------|-------------|
| 1.0 | Security Department | 2025-04-01 | Initial creation | CISO / CTO |
