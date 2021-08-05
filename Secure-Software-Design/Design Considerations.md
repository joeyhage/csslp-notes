# Design Considerations

## Application of Methods to Address Core Security Concepts

### Confidentiality, Integrity, and Availability
- need to be considered/added during design phase
- Examples of tools:
  - Confidentiality -> encryption
  - Integrity -> hashing
  - Availability -> recovery

#### Confidentiality
- data at rest usually encrypted differently than data in transit
- data needed to be confidential in use (encryption key), requires specific attention
- after elements needing to be kept confidential are determined, next need to determine authorized parties

#### Integrity
- controls update and delete
- first aspect is applying controls (e.g. ACLs)
- second aspect (just as important) is determining if data _has_ been altered
  - digests should be stored and transmittted separately

#### Availability
- system is available to _authorized_ users when appropriate
- many options including backups, data replication, failovers
  - just need to determine the need and write a requirement

### Authentication, Authorization, and Auditing
- generally, best to integrate with the existing enterprise environment and/or operating system

#### Authentication
- if incorrect, everything else is wrong
- determine level of confidence needed
- use OS methods when possible, otherwise follow design patterns

#### Authorization
- use OS methods when possible, otherwise follow design patterns

#### Accounting (Audit)
- logging activity
- during design, determine what should be logged and when
- include error trapping and log what devs need to debug problem
- if sensitive data is logged, encryption is needed
- don't log data like PII or paths/filenames

## Secure Design Principles
