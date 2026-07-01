# CompanyX ISO 27001:2022 Mini-ISMS (Public, Sanitized)

This repository contains a fully documented, public, sanitized ISO 27001:2022 Information Security Management System (ISMS) for CompanyX — a remote-first SaaS company operating on AWS with Entra ID, CrowdStrike, Rapid7, and Jira.

This repo is built for:
- Demonstrating ISO 27001 capabilities
- Sharing best-practice templates
- Providing reusable artifacts for GRC portfolios
- Documenting governance, risk, and compliance work

## Repository Contents

### Mandatory Documented Information (ISO 27001:2022)

The table below maps every clause-mandated record to the file that satisfies it, giving a reviewer a single coverage view.

| Document | ISO 27001:2022 Clause | Location |
|----------|-----------------------|----------|
| ISMS scope | 4.3 | `ISMS-policies/scope.md` |
| Information security policy | 5.2 | `IT-security-policies/IT Security01 – Information Security Management Policy.md` |
| Risk assessment process | 6.1.2 | `ISMS-policies/risk-methodology.md` |
| Risk assessment results | 6.1.2 | `registers/risk-register.md` |
| Risk treatment plan | 6.1.3 | `registers/risk-treatment-plan.md` |
| Statement of Applicability | 6.1.3 d) | `soa.md` |
| Information security objectives | 6.2 | `ISMS-policies/objectives.md` |
| Evidence of competence and training | 7.2, 7.3 | `registers/training-register.md` |
| Monitoring and measurement results | 9.1 | `registers/metrics-register.md` |
| Internal audit programme | 9.2 | `ISMS-policies/audit-policy.md` |
| Internal audit results | 9.2 | `internal-audit-checklist.md` |
| Management review results | 9.3 | `ISMS-policies/management-review.md` |
| Nonconformity and corrective action records | 10.2 | `registers/corrective-action-log.md` |

---

### ISMS Governance Policies (Clauses 4–10)
Located in `/ISMS-policies/`, these define the ISMS itself:
- Scope
- Context of Organization
- Objectives
- Risk Methodology
- Management Overview
- Management Review (record template + log)
- Management Review Deck (Marp presentation template, Clause 9.3 inputs and outputs)
- Roles & Responsibilities (RACI Matrix)
- Document Control Policy & Register
- Audit Policy
- Continual Improvement

### IT Security Policies (Annex A Consolidated)
Located in `/IT-security-policies/`.

22 total consolidated policies aligned to ISO/IEC 27001:2022 Annex A controls:
- Information Security Management  
- Access Control & Identity Management  
- Cryptography & Key Management  
- Network & Infrastructure Security  
- Asset Management & Information Classification  
- Secure Configuration & Hardening  
- Logging, Monitoring & Security Event Management  
- Vulnerability & Patch Management  
- Secure Development & Change Management  
- Backup & Recovery  
- Supplier & Vendor Management  
- Physical & Data Center Security  
- Operations Security  
- Malware Protection & Endpoint Security  
- Cloud Security  
- Incident Response  
- Business Continuity & Disaster Recovery  
- Compliance, Audit & Policy Management  
- Acceptable Use
- Remote Working
- Data Protection & Privacy
- AI Acceptable Use & Governance

### Registers
Located in `/registers/`.
- **risk-register.md** — ISO-aligned risks, mapped to Annex A  
- **asset-register.md** — asset inventory template for cloud-native SaaS  
- **vendor-register.md** — vendor tracking + risk tiering
- **risk-treatment-plan.md** — action plan tracking treatment of each risk to residual acceptance
- **training-register.md** — security awareness & role-based training tracking
- **corrective-action-log.md** — nonconformity/CAPA tracking (Clause 10)
- **legal-regulatory-register.md** — legal, regulatory, and contractual obligations tracker
- **bcdr-test-log.md** — backup restore, failover, and tabletop exercise records
- **metrics-register.md** — ISMS performance metrics and measurement results against information security objectives (Clause 9.1)

### Core ISO Documents
- **ISMS-policies/scope.md** — ISMS scope statement (Clause 4.3)
- **ISMS-policies/context-of-organization.md** — internal/external context and interested parties (Clause 4)
- **soa.md** — Statement of Applicability; all 93 Annex A controls with applicability and references (Clause 6.1.3)
- **internal-audit-checklist.md** — audit evidence record and findings tracker (Clause 9.2)

### Certification Readiness Toolkit
- **gap-analysis.md** — maturity-based gap assessment against ISO/IEC 27001:2022 Clauses 4–10 and Annex A policy areas, used to scope and prioritize an implementation project
- **iso27001-readiness-checklist.md** — tracks status of mandatory documents and operational records toward Stage 1/Stage 2 certification readiness

### Diagrams
Located in `/diagrams/`:
- **aws-multiregion-rescaled.jpg** — architecture diagram (for viewing)
- **aws-multiregion-rescaled.drawio** — source file (for editing in Draw.io)

## How This Repo Works

Documents are structured to reflect a lightweight, audit-ready ISO 27001 ISMS. They are intentionally:
- Concise
- Mapped to ISO 27001:2022
- Generic/sanitized using "CompanyX"
- Optimized for remote-first SaaS teams using AWS

### What This Repo Does Not Contain
- Confidential data  
- Proprietary architecture  
- Real customer information  
- Non-public internal processes  

### What This Repo Provides
- A complete example ISMS suitable for:
  - Interviews
  - Portfolio building
  - Demonstrating GRC and ISO 27001 capabilities
  - Teaching others how to structure an ISMS  
  - Seeding a real ISMS in a startup or scale-up

## How to Use This Repo

1. Clone and adapt for your own organization.  
2. Replace "CompanyX" with your company name.  
3. Update the registers with actual data.  
4. Add evidence folders if using this for a real audit.  
5. Use `/IT-security-policies/` to guide technical controls.  
6. Use `/ISMS-policies/` for ISMS governance structure.  

## AI Tooling
[Claude Code](https://claude.ai/code) was used during the development of this repo to review policy content for gaps, control mapping accuracy, and alignment with ISO/IEC 27001:2022 Annex A. All content was authored, reviewed, and validated by a human with GRC domain expertise.

## License
[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

You are free to copy, adapt, and use this material for any purpose, including commercially, provided you give appropriate credit and link back to this repository.
