# IT Security22 – AI Acceptable Use & Governance Policy
(Annex A: A.5.10, A.5.19, A.5.34, A.8.25)

## Overview
Artificial Intelligence (AI) tools, including generative AI models, AI-assisted coding tools, AI-powered SaaS features, and automated decision-support systems, introduce unique risks related to data confidentiality, intellectual property, accuracy, and regulatory compliance. This policy establishes CompanyX's requirements for the acceptable use of AI tools, the approval process for adopting new AI tools, and the governance obligations applicable to all AI-assisted work.

The approval process for AI tools is integrated with the vendor management process defined in IT Security11 (Supplier & Vendor Management Policy). Data classification rules that govern what may be entered into AI tools are defined in IT Security05 (Asset Management & Information Classification Policy). Privacy obligations for AI use involving personal data are defined in IT Security21 (Data Protection & Privacy Policy).

> **Relationship to the AI Management System**: CompanyX operates a dedicated AI Management System (AIMS), aligned to ISO/IEC 42001 (AI Management Systems), the NIST AI Risk Management Framework (AI RMF), and the EU AI Act, documented in the companion `AI-Management_SaaS_Business` repository. This policy remains the ISO 27001-level baseline for AI acceptable use and continues to apply in full. The AIMS provides deeper, AI-specific governance layered on top of this policy — including the authoritative Approved AI Tool List, the AI system inventory, and the AI-specific risk register — and is the authoritative source where both frameworks address the same AI matter.

## Policy

### 1. Approved AI Tools  
(Annex A: A.5.10, A.8.19)
- Employees may only use AI tools that appear on the CompanyX **Approved AI Tool List**, owned by the AI Management Committee under the companion AI Management System (see `AI-Management_SaaS_Business/registers/approved-ai-tool-list.md`), with day-to-day administration delegated by AI-use context per that framework's roles-responsibilities.md.
- The Approved AI Tool List specifies:
  - Tool name and vendor
  - Approved use cases
  - Maximum data classification permitted as input
  - Applicable access controls or configuration requirements
- Using AI tools not on the Approved List is prohibited without prior written approval from the Security Department.

**Default approved tool categories at time of policy creation (examples):**

| Tool | Category | Max Data Classification | Notes |
|------|----------|------------------------|-------|
| GitHub Copilot (Business/Enterprise) | AI coding assistant | Internal | Enterprise tier with org-level data exclusion required |
| Microsoft 365 Copilot | Productivity AI | Confidential | Requires M365 E3/E5 tenant with no training opt-in |
| ChatGPT Enterprise | Generative AI | Confidential | Enterprise/business tier with training opt-out contractually confirmed; zero data retention policy required |

*The Approved AI Tool List is maintained as a living document separate from this policy, in the companion AI Management System repository (`AI-Management_SaaS_Business/registers/approved-ai-tool-list.md`). The table above is illustrative; refer to that list for authoritative approved tools and current data classification limits.*

### 2. Request and Approval Process for New AI Tools  
(Annex A: A.5.19, A.5.20)
- Any employee who wishes to use a new AI tool or AI-enabled feature must submit an **AI Tool Approval Request** to the Security Department before use.
- The approval process follows the vendor onboarding steps in IT Security11 and additionally requires:

  **Step 1 – Request Submission**  
  - Submit tool name, vendor, intended use case, and proposed data inputs to the Security Department via the IT ticketing system.

  **Step 2 – Vendor Security Assessment**  
  - Security conducts a risk-tiered assessment including:
    - Review of vendor's data processing and AI training practices
    - Review of SOC 2, ISO 27001, or equivalent certifications
    - Assessment of data retention, model training opt-out options, and subprocessor disclosure
    - DPIA if personal data will be processed (see IT Security21)

  **Step 3 – Classification and Risk Decision**  
  - Tool is classified as Low, Medium, or High risk per IT Security11 criteria.
  - High-risk AI tools (e.g., those that process Confidential or Highly Confidential data, or that make automated decisions affecting individuals) require CISO approval.

  **Step 4 – Approval and List Update**  
  - Approved tools are added to the Approved AI Tool List with defined scope and data classification limits.
  - Users are notified of approval and any usage conditions.

