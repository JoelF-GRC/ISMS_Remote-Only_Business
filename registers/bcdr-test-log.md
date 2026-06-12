# CompanyX BCDR Test Log
ISO/IEC 27001:2022 Annex A: A.5.30, A.8.13–A.8.14
Last Updated: YYYY-MM-DD

## Purpose
Record business continuity and disaster recovery tests, including backup restoration tests, failover exercises, and tabletop scenarios, satisfying A.5.30 (ICT readiness for business continuity), A.8.13 (Information backup), and A.8.14 (Redundancy of information processing facilities).

## Test Types
- **Backup Restore Test** – Verify backups can be restored and data integrity is intact.
- **Failover Test** – Verify multi-AZ/multi-region failover for production workloads.
- **Tabletop Exercise** – Walkthrough of an incident/continuity scenario with relevant teams, including climate-related scenarios per [climate-change-addendum.md](../climate-change-addendum.md).
- **Communications Test** – Verify incident communication channels and escalation paths function as expected.

---

## Test Log

| Test Date | Test Type | Scope | Scenario | Outcome | Issues Identified | Corrective Actions | Owner | Next Test Due |
|------------|-----------|-------|----------|----------|----------------------|----------------------|-------|----------------|
| | Backup Restore Test | RDS (Prod) | Restore from latest automated snapshot | | | | Infra | |
| | Failover Test | AWS Multi-AZ Production | Simulated AZ outage | | | | Cloud | |
| | Tabletop Exercise | Regional cloud outage (climate-related) | Severe weather impacting us-east-1 | | | | Security/Infra | |

---

## Frequency
- Backup restore tests: at least quarterly.
- Failover tests: at least annually.
- Tabletop exercises (including climate-related scenarios): at least annually, per [risk-methodology.md](../ISMS-policies/risk-methodology.md).

## Reporting
Results and corrective actions must be reported at management review (see [management-review.md](../ISMS-policies/management-review.md)) and logged in [corrective-action-log.md](corrective-action-log.md) if issues are identified.

## Ownership
Infrastructure/Cloud Team, with Security Department oversight.
