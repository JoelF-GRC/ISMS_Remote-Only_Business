# CompanyX Risk Treatment Plan
ISO/IEC 27001:2022 Clause 6.1.3(e)
Last Updated: YYYY-MM-DD

## Purpose
The Risk Treatment Plan (RTP) translates risk treatment decisions recorded in [risk-register.md](risk-register.md) into a concrete, owned, time-bound action plan. While the risk register captures *what the risk is and what control reduces it*, the RTP tracks *what specifically needs to be done, by whom, by when, and with what resources* — and records leadership approval of the residual risk.

## Relationship to the Risk Register
- Each row below should reference a Risk ID from `risk-register.md`.
- A single risk may have multiple treatment actions (one row each).
- Once all actions for a risk are complete and the residual risk is acceptable, the risk register's "Status" should be updated to `Mitigated` or `Accepted`.

---

## Treatment Options
- **Mitigate** – Reduce likelihood or impact via controls.
- **Avoid** – Eliminate the risk by removing the asset, process, or activity.
- **Transfer** – Share or shift the risk (e.g., insurance, outsourcing with contractual liability).
- **Accept** – Formally accept the residual risk with leadership sign-off (no further action planned).

---

## Risk Treatment Plan Table

| Risk ID | Treatment Option | Action / Control to Implement | Resources Required | Owner | Target Date | Status | Residual Risk Approved By | Approval Date |
|---------|-------------------|--------------------------------|----------------------|-------|--------------|--------|------------------------------|----------------|
| R-001 | Mitigate | Enforce Conditional Access MFA for all Entra ID users | Entra ID P2 licensing | IAM Lead | | Not Started | | |
| R-008 | Accept | Document insider-threat residual risk acceptance; rely on PIM + logging | None | Security | | Pending Approval | | |
| R-013 | Accept | Document data retention residual risk acceptance pending policy update | None | GRC | | Pending Approval | | |
| | | | | | | | | |

---

## Review
- The RTP must be reviewed at least quarterly by the Security Department.
- Risk acceptances (Treatment Option = Accept) require sign-off from Security and Leadership, recorded in the "Residual Risk Approved By" / "Approval Date" columns.
- Updates to this plan should be reflected back into `risk-register.md` (Residual Risk and Status columns).

## Ownership
Security Department (ISMS Manager)
