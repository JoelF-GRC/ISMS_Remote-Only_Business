# CompanyX Data Protection Impact Assessment (DPIA) Log
ISO/IEC 27001:2022 Annex A: A.5.34 · GDPR Article 35
Last Updated: 2026-07-02

## Purpose
Implement IT Security21 (Data Protection & Privacy Policy) Section 7: a documented process and log for Data Protection Impact Assessments, required before commencing any processing activity likely to result in high risk to individuals.

This is the "existing GDPR DPIA process" referenced by IT Security21 Section 7 and by the companion AI Management System's AI-Gov05 Section 7 (GDPR DPIA Threshold Assessment for AI Features). AI-Gov05 Section 7 runs a lighter, AI-specific *threshold screening* before a full DPIA is triggered; where that screening concludes a full DPIA is required, it is conducted and logged here using the same process and template used for any other high-risk processing activity.

## When a DPIA Is Required
Per IT Security21 Section 7, a DPIA is mandatory before commencing any processing activity likely to result in high risk to individuals, including:
- Large-scale processing of sensitive categories of data
- Systematic monitoring of publicly accessible areas or employee activity
- Use of new technologies (including AI tools processing personal data)
- Automated decision-making or profiling with significant effects

For AI features specifically, run the threshold screening in AI-Gov05 Section 7 first. A "yes" to any of screening questions 1–3 there triggers a full DPIA, logged below. A "yes" to questions 4–6 (with 1–3 all "no") requires only the lightweight documented assessment described in AI-Gov05 Section 7, recorded in the AI system inventory rather than here.

## DPIA Process
1. Screen the proposed processing activity against the triggers above (or against AI-Gov05 Section 7 for an AI feature).
2. If a full DPIA is required, complete the assessment: describe the processing, assess necessity and proportionality, identify risks to individuals, and define mitigating measures.
3. The Privacy function reviews and signs off the completed DPIA before the processing activity begins.
4. Record the outcome below and cross-reference the relevant RoPA entry (`ropa.md`) and, for an AI feature, the relevant AI system inventory entry in the companion AIMS repository.
5. Re-run the DPIA if the processing activity materially changes.

## DPIA Log

| ID | Date | Processing Activity Assessed | Trigger | Risks Identified | Mitigating Measures | Outcome | RoPA Cross-Reference | AI System Inventory Cross-Reference (if applicable) | Reviewed By (Privacy) | Review Date |
|----|------|-------------------------------|---------|--------------------|------------------------|---------|-------------------------|----------------------------------------------------------|--------------------------|---------------|
| DPIA-001 | | | | | | | | | | |

---

## Retention
Completed DPIAs are retained for audit purposes for a minimum of three years, consistent with CompanyX's ISO 27001 record-retention practice.

## Ownership
Privacy function (GRC), with Legal counsel input where applicable.

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|--------|-----------|--------------|-------------|
| 1.0 | Security Department | 2026-07-02 | Initial creation, implementing IT Security21 Section 7 and providing the concrete "existing GDPR DPIA process" referenced by AI-Gov05 Section 7 in the companion AIMS repository | CISO / CTO |
