# IT Security07 – Logging, Monitoring & Security Event Management Policy
(Annex A: A.8.15, A.8.16, A.8.17, A.8.12, A.5.6, A.5.7)

## Overview
CompanyX collects, monitors, and analyzes security logs from critical systems to detect, investigate, and respond to threats. This policy defines requirements for log generation, retention, SIEM correlation, and real-time security monitoring.

## Policy

### 1. Logging Requirements  
(Annex A: A.8.15, A.8.16)
- Logs must be enabled for:
  - AWS CloudTrail (organization-level)
  - VPC Flow Logs
  - ALB/WAF logs
  - Entra ID sign-in and audit logs
  - Endpoint events (CrowdStrike)
  - CI/CD pipelines
- Logs must include timestamps, event types, user identity, and results.

### 2. Log Protection and Retention  
(Annex A: A.8.15, A.8.12)
- Logs must be stored in:
  - Centralized SIEM (Rapid7)
  - Immutable storage where applicable
- Logs must be protected from alteration and unauthorized access.
- Retention must follow CompanyX’s data retention schedule (typically 12–24 months).

### 3. Security Monitoring  
(Annex A: A.8.16)
- Monitoring tools include:
  - Rapid7 SIEM
  - CrowdStrike XDR
  - AWS GuardDuty
  - AWS Inspector
- Security alerts must be triaged and investigated promptly.

### 4. Event Correlation and Detection  
(Annex A: A.8.16)
- Events must be correlated across identity, endpoint, network, and cloud data sources.
- High-risk detections (impossible travel, privilege escalation, anomalous logins) must generate alerts.

### 5. Time Synchronization  
(Annex A: A.8.17)
- All servers, endpoints, and cloud services must use reliable time sources (e.g., NTP, AWS Time Sync Service).
- Time drift must be corrected automatically.

## Policy Conflicts
Where conflicts exist between this policy and operational procedures, the stricter logging requirement applies.

## Enforcement
Failure to comply may result in disciplinary action up to termination. Intentional log tampering may result in immediate investigation.

## Ownership
Security Department (Security Operations)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-------|----------|--------------|
| 1.0 | Security Department | YYYY-MM-DD | Initial creation | CISO / CTO |
