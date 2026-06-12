# Statement of Applicability (SoA)
CompanyX ISO/IEC 27001:2022  
Last Updated: YYYY-MM-DD

## Purpose
This Statement of Applicability (SoA) lists all Annex A controls from ISO/IEC 27001:2022, declares whether each control is applicable to CompanyX, and identifies the justification and implementation reference.

This version uses the four ISO audit–preferred justification categories:

### Justification Categories
- **Regulatory Requirement** – Mandated by law, regulation, or contract.
- **Organizational Requirement** – Needed to meet business, customer, or operational needs.
- **Best Practice** – Based on industry standards, ISO/NIST/SOC 2 expectations, or secure-by-design principles.
- **Risk-Based Requirement** – Necessary to treat identified risks.

---

# ANNEX A CONTROLS

---

# A.5 — Organizational Controls

| Control | Description | Applicable? | Justification | Reference |
|--------|-------------|-------------|---------------|-----------|
| A.5.1 | Information security policies | Yes | Best Practice | IT Security01 |
| A.5.2 | Roles and responsibilities | Yes | Organizational Requirement | roles-responsibilities.md |
| A.5.3 | Segregation of duties | Yes | Risk-Based Requirement | IT Security02 |
| A.5.4 | Management responsibilities | Yes | Organizational Requirement | management-overview.md |
| A.5.5 | Contact with authorities | Yes | Regulatory Requirement | Incident Response Policy |
| A.5.6 | Special-interest groups | Yes | Best Practice | IT Security07 |
| A.5.7 | Threat intelligence | Yes | Best Practice | IT Security07 |
| A.5.8 | Risk assessment | Yes | Regulatory Requirement | risk-methodology.md |
| A.5.9 | Inventory of assets | Yes | Best Practice | IT Security05 |
| A.5.10 | Acceptable use | Yes | Organizational Requirement | IT Security19 |
| A.5.11 | Return of assets | Yes | Organizational Requirement | HR Offboarding Procedures |
| A.5.12 | Information classification | Yes | Risk-Based Requirement | IT Security05 |
| A.5.13 | Information handling | Yes | Best Practice | IT Security05 |
| A.5.14 | Labeling of information | Yes | Best Practice | IT Security05 |
| A.5.15 | Access control | Yes | Regulatory Requirement | IT Security02 |
| A.5.16 | Identity management | Yes | Best Practice | IT Security02 |
| A.5.17 | Authentication | Yes | Best Practice | IT Security02 |
| A.5.18 | Authorization | Yes | Risk-Based Requirement | IT Security02 |
| A.5.19 | Privileged access | Yes | Risk-Based Requirement | IT Security02 |
| A.5.20 | Privileged utilities | Yes | Best Practice | IT Security02 |
| A.5.21 | Dev/Test/Prod separation | Yes | Organizational Requirement | IT Security09 |
| A.5.22 | Third-party access | Yes | Regulatory Requirement | IT Security11 |
| A.5.23 | Monitoring activities | Yes | Best Practice | IT Security07 |
| A.5.24 | Event reporting | Yes | Organizational Requirement | IT Security16 |
| A.5.25 | Incident response | Yes | Regulatory Requirement | IT Security16 |
| A.5.26 | Incident communication | Yes | Regulatory Requirement | IT Security16 |
| A.5.27 | Learning from incidents | Yes | Best Practice | IT Security16 |
| A.5.28 | Logging | Yes | Best Practice | IT Security07 |
| A.5.29 | Corrective actions | Yes | Regulatory Requirement | continual-improvement.md, registers/corrective-action-log.md |
| A.5.30 | Business continuity | Yes | Regulatory Requirement | IT Security17, registers/bcdr-test-log.md |
| A.5.31 | ICT readiness | Yes | Organizational Requirement | IT Security17, registers/bcdr-test-log.md |
| A.5.32 | Legal, statutory, contractual obligations | Yes | Regulatory Requirement | IT Security18, registers/legal-regulatory-register.md |
| A.5.33 | Privacy protection | Yes | Regulatory Requirement | IT Security05, Vendor Mgmt |
| A.5.34 | Compliance obligations | Yes | Regulatory Requirement | IT Security18, registers/legal-regulatory-register.md |
| A.5.35 | Independent review/audits | Yes | Regulatory Requirement | audit-policy.md |
| A.5.36 | Documented information | Yes | Best Practice | document-control.md |
| A.5.37 | Security awareness | Yes | Organizational Requirement | registers/training-register.md |

---

# A.6 — People Controls

