# CompanyX ISO 27001:2022 Mini-ISMS (Public, Sanitized)

This repository contains a fully documented, public, sanitized ISO 27001:2022 Information Security Management System (ISMS) for CompanyX — a remote-first SaaS company operating on AWS with Entra ID, CrowdStrike, Rapid7, and Jira.

This repo is built for:
- Demonstrating ISO 27001 capabilities
- Sharing best-practice templates
- Providing reusable artifacts for GRC portfolios
- Documenting governance, risk, and compliance work

## 📁 Repository Contents

### ISMS Governance Policies (Clauses 4–10)
Located in `/ISMS-policies/`, these define the ISMS itself:
- Scope
- Context of Organization
- Objectives
- Risk Methodology
- Management Overview
- Management Review (record template + log)
- Audit Policy
- Continual Improvement

### IT Security Policies (Annex A Consolidated)
Located in `/IT-security-policies/`.

18 total consolidated policies aligned to ISO/IEC 27001:2022 Annex A controls:
- Access Control  
- Cryptography  
- Network & Infrastructure Security  
- Asset Management  
- Secure Configuration  
- Logging & Monitoring  
- Vulnerability & Patch  
- Secure Development  
- Backup & Recovery  
- Vendor Management  
- Physical Security  
- Malware Protection  
- Cloud Security  
- Incident Response  
- BCDR  
- Compliance & Audit  
…and more.

### Registers
Located in `/registers/`.
- **risk-register.md** — ISO-aligned risks, mapped to Annex A  
- **asset-register.md** — asset inventory template for cloud-native SaaS  
- **vendor-register.md** — vendor tracking + risk tiering
- **risk-treatment-plan.md** — action plan tracking treatment of each risk to residual acceptance

### Core ISO Documents
- **scope.md**  
- **context-of-organization.md**  
- **soa.md** (Statement of Applicability)  
- **internal-audit-checklist.md**

### Certification Readiness Toolkit
- **gap-analysis.md** — maturity-based gap assessment against ISO/IEC 27001:2022 Clauses 4–10 and Annex A policy areas, used to scope and prioritize an implementation project
- **iso27001-readiness-checklist.md** — tracks status of mandatory documents and operational records toward Stage 1/Stage 2 certification readiness

### Diagrams
Under `/diagrams/` including:
- **aws-multiregion-rescaled.drawio** and **diagram.drawio** (XML for Draw.io compatible diagrams)

## 🧩 How This Repo Works

This repo mimics the structure of a lightweight, audit-ready ISO 27001 ISMS.  
Documents are intentionally:
- High-clarity  
- Concise  
- Mapped to ISO 27001:2022  
- Generic/sanitized using “CompanyX”  
- Optimized for remote-first SaaS teams using AWS

### What This Repo *Does Not* Contain
- Confidential data  
- Proprietary architecture  
- Real customer information  
- Non-public internal processes  

### What This Repo *Does* Provide
- A complete example ISMS suitable for:
  - Interviews
  - Portfolio building
  - Demonstrating GRC and ISO 27001 capabilities
  - Teaching others how to structure an ISMS  
  - Seeding a real ISMS in a startup or scale-up

## 🛠 How to Use This Repo

1. Clone and adapt for your own organization.  
2. Replace “CompanyX” with your company name.  
3. Update the registers with actual data.  
4. Add evidence folders if using this for a real audit.  
5. Use `/IT-security-policies/` to guide technical controls.  
6. Use `/ISMS-policies/` for ISMS governance structure.  

## 📜 License
Open for public reuse. Attribution appreciated but not required.

