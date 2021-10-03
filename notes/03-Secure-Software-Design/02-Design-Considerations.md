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
  - digests should be stored and transmitted separately

#### Availability

- system is available to _authorized_ users when appropriate
- many options including backups, data replication, fail-overs
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

### Good Enough Security

- security should match risk associated with potential vulnerability

### Least Privilege

- natural set of defenses when unexpected things happen

### Separation of Duties

- useful when multiple conditions must be met

### Defense in Depth

- multiple overlapping defenses, dissimilar in nature (e.g. encryption and ACLs)
- one of the oldest security principles
- wider range of threats more efficiently
- **Every piece of software can be compromised/bypassed in some way**

### Fail Safe

- what happens when an element fails?
- degrade gracefully and return to normal through the shortest path

### Economy of Mechanism

- Smaller and simpler = easier to secure
- Extensibility and reuse improve stability
- simple to troubleshoot, expand, use, and administer

### Complete Mediation

- perform authorization checks for sensitive operations
- don't assume a subject has permission

### Open Design

- open communication
- accessible and understandable designs

### Least Common Mechanism

- reusing existing components can create pathways between users/processes
- determine balance between reuse and separation

### Psychological Acceptability

- users are key to system and security
- if security obstructs the user and user disagrees, user will find a workaround
- ensure abnormal system behavior is comprehensible to the user (i.e. don't say, "contact your sysadmin")

### Weakest Link

- analyze local and system views of an application
- prevent local errors from becoming system failures

### Leverage Existing Components

- reduces costs and simplifies programs but failures have larger footprints
- legacy code and 3rd party code still need security reviews

### Single Point of Failure

- single failure should not result in a system failure

## Inter-connectivity

### Session Management

- prevent unauthorized party taking control of authorized communication
- cross-party disclosure should not occur

### Exception Management

- communicate error to user and log information

### Configuration Management

- secure configuration files/elements

## Interfaces

- determine method and level of integration with enterprise resources
- in-band vs out-of-band management of application
- creating separate management interface vs sending information to enterprise management system
