# IT Security16 – Incident Response Policy
(Annex A: A.5.5, A.5.24–A.5.27, A.6.8)

## Overview
CompanyX maintains a structured approach to detecting, reporting, triaging, investigating, and resolving security incidents. This policy ensures effective response that minimizes impact and preserves evidence.

## Policy

### 1. Incident Identification  
(Annex A: A.6.8, A.5.24)
- Incidents may be detected via:
  - SIEM alerts (Rapid7)
  - CrowdStrike detections
  - GuardDuty findings
  - User reports
  - External threat intelligence
- All suspected incidents must be reported immediately to Security.

### 2. Incident Classification  
Incidents must be classified by severity:
- **Low**: Minimal impact, easily contained  
- **Medium**: Limited data or system exposure  
- **High**: Compromise of sensitive data, privileged accounts  
- **Critical**: Widespread impact, ongoing exploitation, ransomware

### 3. Incident Handling Procedures  
(Annex A: A.5.26)
- Incident handlers must follow:
  - Containment
  - Eradication
  - Recovery
  - Forensic evidence preservation
- All steps must be documented in the incident tracking system (e.g., Jira).

### 4. Communication Requirements  
(Annex A: A.5.5, A.5.26)
- Internal communications must be coordinated by Security and leadership.
- External communications (customers, regulators) require approval from:
  - Legal
  - Leadership
  - Security
- Sensitive incident details must not be shared via unencrypted channels.

### 5. Post-Incident Review  
(Annex A: A.5.27)
- After major incidents, a post-incident report (PIR) must be completed within 10 business days.
- PIR must include:
  - Root cause analysis
  - Lessons learned
  - Required control improvements
- All corrective actions must be tracked to closure.

## Policy Conflicts
This policy overrides any informal or undocumented incident handling practices.

## Enforcement
Failure to report or properly handle incidents may result in disciplinary action.

## Ownership
Security Department (Security Operations & Incident Response)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-----------|--------------|-------------|
| 1.0 | Security Department | 2025-04-01 | Initial creation | CISO / CTO |
