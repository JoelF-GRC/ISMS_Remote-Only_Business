# CompanyX Risk Register
ISO/IEC 27001:2022 Annex A Mapped Risk Register  
Last Updated: YYYY-MM-DD

## Methodology
- Likelihood (L): Low / Medium / High  
- Impact (I): Low / Medium / High  
- Inherent Risk = L × I  
- Residual Risk = Post-treatment evaluation  
- Mapping: Each risk mapped to relevant Annex A controls

---

## Risk Register Table

| ID    | Asset             | Threat                  | Vulnerability                        | Inherent Risk | Controls Applied (Annex A)        | Residual Risk | Owner        | Treatment                | Status    |
| ----- | ----------------- | ----------------------- | ------------------------------------ | ------------- | --------------------------------- | ------------- | ------------ | ------------------------ | --------- |
| R-001 | IAM (Entra)       | Account compromise      | Weak credentials, phishing           | High          | A.5.15–A.5.23 (IAM), A.8.2, A.8.3 | Medium        | Security     | MFA, CA Policies         | Mitigated |
| R-002 | AWS Workloads     | Misconfiguration        | Overly permissive IAM or SGs         | High          | A.8.20–A.8.22                     | Medium        | Cloud        | IaC + Config alerts      | Mitigated |
| R-003 | Endpoints         | Malware/Ransomware      | Unpatched OS, user download          | High          | A.8.7, A.8.9, A.5.23              | Medium        | Security Ops | EDR, Patch SLAs          | Mitigated |
| R-004 | S3 Buckets        | Public access exposure  | Misconfigured ACLs                   | High          | A.8.20, A.8.21, A.8.26            | Low           | Cloud        | Block-public-access; IAM | Mitigated |
| R-005 | Production Data   | Data breach             | Lack of encryption or access control | High          | A.8.24–A.8.29                     | Low           | Engineering  | Encryption, RBAC         | Mitigated |
| R-006 | CI/CD             | Supply chain compromise | Vulnerable dependencies              | Medium        | A.8.28, A.8.25                    | Low           | DevOps       | SCA, pinned deps         | Mitigated |
| R-007 | Vendors           | Third-party breach      | Weak vendor security                 | High          | A.5.22, A.5.23                    | Medium        | GRC          | VRM reviews              | Mitigated |
| R-008 | Workforce         | Insider threat          | Privileged misuse                    | Medium        | A.5.19–A.5.21                     | Medium        | Security     | PIM, logging             | Accepted  |
| R-009 | BCDR              | Cloud outage            | Multi-AZ misconfiguration            | High          | A.5.30, A.8.13–A.8.14             | Medium        | Infra        | Multi-AZ, backups        | Mitigated |
| R-010 | Logs              | SIEM visibility gaps    | Logging disabled or misrouted        | Medium        | A.8.15–A.8.23                     | Low           | SecOps       | Central logging          | Mitigated |
| R-011 | API               | API exploit             | Broken auth/validation               | High          | A.8.28                            | Medium        | Engineering  | API Gateway + WAF        | Mitigated |
| R-012 | Remote Access     | Credential theft        | Remote-first risks                   | High          | A.8.2, A.5.23                     | Medium        | IAM          | MFA, CA, VPN rules       | Mitigated |
| R-013 | Data Retention    | Excess retention        | Improper deletion                    | Medium        | A.8.12–A.8.14                     | Medium        | GRC          | Retention policy         | Accepted  |
| R-014 | Incident Response | Detection failure       | Missing alerts                       | Medium        | A.5.24–A.5.27                     | Medium        | SecOps       | SIEM rules, testing      | Mitigated |
| R-015 | Physical Security | Lost laptop             | Remote work risk                     | Medium        | A.7.3–A.7.8                       | Low           | Security     | MDM, disk encryption     | Mitigated |
| R-016 | AWS Region | Climate-related outage | Severe weather causing regional failure | High | A.5.30, A.8.13–A.8.14 | Medium | Infra/Sec | Multi-region planning | Mitigated |
| R-017 | Workforce Availability | Natural disaster | Remote staff affected by wildfire, flood, hurricane | Medium | A.5.30 | Medium | HR/Sec | Distributed workforce, redundancy | Accepted |
| R-018 | Vendor Hosting | Climate infrastructure risk | Supplier data center impacted by environmental conditions | High | A.5.22, A.5.30 | Medium | GRC | Review supplier BC/DR | Mitigated |
| R-019 | Connectivity | ISP instability | Extreme weather affecting last-mile connectivity | Medium | A.5.30 | Medium | IT | Secondary hotspots/ISPs | Mitigated |

---

