# CompanyX Asset Register
Last Updated: YYYY-MM-DD

## Instructions
Each asset must include:
- Owner
- Classification (Public / Internal / Confidential / Highly Confidential)
- Location (AWS region, endpoint, SaaS)
- Protection Requirements
- Backup requirements (if applicable)

---

## Asset Inventory

### Cloud Infrastructure (AWS)

| Asset | Type | Owner | Classification | Location | Protection Requirements |
|-------|------|--------|----------------|-----------|---------------------------|
| AWS Account (Prod) | Cloud Account | Cloud Team | Highly Confidential | us-east-1 | MFA, SCPs, GuardDuty |
| VPC (Prod) | Network | Cloud Team | Internal | us-east-1 | SG/NACL restrictions |
| EC2 Instances | Compute | Engineering | Internal | Multi-AZ | CIS baseline, SSM |
| RDS (Prod) | Database | Engineering | Highly Confidential | Multi-AZ | Encryption, backups |
| S3 Buckets | Storage | Engineering | Confidential | Various | Encryption, block-public-access |

---

### SaaS & Identity

| Asset | Type | Owner | Classification | Location | Protection Requirements |
|-------|------|--------|----------------|-----------|---------------------------|
| Entra ID Tenant | Identity Provider | IAM Lead | Highly Confidential | Global | MFA, CA, PIM |
| Jira Cloud | Ticketing | Product Ops | Internal | Cloud | SSO + RBAC |
| GitHub | Code Repo | Engineering | Confidential | Cloud | SSO, branch protections |
| Rapid7 SIEM | Monitoring | SecOps | Confidential | Cloud | Logging integrity |

---

### Endpoints & Devices

| Asset | Type | Owner | Classification | Location | Protection Requirements |
|-------|------|--------|----------------|-----------|---------------------------|
| Company Laptop | Endpoint | IT | Internal | Remote | MDM, EDR, encryption |
| Mobile Devices | Endpoint | IT | Internal | Remote | MFA, MDM, lock screen |

---

### Data Assets

| Asset | Type | Owner | Classification | Location | Protection Requirements |
|-------|------|--------|----------------|-----------|---------------------------|
| Production Data | Structured Data | Engineering | Highly Confidential | AWS RDS | Encryption, IAM, backups |
| Application Logs | Logs | Engineering | Internal | S3 | Encryption, retention rules |

---

