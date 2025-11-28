# IT Security03 – Cryptography & Key Management Policy
(Annex A: A.8.24–A.8.29)

## Overview
CompanyX uses cryptographic controls to protect information at rest, in transit, and in use across its cloud-native SaaS environment. This policy defines requirements for encryption, key management, certificate governance, and the secure use of cryptographic technologies.

## Policy

### 1. Cryptographic Requirements  
(Annex A: A.8.24)
- Cryptographic controls must follow industry best practices and applicable regulations.
- Encryption must be used to protect sensitive data:
  - At rest (AWS KMS, service-managed encryption)
  - In transit (TLS 1.2+)
  - In use where applicable (memory encryption, hardware-backed secure enclaves)
- Weak or deprecated algorithms (e.g., SHA-1, TLS 1.0/1.1, 3DES) are prohibited.

### 2. Key Management  
(Annex A: A.8.25)
- All cryptographic keys must be:
  - Generated using approved algorithms and entropy sources.
  - Stored in secure key management systems (AWS KMS).
  - Rotated annually or on compromise.
- Access to keys must follow least privilege and be monitored.

### 3. Key Protection and Handling  
(Annex A: A.8.26)
- Keys must never be stored in plaintext, source code, or unsecured configuration files.
- Secrets must be stored in:
  - AWS Secrets Manager
  - Parameter Store (SecureString)
  - Entra Managed Identities or secure vault technologies
- Transmission of keys must use encrypted channels.

### 4. Certificate Management  
(Annex A: A.8.27)
- Certificates must be:
  - Issued by approved certificate authorities.
  - Monitored for expiration.
  - Renewed before expiration.
- Private keys must never leave their secure storage location.

### 5. Cryptographic Roles and Responsibilities  
(Annex A: A.8.28)
- The Security Department must:
  - Approve cryptographic tools and libraries.
  - Maintain an inventory of cryptographic assets.
  - Monitor use of encryption and key management systems.
- Engineering must ensure applications use approved cryptographic methods.

### 6. Cryptographic Governance  
(Annex A: A.8.29)
- All cryptographic mechanisms must be periodically reviewed.
- Risks involving cryptography (e.g., algorithm deprecation) must be documented in the risk register.
- Changes to encryption standards must be approved through the change management process.

## Policy Conflicts
If conflicts occur between this policy and product-level technical requirements, the stronger security requirement takes precedence. Exceptions require documented risk acceptance.

## Enforcement
Failure to comply may result in disciplinary action up to termination. Improper handling of keys or secrets may result in immediate access revocation and investigation.

## Ownership
Security Department (Security Architecture & Engineering)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|---------|------------|----------------|--------------|
| 1.0 | Security Department | YYYY-MM-DD | Initial creation | CISO / CTO |

(Annex A: A.8.24–A.8.29)

## Overview
CompanyX uses cryptographic controls to protect information at rest, in transit, and in use across its cloud-native SaaS environment. This policy defines requirements for encryption, key management, certificate governance, and the secure use of cryptographic technologies.

## Policy

### 1. Cryptographic Requirements  
(Annex A: A.8.24)
- Cryptographic controls must follow industry best practices and applicable regulations.
- Encryption must be used to protect sensitive data:
  - At rest (AWS KMS, service-managed encryption)
  - In transit (TLS 1.2+)
  - In use where applicable (memory encryption, hardware-backed secure enclaves)
- Weak or deprecated algorithms (e.g., SHA-1, TLS 1.0/1.1, 3DES) are prohibited.

### 2. Key Management  
(Annex A: A.8.25)
- All cryptographic keys must be:
  - Generated using approved algorithms and entropy sources.
  - Stored in secure key management systems (AWS KMS).
  - Rotated annually or on compromise.
- Access to keys must follow least privilege and be monitored.

### 3. Key Protection and Handling  
(Annex A: A.8.26)
- Keys must never be stored in plaintext, source code, or unsecured configuration files.
- Secrets must be stored in:
  - AWS Secrets Manager
  - Parameter Store (SecureString)
  - Entra Managed Identities or secure vault technologies
- Transmission of keys must use encrypted channels.

### 4. Certificate Management  
(Annex A: A.8.27)
- Certificates must be:
  - Issued by approved certificate authorities.
  - Monitored for expiration.
  - Renewed before expiration.
- Private keys must never leave their secure storage location.

### 5. Cryptographic Roles and Responsibilities  
(Annex A: A.8.28)
- The Security Department must:
  - Approve cryptographic tools and libraries.
  - Maintain an inventory of cryptographic assets.
  - Monitor use of encryption and key management systems.
- Engineering must ensure applications use approved cryptographic methods.

### 6. Cryptographic Governance  
(Annex A: A.8.29)
- All cryptographic mechanisms must be periodically reviewed.
- Risks involving cryptography (e.g., algorithm deprecation) must be documented in the risk register.
- Changes to encryption standards must be approved through the change management process.

## Policy Conflicts
If conflicts occur between this policy and product-level technical requirements, the stronger security requirement takes precedence. Exceptions require documented risk acceptance.

## Enforcement
Failure to comply may result in disciplinary action up to termination. Improper handling of keys or secrets may result in immediate access revocation and investigation.

## Ownership
Security Department (Security Architecture & Engineering)

## Document Version History

| Version | Author | Date | Changes | Approved By |
|--------|---------|------------|----------------|--------------|
| 1.0 | Security Department | YYYY-MM-DD | Initial creation | CISO / CTO |
