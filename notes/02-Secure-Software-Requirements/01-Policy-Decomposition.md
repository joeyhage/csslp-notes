# Policy Decomposition

## NIST Computer Security Policies 📝

1. **program policies:** foundational for infosec program
2. **issue-specific policies:** specific issues such as PII or data retention
3. **system-specific policies:** technical directives such as firewall rules

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
- deny unauthorized/illegitimate access
- prevent DoS

## Authentication, Authorization, and Auditing Requirements

### Identification and Authentication

Identity Requirements:

- identity mechanism
- mgmt of identities, incl. reaffirmations

Authentication Requirements:

- method of authentication
- strength of authentication

📝 Three general authentication factors

1. Something you know
2. Something you have
3. Something you are

- 📝 Most authentication is one party authenticating the other (bank auth. account holder)
- 📝 Sometime mutual authentication is used (both parties authenticating each other simultaneously) to prevent MITM attacks

### Access Control Mechanisms

#### Mandatory access control MAC

- Much more restrictive
- Access determined by security classification
- Each subject and object has a label, operating system determines if access is granted
- also implements "need to know" - just because a subject has appropriate clearance, does not mean they will be able to access

#### Discretionary access control DAC

- owner of object determines access levels
- ACLs (access control lists)

#### Role-based access control RBAC

- doesn't use ACLs, uses roles (like AD groups)
- users are assigned to roles and roles are assigned access

#### Rule-based access control RBAC

- Uses ACLs but adds rules into ACLs
- MAC can use rule-based for implementation
- rules can be things like dates/times access is allowed
- users are not allowed to change rules

#### Attribute-based access control (ABAC)

- attributes/specific elements of the data/object are used to determine access
- e.g. if a patient has a certain attribute (is receiving certain treatment), that determines which doctors/staff can access

### Auditing

#### risk based issues

📝 audit related risk:

1. **inherent risk**: inherent error rate before controls
2. **detection risk**: audit will not detect it
3. **control risk**: controls will not detect or prevent in a timely fashion

#### Organizational characteristics

Examples:

- organizational history
- business env
- supervisory issues

**organizational security elements:**

- roles and responsibilities
- separation of duties
- training and qualifications
- change mgmt
- control mgmt

## Internal security reqs

Items used by the system to protect data and communications, for example:

- protect audit logs
- manage data loss prevention elements
- monitor internal system traffic
- monitor internal controls
- protect configuration files

## External security reqs

statutory and regulatory regulations, contractual obligations, for example:

- use security controls to manage external connections
- manage external connections and authentication
- content filtering and proxies to protect against web-based threats
