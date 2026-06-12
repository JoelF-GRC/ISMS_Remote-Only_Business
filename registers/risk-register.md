# CompanyX Risk Register
ISO/IEC 27001:2022 Annex A Mapped Risk Register  
Last Updated: 2026-06-12  
Next Review Due: 2027-06-12

## Methodology
- Likelihood (L): Low / Medium / High  
- Impact (I): Low / Medium / High  
- Inherent Risk = L × I  
- Residual Risk = Post-treatment evaluation  
- Mapping: Each risk mapped to relevant Annex A controls

---

## Risk Register Table

| ID    | Asset             | Threat                  | Vulnerability                        | Inherent Risk | Controls Applied (Annex A)        | Residual Risk | Owner        | Treatment                | Status    | Date Identified | Last Reviewed |
| ----- | ----------------- | ----------------------- | ------------------------------------ | ------------- | --------------------------------- | ------------- | ------------ | ------------------------ | --------- | ---------------- | -------------- |
| R-001 | IAM (Entra)       | Account compromise      | Weak credentials, phishing           | High          | A.5.15–A.5.18, A.8.2, A.8.3, A.8.5 | Medium        | Security     | MFA, CA Policies         | Mitigated | 2025-06-12 | 2026-06-12 |
| R-002 | AWS Workloads     | Misconfiguration        | Overly permissive IAM or SGs         | High          | A.8.9, A.8.20–A.8.22               | Medium        | Cloud        | IaC + Config alerts      | Mitigated | 2025-06-12 | 2026-06-12 |
| R-003 | Endpoints         | Malware/Ransomware      | Unpatched OS, user download          | High          | A.8.1, A.8.7, A.8.9, A.8.16        | Medium        | Security Ops | EDR, Patch SLAs          | Mitigated | 2025-06-12 | 2026-06-12 |
| R-004 | S3 Buckets        | Public access exposure  | Misconfigured ACLs                   | High          | A.8.3, A.8.9, A.8.12              | Low           | Cloud        | Block-public-access; IAM | Mitigated | 2025-06-12 | 2026-06-12 |
| R-005 | Production Data   | Data breach             | Lack of encryption or access control | High          | A.8.3, A.8.24, A.5.34             | Low           | Engineering  | Encryption, RBAC         | Mitigated | 2025-06-12 | 2026-06-12 |
| R-006 | CI/CD             | Supply chain compromise | Vulnerable dependencies              | Medium        | A.5.21, A.8.25, A.8.28            | Low           | DevOps       | SCA, pinned deps         | Mitigated | 2025-06-12 | 2026-06-12 |
| R-007 | Vendors           | Third-party breach      | Weak vendor security                 | High          | A.5.19, A.5.20, A.5.22            | Medium        | GRC          | VRM reviews              | Mitigated | 2025-06-12 | 2026-06-12 |
| R-008 | Workforce         | Insider threat          | Privileged misuse                    | Medium        | A.5.3, A.8.2, A.8.18              | Medium        | Security     | PIM, logging             | Accepted  | 2025-06-12 | 2026-06-12 |
| R-009 | BCDR              | Cloud outage            | Multi-AZ misconfiguration            | High          | A.5.29, A.5.30, A.8.14            | Medium        | Infra        | Multi-AZ, backups        | Mitigated | 2025-06-12 | 2026-06-12 |
| R-010 | Logs              | SIEM visibility gaps    | Logging disabled or misrouted        | Medium        | A.8.15, A.8.16                    | Low           | SecOps       | Central logging          | Mitigated | 2025-06-12 | 2026-06-12 |
| R-011 | API               | API exploit             | Broken auth/validation               | High          | A.8.5, A.8.26, A.8.28             | Medium        | Engineering  | API Gateway + WAF        | Mitigated | 2025-06-12 | 2026-06-12 |
| R-012 | Remote Access     | Credential theft        | Remote-first risks                   | High          | A.6.7, A.8.2, A.8.5               | Medium        | IAM          | MFA, CA, VPN rules       | Mitigated | 2025-06-12 | 2026-06-12 |
| R-013 | Data Retention    | Excess retention        | Improper deletion                    | Medium        | A.8.10, A.5.33                    | Medium        | GRC          | Retention policy         | Accepted  | 2025-06-12 | 2026-06-12 |
| R-014 | Incident Response | Detection failure       | Missing alerts                       | Medium        | A.5.24, A.5.25, A.8.16            | Medium        | SecOps       | SIEM rules, testing      | Mitigated | 2025-06-12 | 2026-06-12 |
| R-015 | Physical Security | Lost laptop             | Remote work risk                     | Medium        | A.6.7, A.7.9, A.8.1               | Low           | Security     | MDM, disk encryption     | Mitigated | 2025-06-12 | 2026-06-12 |
| R-016 | AWS Region | Climate-related outage | Severe weather causing regional failure | High | A.5.29, A.5.30, A.8.14 | Medium | Infra/Sec | Multi-region planning | Mitigated | 2025-11-03 | 2026-06-12 |
| R-017 | Workforce Availability | Natural disaster | Remote staff affected by wildfire, flood, hurricane | Medium | A.5.29, A.5.30 | Medium | HR/Sec | Distributed workforce, redundancy | Accepted | 2025-11-03 | 2026-06-12 |
| R-018 | Vendor Hosting | Climate infrastructure risk | Supplier data center impacted by environmental conditions | High | A.5.22, A.5.30 | Medium | GRC | Review supplier BC/DR | Mitigated | 2025-11-03 | 2026-06-12 |
| R-019 | Connectivity | ISP instability | Extreme weather affecting last-mile connectivity | Medium | A.5.30, A.6.7 | Medium | IT | Secondary hotspots/ISPs | Mitigated | 2025-11-03 | 2026-06-12 |

---

