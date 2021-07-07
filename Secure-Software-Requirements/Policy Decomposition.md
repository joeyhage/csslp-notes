# Policy Decomposition

## Computer Security Policies
1. program policies: foundational for infosec program
2. issue-specific policies: specific issues such as PII or data retention
3. system-specific policies: technical directives such as firewall rules

Regulations and government directives are also sources of security requirements

## Confidentiality, Integrity, and Availability Requirements

### Confidentiality
- Who is authorized to see what data
- mechanism to enforce
- business requirements with respect to data collection, transfer, storage, and use

### Integrity
- who is authorized to alter what data
- mechanism to detect errors and enforce
- business requirements with respect to data collection, transfer, storage, and use

### Availability
- available to authorized users when needed
- deny unauthorized
- prevent DoS

## Authentication, Authorization, and Auditing Requirements

### Identification and Authentication
Identity Requirements:
- identity mechanism
- mgmt of identities, incl. reaffirmations

Authentication Requirements:
- method of authentication
- strength of authentication

- Most authentication is one party authenticating the other (bank auth. account holder)
- Sometime mutual authentication is used (both parties authenticating each other simultaneously) to prevent MITM attacks

### Access Control Mechanisms

#### Mandatory access control MAC
#### Discretionary access control DAC
#### Role-based access control RBAC
#### Rule-based access control RBAC