- Urgent or time-sensitive requests may follow the emergency change process in IT Security09 (Secure Development & Change Management Policy) with retrospective review.

### 3. Data Classification Restrictions for AI Inputs  
(Annex A: A.5.10, A.5.34, A.8.12)
- The data classification level that may be entered into an AI tool is determined by the tool's entry in the Approved AI Tool List.
- As a general default:

| Data Classification | AI Tool Input Permitted? |
|--------------------|-----------------------|
| Public | Yes — all approved tools |
| Internal | Yes — approved tools with data isolation confirmed |
| Confidential | Only tools explicitly approved for Confidential data |
| Highly Confidential | Prohibited unless CISO approves a specific use case |

- Customer personal data (PII) must not be entered into any AI tool unless the tool has a confirmed no-training policy, a DPA is in place per IT Security21, and the use has been reviewed for DPIA requirements.
- Production database exports, credentials, encryption keys, and security configurations must never be entered into AI tools regardless of approval status.

### 4. Prohibited Uses of AI Tools  
(Annex A: A.5.10)
The following uses are prohibited regardless of tool approval status:
- Entering credentials, API keys, passwords, or secrets into AI tools
- Uploading Highly Confidential data (financial records, M&A information, unreleased IP) to any AI tool
- Using AI tools to make unreviewed automated decisions that affect individuals (hiring, performance, access rights)
- Using AI tools to generate or distribute content designed to deceive, manipulate, or mislead (deepfakes, disinformation)
- Using AI to attempt to reverse-engineer CompanyX or competitor systems, circumvent security controls, or generate malicious code
- Using unapproved AI tools under the assumption they will be retroactively approved

### 5. AI-Generated Content Review  
(Annex A: A.5.10, A.8.28)
- AI-generated code, documents, legal text, security configurations, and customer communications must be reviewed by a qualified human before use in production or external distribution.
- Developers using AI coding assistants must verify AI-generated code for:
  - Security vulnerabilities (OWASP Top 10, injection, insecure defaults)
  - License compatibility
  - Correctness and alignment with CompanyX architecture
- AI-generated content must not be represented as human-authored in contexts where that distinction is material.

### 6. Intellectual Property and Copyright  
(Annex A: A.5.10)
- Employees must not enter CompanyX proprietary code, trade secrets, or unreleased product information into AI tools whose training terms could expose that content.
- AI-generated output may incorporate training data from third parties. Legal must be consulted where AI-generated content is intended for commercial use or external publication.
- CompanyX's ownership of AI-assisted work products follows standard employment agreements.

### 7. Monitoring and Audit  
(Annex A: A.5.10, A.8.15)
- Security may audit the use of AI tools, including reviewing access logs, DLP alerts, and vendor usage reports.
- Use of unapproved AI tools that results in exposure of Confidential data will be treated as a security incident per IT Security16 (Incident Response Policy).
- The Approved AI Tool List is reviewed at least annually and when significant changes occur in a tool's data handling practices.

### 8. Training and Awareness  
(Annex A: A.6.3)
- All employees using approved AI tools must complete AI security awareness training that covers:
  - Data classification restrictions
  - Prohibited inputs
  - Reviewing AI-generated output
  - How to request approval for new AI tools
- Training must be completed before first use of an approved AI tool and refreshed annually.

## Policy Conflicts
Where an approved AI tool's vendor changes its data handling or training practices, the tool must be reassessed before continued use of Confidential data inputs.

## Enforcement
Use of unapproved AI tools or violation of data classification restrictions may result in disciplinary action. Exposure of Confidential or Highly Confidential data through AI tools will be treated as a data breach and investigated under IT Security16.

## Ownership
Security Department (AI Governance & Risk)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-----------|--------------|-------------|
| 1.0 | Security Department | 2026-06-12 | Initial creation | CISO / CTO |
| 1.1 | Security Department | 2026-07-02 | Replaced Future Alignment Note with Relationship to the AI Management System now that the companion AIMS repo exists; corrected Approved AI Tool List ownership to the AI Management Committee; corrected ChatGPT Enterprise illustrative classification to Confidential to match the authoritative Approved AI Tool List | CISO / CTO |
