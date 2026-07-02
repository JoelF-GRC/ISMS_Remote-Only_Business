# CompanyX Vendor Register
Last Updated: 2026-07-02

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
| Foundation Model API Provider (illustrative: "a frontier LLM API provider") | Embedded product AI backend | High | SOC 2, DPA, training opt-out confirmed | Annual, or on model/provider change | Product/Engineering | Base vendor review under this register; AI-specific due diligence delta tracked in `AI-Management_SaaS_Business/registers/ai-vendor-due-diligence-register.md` per AI-Gov04 |
| ChatGPT Enterprise | Generative AI, internal productivity | Medium | SOC 2, training opt-out confirmed | Annual | Security | See Approved AI Tool List (ATL-002) for data classification limits |
| Microsoft 365 Copilot | Generative AI, productivity suite add-on | Medium | SOC 2, covered under existing M365/Entra tenant agreement | Annual | IT | See Approved AI Tool List (ATL-001) for data classification limits |
| GitHub Copilot (Business/Enterprise) | AI coding assistant | Medium | SOC 2, org-level data exclusion required | Annual | Engineering | Add-on to existing GitHub relationship above; see Approved AI Tool List (ATL-003) |

---

## Review Schedule
High-risk vendors reviewed annually, medium risk every two years.

## Offboarding Requirements
- Data destruction confirmation  
- Credential revocation  
- Termination of integrations  

