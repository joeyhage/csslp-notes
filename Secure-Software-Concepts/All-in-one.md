# General Security Concepts

## General Security Concepts

### Security Basics
Determining and applying the appropriate balance of confidentiality, integrity, and availability (CIA)
Although different, they are not necessarily contradictory - but they all require resources (money) and so the balance should be determined early on in the design process

#### Confidentiality
###### Prevent disclosure of information to unauthorized parties
Numerous methods for keeping data confidential: e.g. access controls, encryption

**Access Controls**: Preferred for data in use and at rest
**Encryption**: Data at rest and in transit

#### Integrity
###### Protect data from unauthorized alteration
e.g. Read-only, Read-and-write, write-only, delete access, etc
Integrity contributes to a system's **stability** and **reliability** as well as the **authenticity** of data

#### Availability
Availability needed is determined by criticality of data and purpose in the overall system

#### Authentication
###### Determining the **identity** of a user. A user is authenticated before their authorization can be determined.

To verify identity, a user can provide:
- Something you know - e.g. username/password (not very reliable)
- Something you have - e.g. token
- Something about you (something you are) e.g. biometrics
  - Requires extra hardware, lacks specificity
New categories
- what users do (dynamic biometrics such as typing patterns, gait)
- where a user is (physical location)

ATMs use combination of something you know (PIN) and something you have (card) so if the card is lost, someone cannot authenticate as you

#### Authorization
###### Applies predetermined access levels to the user

Three elemends are used:
1. Requestor (subject) - already known due to authentication system
2. Object
   1. file, program, data, other resource
3. Type/level of access to be granted
   1. Read, write, create, delete, right to grant access rights to other objects

#### Accounting (Auditing)
###### Accounting is a means of measuring activity, auditing is the verification of what actual happened and allows management to observe in a nonpartisan manner

Accounting can be done in IT systems by logging crucial activity as it occurs
Accounting is needed when activity of specific data elements is crucial enough that it may be audited at a later date and time

Security level auditing can be performed at several levels: 
- analysis of logging function
- verification of existence and operation of specific controls
- etc

Auditing takes resources to create, store, and review. Typically defaulted to minimal level so system operator must detemine correct level based on system criticality.

**System criticality** is determed by information criticality associated with information manipulated/stored with the system


#### Non-repudiation
###### Preventing a subject from denying a previous action with an object
When authentication, authorization, and auditing are properly configured, non-repudiation is ensured
**Security requirements must specify the subjects, objects, and events for which non-repudiation is desired**

### System Tenets

#### Session Management
###### Design and implementation of controls to ensure that communication channels are secured from unauthorized access and disruption
TCP (Transmission Control Protocol)
- sequential numbering of packets and retransmission for missing packets
- Prevents unauthorized packets and session hijacking
- Has overhead
UDP (User Datagram Protocol)
- connectionless/sessionles

#### Exception Management
- All exceptions must be detected and handled
- System should not fail in an insecure state
- Exception should not be leaked

#### Configuration Management
Configuration should be protected from unauthorized changes
e.g. separation of duties between production/non-prod personnel

### Secure Design Tenets

#### Good Enough Security
Don't spend $10,000 to protect a $20 bill
Trade-offs exist between security and other aspects

#### Least Privilege
If a subject may require different levels of security for different tasks, better to switch security levels with specific tasks than run all the time at higher privilege

#### Separation of Duties
No single individual can abuse the system

#### Defense in Depth
i.e. layered security/defense and diversity defense
Multiple, overlapping defenses
No system is 100% secure - **true goal of security is to make cost of compromising greater in time/effort/resources than it is worth**

Diversity of defense - layers should be dissimalr in nature

#### Fail-safe
###### When a system experiences a failure, it should fail to a safe state
Example: explicit deny
CIA need to be appropriately maintained - availability causes the greatest design difficulties

#### Economy of Mechanism
Higher complexity generally results in less security due to lack of understanding and more attack vectors
Root cause analysis, especially for potential security issues, is much more difficult in complex systems
**Rule of thumb**: eliminate all nonessential services and protocols

#### Complete Mediation
###### Authorization is never circumvented, even with repeated access
Example: security kernel

#### Open Design
Don't rely on security by obscurity
Example: modern cryptography relies on the secrecy of the key, not secrecy of the algorithm

#### Least Common Mechanism
###### Prevent inadvertent sharing of information by using separate processes when possible

#### Psychological Acceptability
Users will try to get around security if it is seen as an obstacle

#### Weakest Link
Adding to the security of a system is most effective when applied to the weakest link

#### Leveraging Existing Components
Pros: increase efficiency and security
Cons: monoculture environment (failures have a larger footprint)

#### Single Point of Failure
No one single piece should be able to cause the whole system to fail

## Security Models

### Access Control Models

### Multilevel Security Model

### Integrity Models

### Information Flow Models

## Adversaries

### Adversary Type

### Adversary Groups

### Threat Landscape Shift

## Review

# Risk Management

# Security Policies and Regulations

# Software Development Methodologies
