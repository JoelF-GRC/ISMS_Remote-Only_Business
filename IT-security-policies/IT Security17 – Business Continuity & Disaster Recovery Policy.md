# IT Security17 – Business Continuity & Disaster Recovery Policy
(Annex A: A.5.29, A.5.30, A.8.14)

## Overview
CompanyX maintains business continuity and disaster recovery (BC/DR) capabilities to ensure the resilience and ongoing delivery of services during disruptions. This policy defines requirements for continuity planning, recovery objectives, testing, and crisis communication.

## Policy

### 1. Business Continuity Planning  
(Annex A: A.5.29, A.5.30)
- Business functions must conduct Business Impact Assessments (BIAs) at least every two years.
- BIAs must identify:
  - Critical systems and processes
  - Maximum tolerable downtime (MTD)
  - Recovery Time Objective (RTO)
  - Recovery Point Objective (RPO)
- Continuity plans must be documented and maintained by each department.

### 2. Climate-Related Continuity Requirements
BC/DR plans must include consideration of:
- Regional AWS data center disruptions due to severe weather
- Remote workforce outages (power, internet, natural disasters)
- Supplier climate-related outages
- Restoration scenarios involving relocation of workloads to unaffected regions


### 3. Disaster Recovery Planning  
(Annex A: A.8.13, A.8.14)
- Disaster recovery procedures must be defined for:
  - AWS production environments
  - Core SaaS applications (Jira, Entra ID, GitHub, etc.)
  - Datastores (RDS, S3, DynamoDB)
- AWS workloads must use:
  - Multi-AZ redundancy by default
  - Backup and snapshot schedules aligned to RPO/RTO requirements
  - Replication capabilities (e.g., S3 CRR) for critical workloads

### 4. Backup and Restoration  
- Backups must be:
  - Encrypted
  - Tested at least quarterly
  - Stored in separate AZs or regions
- Restoration tests must validate:
  - Data integrity
  - Recovery procedures
  - RTO/RPO alignment

### 5. Crisis Communication  
- Communication during incidents must follow:
  - Defined internal escalation paths
  - Pre-approved external communication templates
  - Coordination among Security, Engineering, Leadership, and Legal
- Unauthorized individuals must not communicate externally about CompanyX incidents.

### 6. Continuity Testing  
- BC/DR plans must be tested at least annually.
- Test types may include:
  - Tabletop exercises
  - Partial or full failover tests
  - Simulation of cloud outages
- Tests should include at least one climate-related scenario annually (e.g., wildfire smoke event, regional AWS outage).
- Test results must be documented and corrective actions tracked to completion.

### 7. Climate Scenario Testing Requirements
At least one BC/DR exercise per year should simulate a climate-related failure such as:
- AWS regional outage due to weather
- Remote workforce unable to access systems due to local emergency
- Vendor outage due to climate-related power failure
- Network connectivity interruptions across an affected geography

### 8. Third-Party Dependencies  
- Critical suppliers must maintain BC/DR programs.
- CompanyX must review:
  - SOC reports
  - Continuity test summaries
  - Status pages and outage patterns

## Policy Conflicts
This policy supersedes any informal continuity or recovery plans unless approved by Security.

## Enforcement
Failure to adhere to BC/DR responsibilities may result in disciplinary action or removal of system access.

## Ownership
Security Department (Business Resilience & Continuity)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|---------|-----------|--------------|-------------|
| 1.0 | Security Department | YYYY-MM-DD | Initial creation | CISO / CTO |
