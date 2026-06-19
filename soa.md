# Statement of Applicability (SoA)
CompanyX ISO/IEC 27001:2022  
Last Updated: 2026-06-19

## Purpose
This Statement of Applicability (SoA) lists all 93 Annex A controls from ISO/IEC 27001:2022 (A.5: 37 controls, A.6: 8 controls, A.7: 14 controls, A.8: 34 controls), declares whether each control is applicable to CompanyX, and identifies the justification and implementation reference.

This version uses the four ISO audit–preferred justification categories:

### Justification Categories
- **Regulatory Requirement** – Mandated by law, regulation, or contract.
- **Organizational Requirement** – Needed to meet business, customer, or operational needs.
- **Best Practice** – Based on industry standards, ISO/NIST/SOC 2 expectations, or secure-by-design principles.
- **Risk-Based Requirement** – Necessary to treat identified risks.

### Note on HR References
References to "HR Policy," "HR Training," "Offboarding SOP," and "Employment Agreements" (A.6.1, A.6.2, A.6.4, A.6.5, A.6.6) point to CompanyX's HR documentation, which is maintained outside this repository (see README — out-of-scope items). They are listed here for SoA completeness.

### Note on A.7 Physical Controls and AWS Inheritance
CompanyX is a fully remote organization with no company-operated offices, server rooms, or physical facilities (see ISMS-policies/scope.md). All information processing infrastructure runs on AWS. Under the AWS Shared Responsibility Model, AWS retains responsibility for the physical security of its data centers, including perimeter security, physical access controls, environmental protections, supporting utilities, and equipment siting. CompanyX inherits these controls through AWS's ISO 27001 and SOC 2 certifications, and documents its reliance on AWS physical assurances in IT Security12 (Physical & Data Center Security Policy). Controls covering exclusively company-operated facilities — specifically A.7.3 (offices and rooms), A.7.6 (secure areas), and A.7.12 (cabling) — are excluded, as CompanyX has no such facilities. CompanyX-owned physical security obligations, which primarily govern employee endpoints, home offices, and remote work environments, are addressed in IT Security12 and IT Security20 (Remote Working Policy).

---

# ANNEX A CONTROLS

---

# A.5 — Organizational Controls (37 controls)

| Control | Description | Applicable? | Justification | Reference |
|--------|-------------|-------------|---------------|-----------|
| A.5.1 | Policies for information security | Yes | Best Practice | IT Security01 |
| A.5.2 | Information security roles and responsibilities | Yes | Organizational Requirement | roles-responsibilities.md |
| A.5.3 | Segregation of duties | Yes | Risk-Based Requirement | IT Security02 |
| A.5.4 | Management responsibilities | Yes | Organizational Requirement | management-overview.md |
| A.5.5 | Contact with authorities | Yes | Regulatory Requirement | IT Security16 |
| A.5.6 | Contact with special interest groups | Yes | Best Practice | IT Security07 |
| A.5.7 | Threat intelligence | Yes | Best Practice | IT Security07 |
| A.5.8 | Information security in project management | Yes | Organizational Requirement | IT Security09 |
| A.5.9 | Inventory of information and other associated assets | Yes | Best Practice | IT Security05, asset-register.md |
| A.5.10 | Acceptable use of information and other associated assets | Yes | Organizational Requirement | IT Security19, IT Security22 |
| A.5.11 | Return of assets | Yes | Organizational Requirement | IT Security19, HR Offboarding Procedures |
| A.5.12 | Classification of information | Yes | Risk-Based Requirement | IT Security05 |
| A.5.13 | Labelling of information | Yes | Best Practice | IT Security05 |
| A.5.14 | Information transfer | Yes | Best Practice | IT Security05, IT Security04 |
| A.5.15 | Access control | Yes | Regulatory Requirement | IT Security02 |
| A.5.16 | Identity management | Yes | Best Practice | IT Security02 |
| A.5.17 | Authentication information | Yes | Best Practice | IT Security02 |
| A.5.18 | Access rights | Yes | Risk-Based Requirement | IT Security02 |
| A.5.19 | Information security in supplier relationships | Yes | Regulatory Requirement | IT Security11, IT Security22 |
| A.5.20 | Addressing information security within supplier agreements | Yes | Regulatory Requirement | IT Security11 |
| A.5.21 | Managing information security in the ICT supply chain | Yes | Risk-Based Requirement | IT Security11, IT Security09 |
| A.5.22 | Monitoring, review and change management of supplier services | Yes | Best Practice | IT Security11, vendor-register.md |
| A.5.23 | Information security for use of cloud services | Yes | Best Practice | IT Security15 |
| A.5.24 | Information security incident management planning and preparation | Yes | Organizational Requirement | IT Security16 |
| A.5.25 | Assessment and decision on information security events | Yes | Regulatory Requirement | IT Security16 |
| A.5.26 | Response to information security incidents | Yes | Regulatory Requirement | IT Security16 |
| A.5.27 | Learning from information security incidents | Yes | Best Practice | IT Security16, corrective-action-log.md |
| A.5.28 | Collection of evidence | Yes | Best Practice | IT Security16, IT Security07 |
| A.5.29 | Information security during disruption | Yes | Regulatory Requirement | IT Security17 |
| A.5.30 | ICT readiness for business continuity | Yes | Organizational Requirement | IT Security17, bcdr-test-log.md |
| A.5.31 | Legal, statutory, regulatory and contractual requirements | Yes | Regulatory Requirement | IT Security18, legal-regulatory-register.md |
| A.5.32 | Intellectual property rights | Yes | Regulatory Requirement | IT Security18, legal-regulatory-register.md |
| A.5.33 | Protection of records | Yes | Regulatory Requirement | IT Security05, document-control.md |
| A.5.34 | Privacy and protection of PII | Yes | Regulatory Requirement | IT Security21 (primary), IT Security05, legal-regulatory-register.md |
| A.5.35 | Independent review of information security | Yes | Regulatory Requirement | audit-policy.md |
| A.5.36 | Compliance with policies, rules and standards for information security | Yes | Best Practice | IT Security18, document-control.md |
| A.5.37 | Documented operating procedures | Yes | Best Practice | IT Security13, document-control.md |

