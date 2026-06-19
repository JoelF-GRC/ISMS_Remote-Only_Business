# IT Security12 – Physical & Data Center Security Policy
(Annex A: A.7.1–A.7.9, A.7.11, A.7.13–A.7.14, A.6.7)

## Overview
CompanyX operates as a remote-first SaaS provider with no dedicated corporate offices. Physical security relates primarily to employee endpoints, approved coworking environments, and third-party data centers hosting cloud infrastructure (e.g., AWS). This policy defines minimum controls for safe physical handling and protection of assets.

Remote working security requirements (A.6.7) are fully defined in IT Security20 (Remote Working Policy). This policy covers the physical and endpoint security aspects of remote work locations and devices.

## Policy

### 1. Data Center Controls (AWS and Third-Party Facilities)  
(Annex A: A.7.1, A.7.2, A.7.4)
- AWS and other cloud providers must maintain:
  - 24/7 staffed security
  - CCTV and access logging
  - Biometric and badge-based access
  - Environmental controls (HVAC, fire suppression)
  - Redundant power and network paths
- CompanyX relies on AWS SOC 2/ISO 27001 assurances for physical controls.

### 2. Employee Endpoint Physical Security  
(Annex A: A.7.9)
- Devices must be:
  - Encrypted (FileVault/BitLocker)
  - MDM-managed
  - Screen-locked when unattended
  - Secured during travel with physical protections (bags, cable locks)
- Employees must not leave devices unattended in public spaces.

### 3. Remote Work Location Requirements  
(Annex A: A.7.3, A.7.7, A.6.7)
- Employees must:
  - Work in locations where unauthorized individuals cannot view screens
  - Use privacy shields when necessary
  - Secure home Wi-Fi using WPA2/WPA3 encryption
- Work in coworking spaces requires:
  - Private room or secure workspace
  - No confidential conversations in shared areas

### 4. Visitor and Access Controls  
(Annex A: A.7.6)
- Visitors to locations where CompanyX assets are used must not have unsupervised access to devices.
- Employees must store devices securely when not in use (locked rooms, drawers, safes).

### 5. Asset Handling  
(Annex A: A.7.14, A.7.9)
- End-of-life assets must be securely wiped before disposal.
- Lost or stolen devices must be reported to Security within 1 hour.

## Policy Conflicts
This policy supersedes any legacy on-premise physical security procedures.

## Enforcement
Violations may result in disciplinary action. Failure to report lost/stolen devices may result in immediate investigation.

## Ownership
Security Department (Corporate Security)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-----------|----------------|-------------|
| 1.0 | Security Department | 2025-04-01 | Initial creation | CISO / CTO |
