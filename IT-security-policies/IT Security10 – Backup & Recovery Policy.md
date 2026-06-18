# IT Security10 – Backup & Recovery Policy
(Annex A: A.8.13, A.8.10, A.5.30)

## Overview
CompanyX implements and maintains backup and recovery capabilities to ensure data availability and integrity in the event of system failure, data loss, corruption, or disaster.

## Policy

### 1. Backup Requirements  
(Annex A: A.8.13)
- Backups must be created for:
  - Application databases
  - Critical configuration data
  - IAM data where applicable
  - Logs required for business or compliance purposes
- Backups must be encrypted at rest and in transit.

### 2. Backup Frequency  
- Production systems must be backed up:
  - Databases: at least daily, with point-in-time recovery where feasible
  - Critical infrastructure: daily
  - Logs: continuous or near-real-time
- Non-production backups must follow business requirements.

### 3. Retention  
- Backup retention must comply with legal, regulatory, and contractual requirements.
- Typical minimum retention: 30–90 days depending on data type.

### 4. Restoration Testing  
(Annex A: A.5.30)
- Backup restoration tests must be performed at least quarterly.
- Results must be documented, reviewed, and tracked by the Security Department.

### 5. Isolation of Backups  
- Backups must be stored in:
  - Separate AWS regions or availability zones
  - Immutable storage where required (e.g., S3 Object Lock)
- Backup access must follow least privilege.

### 6. Failure Handling  
- Backup failures must be alerted, logged, and resolved within defined SLAs.

## Policy Conflicts
If system performance conflicts with backup schedules, Security must assess and approve adjustments.

## Enforcement
Failure to comply may result in disciplinary action or revocation of system access.

## Ownership
Security Department (Infrastructure & Resilience)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|---------|-----------|--------------|--------------|
| 1.0 | Security Department | YYYY-MM-DD | Initial creation | CISO / CTO |
