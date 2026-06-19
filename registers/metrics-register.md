# CompanyX Information Security Metrics Register
ISO/IEC 27001:2022 Clause 9.1 — Monitoring, Measurement, Analysis and Evaluation  
Last Updated: 2026-06-19  
Next Review Due: Q3-2026 Management Review

## Purpose
Record measurement results for each Information Security Objective defined in [objectives.md](../ISMS-policies/objectives.md), satisfying the documented-information requirement of ISO/IEC 27001:2022 Clause 9.1. Results are reviewed quarterly by the Security Department and presented at each Management Review as a required Clause 9.3.2 input (see [management-review.md](../ISMS-policies/management-review.md)).

## Reporting Periods

| Period Label | Calendar Period |
|-------------|----------------|
| Q3-2025 | Jul – Sep 2025 |
| Q4-2025 | Oct – Dec 2025 |
| Q1-2026 | Jan – Mar 2026 |
| Q2-2026 | Apr – Jun 2026 |

Quarterly metrics report each period. Annual metrics report in the quarter when measurement occurs; remaining quarters show —.

---

## Metrics

| Metric ID | Metric | Linked Objective | Target | Measurement Method | Data Source | Frequency | Owner | Q3-2025 | Q4-2025 | Q1-2026 | Q2-2026 | Trend |
|-----------|--------|-----------------|--------|-------------------|-------------|-----------|-------|---------|---------|---------|---------|-------|
| MET-01 | Production service uptime | Maintain CIA of SaaS platform; uptime ≥ 99.9% | ≥ 99.9% monthly average uptime | Aggregate CloudWatch availability metrics across all production services; calculated monthly, reported quarterly | AWS CloudWatch / status page | Monthly (reported quarterly) | Engineering Lead | 99.97% ✓ | 99.85% ✗ | 99.94% ✓ | 99.98% ✓ | ↑ Recovering after Q4-2025 incident (65-min unplanned outage Nov-25); corrective action closed Q1-2026 |
| MET-02 | Access review participation rate | Complete quarterly access reviews with 100% participation | 100% of scheduled reviewers complete certification within the review window | Count completed certifications vs. total required per review cycle; tracked per cycle in Entra ID and Jira | Entra ID access reviews / Jira | Quarterly | Security Department | 96% ✗ (2 contractors missed) | 100% ✓ | 100% ✓ | 100% ✓ | ↑ Three consecutive quarters at target following process update in Q4-2025 |
| MET-03 | Critical vulnerability resolution SLA | Resolve critical vulnerabilities within 7 days | 100% of Critical (CVSS ≥ 9.0) findings remediated or formally risk-accepted within 7 calendar days of detection | % of critical findings closed within SLA per scan cycle; tracked per finding in Rapid7 | Rapid7 Vulnerability Management | Monthly (reported quarterly) | Security Department | 87% ✗ (2 of 15 exceeded SLA) | 94% ✗ (1 of 17 exceeded SLA — third-party dependency) | 100% ✓ (12 of 12) | 100% ✓ (8 of 8) | ↑ At target for two consecutive quarters; patching runbook updated Q4-2025 after SLA breaches |
| MET-04 | Internal audit completion | Complete annual internal audit | 1 full-scope internal audit completed per year; all findings tracked to closure within agreed timelines | Audit completion status confirmed; % of findings closed by agreed target dates | Internal audit report; corrective-action-log.md | Annual | ISMS Manager / Internal Auditor | — | Completed Oct-2025 ✓; 3 minor findings raised | 2 of 3 findings closed | All 3 findings closed ✓ | ✓ 2025 audit delivered on schedule; all findings resolved by Q2-2026 |
| MET-05 | Management review completion | Complete annual management review | Formal management review conducted at least annually; all Clause 9.3.2 inputs addressed; decisions and actions documented | Review completion confirmed; minutes produced; action items logged in corrective-action-log.md | management-review.md | Annual | CISO / CTO | — | Completed Dec-2025 ✓; all Clause 9.3 inputs documented | Q4-2025 actions in progress | All Q4-2025 actions closed ✓; 2026 review scheduled Q4-2026 | ✓ Conducted in 2024 and 2025; actions tracked to closure |
| MET-06 | ISO 27001 open nonconformities | Ensure compliance with ISO 27001 | Zero unresolved major nonconformities at any time; minor nonconformities closed within agreed timelines | Count of open major and minor nonconformities at end of period | corrective-action-log.md; internal audit reports | Quarterly | ISMS Manager | 0 major, 2 minor open ✓ | 0 major, 3 minor open ✓ (3 new from Oct-2025 audit) | 0 major, 1 minor open ✓ | 0 major, 0 minor open ✓ | ↑ All items cleared entering Q3-2026; zero major nonconformities maintained throughout all periods |
| MET-07 | Customer security commitment breaches | Ensure compliance with customer commitments | Zero unresolved customer-reported security obligation breaches | Count of contractual security obligations breached or formally escalated by customers during the period | Customer incident log; legal-regulatory-register.md | Quarterly | Security Department / Legal | 0 ✓ | 0 ✓ | 0 ✓ | 0 ✓ | ✓ No customer-reported security commitment breaches in any reported period |

---

## Result Indicators

| Symbol | Meaning |
|--------|---------|
| ✓ | Met target |
| ✗ | Missed target — nonconformity or observation to be raised |
| — | Not measured this period (annual metric) |
| ↑ | Improving trend |
| → | Stable / sustained at target |
| ↓ | Declining trend — escalation required |

---

## Escalation
- Any metric that misses its target must be raised in corrective-action-log.md as a nonconformity or observation within 5 business days.
- Two or more consecutive missed periods for the same metric must be escalated to the CISO for formal risk acceptance or revised treatment.
- All metric results are reviewed at management reviews per management-review.md.

## Ownership
Security Department (ISMS Manager)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|---------|------------|----------------|--------------|
| 1.0 | Security Department | 2026-06-19 | Initial creation | CISO / CTO |
