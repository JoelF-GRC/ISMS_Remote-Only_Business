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
(Annex A: A.8.15)
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

### 6. Data Leakage Prevention  
(Annex A: A.8.12)
- CompanyX must implement controls to prevent unauthorized disclosure of sensitive information across channels including email, cloud storage, endpoint, and network egress.
- DLP controls must be configured to detect and alert on or block transmission of Confidential or Highly Confidential data to unauthorized destinations.
- Outbound data transfers from production environments must be monitored and, where technically feasible, inspected for sensitive content.
- DLP policy exceptions must be formally approved and logged.
- Incidents detected by DLP controls must be escalated per the Incident Response Policy (IT Security16).

### 7. Threat Intelligence  
(Annex A: A.5.7)
- CompanyX must maintain access to relevant cyber threat intelligence to inform risk decisions and detection tuning.
- Threat intelligence sources must include, at minimum:
  - Vendor security advisories (AWS, Microsoft, CrowdStrike, Rapid7)
  - Government and industry feeds (e.g., CISA KEV, NCSC alerts)
  - SIEM and XDR built-in threat intelligence integrations
- Threat intelligence findings must be reviewed by the Security team and used to update detection rules, patch priorities, and risk assessments where applicable.

### 8. Contact with Special Interest Groups  
(Annex A: A.5.6)
- The Security Department must maintain relationships with relevant external security groups and information-sharing communities to remain current on emerging threats and best practices.
- Participation may include:
  - Industry ISACs (Information Sharing and Analysis Centers) relevant to CompanyX's sector
  - Vendor security councils and early-warning programs
  - Professional bodies (e.g., ISC², ISACA, IAPP)
- Insights gained through external engagement must be shared internally as appropriate and used to inform the ISMS risk posture.

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
