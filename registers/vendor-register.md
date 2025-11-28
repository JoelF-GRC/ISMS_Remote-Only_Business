# CompanyX Vendor Register
Last Updated: YYYY-MM-DD

## Risk Tiers
- **High Risk:** Access to production data/systems  
- **Medium Risk:** Access to internal systems  
- **Low Risk:** No system/data access

---

## Vendor Inventory

| Vendor              | Service            | Risk Tier | Security Evidence | Renewal Date | Owner       | Notes                        |
| ------------------- | ------------------ | --------- | ----------------- | ------------ | ----------- | ---------------------------- |
| AWS                 | Cloud hosting      | High      | SOC 2, ISO 27001  | Annual       | Cloud       | Primary infrastructure       |
| Microsoft Entra ID  | Identity provider  | High      | SOC 2, ISO 27001  | Annual       | IAM         | SSO + Conditional Access     |
| Atlassian Jira      | Ticketing          | Medium    | SOC 2             | Annual       | Product Ops | SSO-enabled                  |
| GitHub              | Code repo          | High      | SOC 2             | Annual       | Engineering | SSO, branch protections      |
| CrowdStrike         | EDR/XDR            | High      | SOC 2             | Annual       | SecOps      | Identity protection included |
| Rapid7              | SIEM               | High      | SOC 2             | Annual       | SecOps      | Central logging              |
| Slack               | Communications     | Medium    | SOC 2             | Annual       | IT          | SSO required                 |
| Zoom                | Video conferencing | Medium    | SOC 2             | Annual       | IT          | Waiting room, host controls  |
| Payroll/HRIS Vendor | HR Data            | High      | SOC 2             | Annual       | HR          | Handles PII                  |

---

## Review Schedule
High-risk vendors reviewed annually, medium risk every two years.

## Offboarding Requirements
- Data destruction confirmation  
- Credential revocation  
- Termination of integrations  

