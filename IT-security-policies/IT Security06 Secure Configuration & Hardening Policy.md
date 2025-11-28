# IT Security06 – Secure Configuration & Hardening Policy
(Annex A: A.8.8, A.8.9, A.8.10)

## Overview
CompanyX enforces secure configuration standards for systems, cloud services, network components, and endpoints. This policy ensures systems are deployed, maintained, and monitored using hardened baselines aligned with industry best practices.

## Policy

### 1. Baseline Hardening Requirements  
(Annex A: A.8.8)
- All systems must follow documented hardening baselines, including:
  - CIS Benchmarks (AWS, Linux, Windows, macOS)
  - Secure configuration standards for containers and serverless services
  - Restrictions on insecure services and ports
- Baselines must be reviewed annually.

### 2. Configuration Management  
(Annex A: A.8.9)
- Infrastructure-as-code (IaC) must be used for AWS where feasible (CloudFormation, Terraform).
- Manual changes to production configurations are prohibited unless approved under emergency change procedures.
- Changes must be logged, version-controlled, and traceable to an authorized requester.

### 3. Endpoint Configuration  
(Annex A: A.8.10)
- All endpoints must be:
  - Encrypted (FileVault, BitLocker)
  - Protected by CrowdStrike
  - Managed through MDM with enforced policies
  - Configured with local firewalls enabled
- Administrative rights for endpoints require Security approval.

### 4. Cloud Service Configuration  
- AWS resources must enforce:
  - Private subnets for data workloads
  - Security groups with least privilege rules
  - IMDSv2 for EC2
  - S3 bucket encryption and block-public-access
- Entra ID must enforce:
  - Conditional Access
  - MFA
  - Session controls

### 5. Configuration Drift Detection  
- Automated tools must monitor for drift (AWS Config, Inspector, MDM alerts).
- Drift events must trigger investigation and corrective action.

## Policy Conflicts
If procedures conflict with these baselines, exceptions must be documented and risk accepted by the Security Department.

## Enforcement
Noncompliance may result in revoked privileges or disciplinary action. Critical misconfigurations may trigger incident response.

## Ownership
Security Department (Security Engineering)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-------|----------|--------------|
| 1.0 | Security Department | YYYY-MM-DD | Initial creation | CISO / CTO |
