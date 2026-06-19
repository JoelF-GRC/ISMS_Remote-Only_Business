# IT Security13 – Operations Security Policy
(Annex A: A.5.37, A.8.6)

## Overview
CompanyX ensures secure and reliable operation of cloud services, production systems, and supporting infrastructure. This policy governs operational responsibilities, job scheduling, capacity management, and protection of operational processes.

## Policy

### 1. Operational Procedures  
(Annex A: A.5.37)
- Documented procedures must exist for:
  - Deployment processes
  - Production support
  - System maintenance
  - Backup and recovery
  - Incident response
- Procedures must be reviewed annually.

### 2. Change Control  
(Annex A: A.8.32)
- All changes to production systems must follow:
  - Change management workflow
  - Peer review
  - Testing requirements
  - Security assessment (if applicable)

### 3. Malware and Threat Protection  
(Annex A: A.8.7)
- Endpoints must be protected with CrowdStrike.
- Servers and workloads must use:
  - GuardDuty
  - Inspector
  - IAM least privilege controls
- Malicious activity must trigger alerts and investigation.

### 4. Capacity & Resource Management  
(Annex A: A.8.6)
- AWS resources must be monitored for:
  - CPU/Memory thresholds
  - Network usage
  - Autoscaling limits
- Capacity planning must occur quarterly.

### 5. Separation of Development, Test, and Production  
(Annex A: A.8.31)
- Environments must be isolated within AWS using separate accounts or VPCs.
- Test data must not include production data unless anonymized.

### 6. Event Logging and Monitoring  
(Annex A: A.8.15, A.8.16)
- All production systems must generate logs.
- Logs must be:
  - Centralized in SIEM
  - Monitored for anomalies
  - Retained according to policy

## Policy Conflicts
Where conflicts occur with product team operational requirements, this policy is authoritative unless an approved exception exists.

## Enforcement
Noncompliance may lead to disciplinary action or operational access suspension.

## Ownership
Security Department (Security Operations & Infrastructure)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-----------|--------------|-------------|
| 1.0 | Security Department | 2025-04-01 | Initial creation | CISO / CTO |