---

# A.6 — People Controls (8 controls)

| Control | Description | Applicable? | Justification | Reference |
|--------|-------------|-------------|---------------|-----------|
| A.6.1 | Screening | Yes | Regulatory Requirement | HR Policy |
| A.6.2 | Terms and conditions of employment | Yes | Organizational Requirement | HR Policy |
| A.6.3 | Information security awareness, education and training | Yes | Best Practice | training-register.md |
| A.6.4 | Disciplinary process | Yes | Organizational Requirement | HR Policy |
| A.6.5 | Responsibilities after termination or change of employment | Yes | Organizational Requirement | IT Security19, Offboarding SOP |
| A.6.6 | Confidentiality or non-disclosure agreements | Yes | Regulatory Requirement | Employment Agreements |
| A.6.7 | Remote working | Yes | Organizational Requirement | IT Security20 (primary), IT Security12, IT Security19 |
| A.6.8 | Information security event reporting | Yes | Organizational Requirement | IT Security16 |

---

# A.7 — Physical Controls (14 controls)

| Control | Description | Applicable? | Justification | Reference |
|--------|-------------|-------------|---------------|-----------|
| A.7.1 | Physical security perimeters | Yes | Risk-Based Requirement | AWS Shared Responsibility Model (inherited), IT Security12 |
| A.7.2 | Physical entry | Yes | Regulatory Requirement | AWS Shared Responsibility Model (inherited), IT Security12 |
| A.7.3 | Securing offices, rooms and facilities | No | N/A | See Excluded Controls |
| A.7.4 | Physical security monitoring | Yes | Risk-Based Requirement | AWS Shared Responsibility Model (inherited), IT Security12 |
| A.7.5 | Protecting against physical and environmental threats | Yes | Risk-Based Requirement | AWS Shared Responsibility Model (inherited), IT Security12, climate-change-addendum.md |
| A.7.6 | Working in secure areas | No | N/A | See Excluded Controls |
| A.7.7 | Clear desk and clear screen | Yes | Best Practice | IT Security12, IT Security20 |
| A.7.8 | Equipment siting and protection | Yes | Risk-Based Requirement | AWS Shared Responsibility Model (inherited), IT Security12, IT Security20 |
| A.7.9 | Security of assets off-premises | Yes | Risk-Based Requirement | IT Security12, IT Security20, IT Security19 |
| A.7.10 | Storage media | Yes | Best Practice | IT Security05, IT Security03, IT Security12 |
| A.7.11 | Supporting utilities | Yes | Risk-Based Requirement | AWS Shared Responsibility Model (inherited), IT Security12 |
| A.7.12 | Cabling security | No | N/A | See Excluded Controls |
| A.7.13 | Equipment maintenance | Yes | Organizational Requirement | AWS Shared Responsibility Model (inherited), IT Security12 |
| A.7.14 | Secure disposal or re-use of equipment | Yes | Regulatory Requirement | IT Security12 (employee devices), AWS Shared Responsibility Model (infrastructure media) |

