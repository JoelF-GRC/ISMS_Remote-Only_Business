# IT Security11 – Supplier & Vendor Management Policy
(Annex A: A.5.19, A.5.20, A.5.21, A.5.22, A.8.30)

## Overview
CompanyX ensures that third-party suppliers, vendors, hosting providers, and service partners operate in a secure manner consistent with CompanyX’s information security and compliance requirements. This policy governs the onboarding, assessment, monitoring, and termination of supplier relationships.

## Policy

### 1. Supplier Classification  
(Annex A: A.5.19)
- Suppliers must be classified based on risk:
  - **Low Risk**: No access to data or systems.
  - **Medium Risk**: Access to internal systems or non-sensitive data.
  - **High Risk**: Access to production systems or Confidential/Highly Confidential data.
- High-risk vendors require formal security review and contract terms.

### 2. Security Due Diligence  
- Prior to onboarding, High and Medium risk suppliers must undergo:
  - Security questionnaire review
  - SOC 2, ISO 27001, or equivalent reports
  - Penetration test or vulnerability scan evidence (if applicable)
  - Assessment of data protection measures
- Evaluate whether critical suppliers maintain climate-resilient operations (e.g., multi-region redundancy, environmental risk planning).
- Identified risks must be documented in the Supplier Risk Register.
- **AI Tool Vendors**: The onboarding and approval of AI tools and AI-enabled services is governed by IT Security22 (AI Acceptable Use & Governance Policy). AI tool vendor assessments must additionally include review of data training practices, model data retention policies, and sub-processor disclosure.

### 3. Contractual Requirements
- Contracts with suppliers must include:
  - Confidentiality and data protection clauses
  - Breach notification requirements
  - Right to audit (or equivalent assurances)
  - Requirements for MFA, encryption, and secure access
  - Data retention and destruction terms

### 4. Ongoing Monitoring  
- High-risk suppliers must be reviewed at least annually.
- Medium-risk suppliers must be reviewed at least every two years.
- Vendor performance and security posture must be reassessed based on:
  - Updated SOC 2/ISO reports
  - Changes in service scope
  - Incident history
  - Vulnerability exposure notifications
### 5. Access Control for Vendors  
(Annex A: A.5.22)
- Vendor access must:
  - Use CompanyX-managed identities where possible
  - Be time-bound and role-based
  - Be monitored for unusual activity
- Privileged vendor access must require MFA and approval.

### 6. Offboarding of Vendors  
- Upon termination, vendors must:
  - Return or securely destroy CompanyX data
  - Revoke any access credentials within 24 hours
- Offboarding must be coordinated through Security and Procurement.

## Policy Conflicts
If conflict arises between this policy and supplier requirements, CompanyX security requirements take precedence unless formally accepted via risk governance.

## Enforcement
Noncompliance may result in termination of supplier relationships or internal disciplinary action.

## Ownership
Security Department (Vendor Risk Management)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-----------|--------------|-------------|
| 1.0 | Security Department | 2025-04-01 | Initial creation | CISO / CTO |
