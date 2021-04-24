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
3. Object
  - file, program, data, other resource
4. Type/level of access to be granted
  - Read, write, create, delete, right to grant access rights to other objects

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

### Secure Design Tenets

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