| Control | Description | Applicable? | Justification | Reference |
|--------|-------------|-------------|---------------|-----------|
| A.6.1 | Background checks | Yes | Regulatory Requirement | HR Policy |
| A.6.2 | Employment terms | Yes | Organizational Requirement | HR Policy |
| A.6.3 | Security responsibilities | Yes | Best Practice | IT Security01 |
| A.6.4 | Security awareness | Yes | Regulatory Requirement | HR Training |
| A.6.5 | Disciplinary process | Yes | Organizational Requirement | HR Policy |
| A.6.6 | Responsibilities after termination | Yes | Organizational Requirement | Offboarding SOP |
| A.6.7 | Confidentiality agreements | Yes | Regulatory Requirement | Employment Agreements |

---

# A.7 — Physical Controls

| Control | Description | Applicable? | Justification | Reference |
|--------|-------------|-------------|---------------|-----------|
| A.7.1 | Physical security perimeter | Yes* | Risk-Based Requirement | IT Security12 |
| A.7.2 | Physical entry controls | Yes* | Regulatory Requirement | IT Security12 |
| A.7.3 | Securing offices/remote workspace | Yes | Organizational Requirement | IT Security12 |
| A.7.4 | Protecting assets | Yes | Risk-Based Requirement | IT Security12 |
| A.7.5 | Equipment maintenance | Yes | Organizational Requirement | IT Security12 |
| A.7.6 | Asset removal | Yes | Organizational Requirement | IT Security12 |
| A.7.7 | Secure disposal | Yes | Regulatory Requirement | IT Security12 |
| A.7.8 | Unattended equipment | Yes | Risk-Based Requirement | IT Security12 |
| A.7.9 | Clear desk/screen | Yes | Best Practice | IT Security12 |

(*Inherited AWS Data Center controls noted in policy*)

---

# A.8 — Technological Controls

| Control | Description | Applicable? | Justification | Reference |
|--------|-------------|-------------|---------------|-----------|
| A.8.1 | Operational procedures | Yes | Organizational Requirement | IT Security13 |
| A.8.2 | Change management | Yes | Regulatory Requirement | IT Security09 |
| A.8.3 | Capacity management | Yes | Organizational Requirement | IT Security13 |
| A.8.4 | Separation of environments | Yes | Best Practice | IT Security09 |
| A.8.5 | Capacity monitoring | Yes | Best Practice | IT Security13 |
| A.8.6 | Availability | Yes | Regulatory Requirement | IT Security17 |
| A.8.7 | Malware protection | Yes | Risk-Based Requirement | IT Security14 |
| A.8.8 | Vulnerability management | Yes | Regulatory Requirement | IT Security08 |
| A.8.9 | Configuration management | Yes | Best Practice | IT Security06 |
| A.8.10 | Configuration monitoring | Yes | Best Practice | IT Security06 |
| A.8.11 | Data masking | Yes | Organizational Requirement | IT Security09 |
| A.8.12 | Data retention | Yes | Regulatory Requirement | IT Security10 |
| A.8.13 | Backup | Yes | Regulatory Requirement | IT Security10 |
| A.8.14 | Backup testing | Yes | Best Practice | IT Security10 |
| A.8.15 | Logging | Yes | Regulatory Requirement | IT Security07 |
| A.8.16 | Monitoring | Yes | Best Practice | IT Security07 |
| A.8.17 | Log protection | Yes | Best Practice | IT Security07 |
| A.8.18 | Clock synchronization | Yes | Best Practice | IT Security07 |
| A.8.19 | Logging anomalies | Yes | Best Practice | IT Security07 |
| A.8.20 | Network security | Yes | Best Practice | IT Security04 |
| A.8.21 | Network controls | Yes | Risk-Based Requirement | IT Security04 |
| A.8.22 | Network segmentation | Yes | Best Practice | IT Security04 |
| A.8.23 | Cloud/SaaS monitoring | Yes | Best Practice | IT Security15 |
| A.8.24 | Cryptography | Yes | Regulatory Requirement | IT Security03 |
| A.8.25 | Key management | Yes | Best Practice | IT Security03 |
| A.8.26 | Key protection | Yes | Best Practice | IT Security03 |
| A.8.27 | Certificate management | Yes | Best Practice | IT Security03 |
| A.8.28 | Secure development | Yes | Best Practice | IT Security09 |
| A.8.29 | Code review + SDLC controls | Yes | Organizational Requirement | IT Security09 |

---

# Excluded Controls

| Control | Reason |
|--------|--------|
| A.7.10 (if applicable to large physical offices) | CompanyX is fully remote; no leased physical corporate office requiring physical perimeter controls |

---

# Approval
Approved by: CISO / CTO  
Date: YYYY-MM-DD
