# Terms

## Secure Design Tenets

### Good Enough Security

Appropriate level of security for any given system. 

### Least Privilege

Programs and users (subjects) should only have the bare minimum rights and privileges to perform current task

### Separation of Duties

More than one person needs to be involved for any given task so no single person can abuse the system

### Defense in Depth

A.k.a. layered security or diversity defense.

Software should have multiple layers of defenses that are dissimilar in nature. ❗ True goal of security is to make the cost/time/effort of exploiting a system more than it is worth to an adversary.

### Fail-safe

When a system fails, it should fail to a safe state. E.g. explicit deny

### Economy of Mechanism

Greater system or software complexity generally results in worse security. Troubleshooting issues gets more difficult the more complex something is. This also includes turning off/disabling protocols and services that are not needed.

### Complete Mediation

When a subject is authorized, verification should occur every time access to an object is requested.

### Open Design

❗ Security by obscurity does not provide actual security!

### Least Common Mechanism

Multiple, different processes that share common mechanisms can lead to inadvertent sharing of information. Better to keep processes completely separate.

### Leverage Existing Components

Reuse components so the attack surface of a system is reduced. ❗ This often results in a larger footprint when errors occur.

### Psychological Acceptability

When securing a system or software, the controls should not obstruct the user and ease-of-use enough that the user is motivated to circumvent the controls.

### Weakest Link

This is the common point of failure for all systems. A system is only as strong as its weakest link.

### Single Point of Failure

An entire system should not fail if a single aspect fails.

## Access Control Models

### Mandatory Access Control

Restrict access based on sensitivity of the information in the object and whether the subject is authorized to access information with that level of sensitivity.

### Discretionary Access Control

The owner of an object specifies which subjects have access and what level of access each subject has. 
❗ It is optional (discretionary) and requires owner to define access for all objects under its control.

### Role-based Access Control

A user is assigned to any number of potentially overlapping roles. Roles are then assigned access.

### Rule-based Access Control

Building rules into ACLs. Examples include time-of-day or network restrictions.

### Attribute-based Access Control

Grant access based on attributes associated with the subject.

### Simple Security Rule

Subjects can only read objects they are authorized to read.

## Qualitative risk assessment

Subjectively determine impact of an event - involves experts and group consensus

## Quantitative risk assessment

Objectively determine impact of an event - involves use of metrics and models

## Single loss expectancy (SLE)

monetary loss or impact of each occurrence of a threat

## Exposure factor

measure of magnitude of loss of an asset, used to calculate SLE

## Annualized rate of occurrence (ARO)

how many times expected to occur annually

## Annualized loss expectancy (ALE)

how much an event is expected to cost per year
