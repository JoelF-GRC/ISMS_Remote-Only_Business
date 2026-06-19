# IT Security20 – Remote Working Policy
(Annex A: A.6.7, A.7.7, A.7.9)

## Overview
CompanyX operates as a fully remote organization with no dedicated corporate offices. All employees and contractors work from home or approved remote locations. This policy defines the minimum security requirements for remote work environments to ensure that the absence of a traditional office perimeter does not compromise the confidentiality, integrity, or availability of CompanyX information and systems.

This policy is primary for A.6.7 (Remote working). Physical device and endpoint requirements are further defined in IT Security12 (Physical & Data Center Security Policy). Acceptable use obligations are defined in IT Security19 (Acceptable Use Policy).

## Policy

### 1. Remote Work Environments  
(Annex A: A.6.7, A.7.3)
- Employees must perform work from locations where unauthorized individuals cannot view their screens or overhear confidential conversations.
- Screen privacy filters must be used when working in shared or public spaces (e.g., coworking areas, cafés).
- Confidential calls and discussions must not be conducted in environments where non-CompanyX individuals can hear.
- Approved remote work locations include:
  - Employee home offices
  - Private rooms in coworking facilities
- Shared open-plan coworking spaces are permitted only for non-sensitive tasks and must not involve the display of Confidential or Highly Confidential data.

### 2. Network Access and VPN  
(Annex A: A.6.7, A.8.20)
- All access to CompanyX production systems, internal tools, and Confidential data must occur over:
  - A CompanyX-approved VPN or Zero Trust Network Access (ZTNA) solution, or
  - Secure, direct cloud application access protected by MFA and Conditional Access policies
- Public or untrusted Wi-Fi (e.g., airport, café, hotel) must not be used for CompanyX work without an active VPN or ZTNA tunnel.
- Home networks must use WPA2 or WPA3 encryption. Default router credentials must be changed.
- Employees are responsible for ensuring home routers are patched and free of unauthorized connected devices.

### 3. Approved Devices  
(Annex A: A.6.7, A.7.9, A.8.1)
- Only CompanyX-issued or formally approved BYOD devices may be used to access CompanyX systems and data.
- All approved devices must:
  - Be encrypted (FileVault for macOS, BitLocker for Windows)
  - Be enrolled in CompanyX's Mobile Device Management (MDM) solution
  - Have endpoint detection and response (EDR) software installed and active
  - Have automatic screen locking configured (maximum 5 minutes of inactivity)
  - Run current, supported operating system versions
- Personal devices used for CompanyX work under an approved BYOD program must meet equivalent security baseline requirements.
- Family members and non-authorized individuals must not use CompanyX devices.

### 4. Clear Screen and Physical Security at Home  
(Annex A: A.7.7, A.7.9)
- Employees must lock or log out of all CompanyX systems when leaving their workstation, even briefly.
- CompanyX devices must not be left unattended and unlocked in any location, including at home.
- Sensitive documents (printed materials, notes) must be stored securely and shredded when no longer needed.
- Devices must be stored securely when not in use (e.g., locked room, locked drawer).
- Employees must report lost or stolen devices to the Security Department within 1 hour of discovery.

### 5. Approved Communication Tools  
(Annex A: A.6.7, A.5.14)
- CompanyX business must be conducted only through company-approved communication platforms (e.g., Microsoft Teams, Slack, corporate email).
- Personal email accounts, personal SMS, or unapproved messaging platforms must not be used to transmit CompanyX data.
- Confidential or Highly Confidential information must not be shared in group channels or tools where the audience cannot be controlled.

### 6. Remote Work and Data Handling  
(Annex A: A.5.12, A.5.13)
- Data classification rules from IT Security05 (Asset Management & Information Classification Policy) apply in full to remote work environments.
- Printing of CompanyX data at home is strongly discouraged. Where necessary, printed documents must be stored securely and disposed of via cross-cut shredding.
- Local copies of CompanyX data on personal or home drives are prohibited unless explicitly required and approved by the Security Department.

### 7. Secure Disposal of Assets  
(Annex A: A.7.14)
- End-of-life devices must be returned to the Security Department or disposed of per the secure disposal process defined in IT Security12.
- Employees must not personally dispose of CompanyX devices or storage media.

### 8. Incident Reporting While Remote  
(Annex A: A.6.8)
- Employees must report security incidents, suspicious activity, or policy violations regardless of location.
- Incident reporting must follow the process defined in IT Security16 (Incident Response Policy).
- If a device is lost, stolen, or suspected of compromise, the Security Department must be contacted immediately.

### 9. Remote Working Agreements  
(Annex A: A.6.7)
- All employees and contractors must acknowledge and accept this policy as a condition of employment.
- Remote working arrangements must be reviewed annually or when job role or location changes.

## Policy Conflicts
This policy takes precedence over informal remote work arrangements. Where conflicts arise with local jurisdiction requirements, Legal must be consulted.

## Enforcement
Violations of this policy may result in disciplinary action, revocation of remote work privileges, or termination of employment or contract.

## Ownership
Security Department (Workforce & Endpoint Security)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-----------|--------------|-------------|
| 1.0 | Security Department | 2026-06-12 | Initial creation | CISO / CTO |
