# IT Security04 – Network & Infrastructure Security Policy
(Annex A: A.8.20–A.8.23, A.8.27, A.5.14)

## Overview
CompanyX implements layered network and infrastructure security controls to protect its cloud-native, remote-first SaaS environment. This policy defines requirements for network segmentation, firewall configurations, Zero Trust networking, remote access, hardening, and ongoing monitoring across AWS, Entra, and endpoint environments.

## Policy

### 1. Network Segmentation and Architecture  
(Annex A: A.8.20)
- CompanyX must segment networks based on sensitivity and function, including:
  - Public subnets (ingress-only)
  - Private application subnets
  - Private data subnets (no public routing)
  - Management networks
- Security groups and NACLs must enforce least privilege access.
- Direct access to production databases is prohibited unless via approved bastion, SSM Session Manager, or VPN restricted to specific roles.

### 2. Firewall and Traffic Filtering Requirements  
(Annex A: A.8.21)
- Stateful firewalls, AWS security groups, and WAF rules must enforce:
  - Default deny inbound rules
  - Restricted outbound connectivity
  - IP allowlists for administrative interfaces
- AWS WAF must be enabled for public-facing applications where applicable.
- Firewall rules must be reviewed at least quarterly.

### 3. Zero Trust Networking  
(Annex A: A.8.20, A.8.22)
- CompanyX follows Zero Trust principles:
  - Verify explicitly (identity, device posture, geolocation)
  - Enforce least privilege
  - Assume breach
- All remote access requires MFA and conditional access enforcement.
- Lateral movement must be minimized by network segmentation and identity-based controls.

### 4. Remote Access and VPN Requirements  
(Annex A: A.8.21, A.6.7)
- Remote access must use:
  - Entra Conditional Access
  - Approved VPN solutions with MFA
  - Allowed geographic regions based on risk appetite
- Split tunneling is prohibited unless technically required and approved.
- SSH/RDP ports must remain closed to the internet; access must occur through:
  - AWS SSM Session Manager
  - Bastion hosts with logging
  - Zero Trust remote access tools

### 5. Infrastructure Hardening  
(Annex A: A.8.9)
- Hardening baselines must exist for:
  - EC2 instances
  - Containers
  - Endpoints (Windows/macOS)
  - Network appliances
- CIS Benchmarks or equivalent must be applied where applicable.
- Unnecessary services and ports must be disabled.

### 6. Vulnerability Monitoring Across Network Surfaces  
(Annex A: A.8.8, A.8.16)
- The network must be continuously monitored using:
  - Rapid7 SIEM/SOAR
  - AWS GuardDuty
  - AWS Inspector
  - CrowdStrike
- Alerts for suspicious traffic (port scanning, brute force, anomalous geolocation) must be investigated promptly.

### 7. Cloud Network Governance  
(Annex A: A.5.23)
- VPC design changes must go through change management.
- Peering, Transit Gateway, and routing updates must follow approval workflows.
- Public S3 buckets are prohibited unless explicitly approved, logged, and monitored.

### 8. Logging and Monitoring  
(Annex A: A.8.15, A.8.16)
- Logs must be collected from:
  - Network gateways
  - AWS VPC Flow Logs
  - CloudTrail
  - WAF and ALB logs
  - VPN and remote access systems
- Logs must be protected from alteration and retained according to CompanyX policy.
- Network anomalies must be correlated with identity telemetry and endpoint events.

## Policy Conflicts
This policy overrides any legacy networking or firewall configuration standards. More restrictive business or regulatory requirements take precedence.

## Enforcement
Failure to comply may result in access revocation, disciplinary action, or termination. Intentional bypass of network security controls may trigger formal investigation.

## Ownership
Security Department (Security Engineering & Cloud Infrastructure)

## Document Version History

| Version | Author             | Date       | Changes          | Approved By |
|---------|--------------------|------------|------------------|-------------|
| 1.0     | Security Department| 2025-04-01 | Initial creation | CISO / CTO  |
