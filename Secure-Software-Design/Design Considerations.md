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