---

# A.8 — Technological Controls (34 controls)

| Control | Description | Applicable? | Justification | Reference |
|--------|-------------|-------------|---------------|-----------|
| A.8.1 | User endpoint devices | Yes | Best Practice | IT Security14 |
| A.8.2 | Privileged access rights | Yes | Risk-Based Requirement | IT Security02 |
| A.8.3 | Information access restriction | Yes | Regulatory Requirement | IT Security02 |
| A.8.4 | Access to source code | Yes | Risk-Based Requirement | IT Security02, IT Security09 |
| A.8.5 | Secure authentication | Yes | Best Practice | IT Security02 |
| A.8.6 | Capacity management | Yes | Organizational Requirement | IT Security13 |
| A.8.7 | Protection against malware | Yes | Risk-Based Requirement | IT Security14 |
| A.8.8 | Management of technical vulnerabilities | Yes | Regulatory Requirement | IT Security08 |
| A.8.9 | Configuration management | Yes | Best Practice | IT Security06 |
| A.8.10 | Information deletion | Yes | Regulatory Requirement | IT Security05, IT Security10 |
| A.8.11 | Data masking | Yes | Organizational Requirement | IT Security09 |
| A.8.12 | Data leakage prevention | Yes | Risk-Based Requirement | IT Security05, IT Security07 |
| A.8.13 | Information backup | Yes | Regulatory Requirement | IT Security10 |
| A.8.14 | Redundancy of information processing facilities | Yes | Best Practice | IT Security17 |
| A.8.15 | Logging | Yes | Regulatory Requirement | IT Security07 |
| A.8.16 | Monitoring activities | Yes | Best Practice | IT Security07 |
| A.8.17 | Clock synchronization | Yes | Best Practice | IT Security07 |
| A.8.18 | Use of privileged utility programs | Yes | Best Practice | IT Security02 |
| A.8.19 | Installation of software on operational systems | Yes | Best Practice | IT Security06, IT Security19 |
| A.8.20 | Networks security | Yes | Best Practice | IT Security04 |
| A.8.21 | Security of network services | Yes | Risk-Based Requirement | IT Security04 |
| A.8.22 | Segregation of networks | Yes | Best Practice | IT Security04 |
| A.8.23 | Web filtering | Yes | Best Practice | IT Security14, IT Security04 |
| A.8.24 | Use of cryptography | Yes | Regulatory Requirement | IT Security03 |
| A.8.25 | Secure development life cycle | Yes | Best Practice | IT Security09 |
| A.8.26 | Application security requirements | Yes | Organizational Requirement | IT Security09 |
| A.8.27 | Secure system architecture and engineering principles | Yes | Best Practice | IT Security09, IT Security04 |
| A.8.28 | Secure coding | Yes | Best Practice | IT Security09 |
| A.8.29 | Security testing in development and acceptance | Yes | Organizational Requirement | IT Security09, IT Security08 |
| A.8.30 | Outsourced development | Yes | Risk-Based Requirement | IT Security09, IT Security11 |
| A.8.31 | Separation of development, test and production environments | Yes | Organizational Requirement | IT Security09 |
| A.8.32 | Change management | Yes | Regulatory Requirement | IT Security09 |
| A.8.33 | Test information | Yes | Best Practice | IT Security09, IT Security05 |
| A.8.34 | Protection of information systems during audit testing | Yes | Best Practice | audit-policy.md, IT Security09 |

---

# Excluded Controls

| Control | Reason |
|--------|--------|
| A.7.3 | Securing offices, rooms and facilities — CompanyX has no company-operated offices, rooms, or physical facilities (corporate office locations are explicitly out of scope; see ISMS-policies/scope.md). Physical security of information processing infrastructure is inherited from AWS. Home office and remote work environment requirements are addressed under A.6.7 in IT Security20. |
| A.7.6 | Working in secure areas — CompanyX has no company-operated secure areas, server rooms, or controlled access zones. Physical security of AWS data center secure areas is inherited under the AWS Shared Responsibility Model. Home office workspace security is addressed under A.6.7 in IT Security20. |
| A.7.12 | Cabling security — CompanyX is fully remote with no company-operated offices or data centers. Network cabling for AWS data centers is covered under AWS's shared-responsibility/ISO 27001 certification, and employee home/ISP cabling is outside CompanyX's control boundary. |

---

# Approval
Approved by: CISO / CTO  
Date: 2025-04-01
