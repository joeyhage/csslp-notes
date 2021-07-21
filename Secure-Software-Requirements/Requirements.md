# Requirements

## Functional Requirements
- business reqs
- IT reqs (e.g. database, environment, DR/BCP)
- org reqs (e.g. coding standards, maintainability)
- security reqs 

### Role and User Definitions
- which user groups are allowed access, and to what functionality
- part of the use-case definition
- users = subjects

### Objects
- ensures members of dev team can use common set of objects and control appropriately

### Activities/Actions
- Each object in a system should have all possible activities/actions defined + documented

### Subject-Object-Activity Matrix
- to help establish relationships
- creates list of allowable actions and another list of denied actions

### Use cases
- a specific example of an intended behavior of the system, usually for complex/confusing/amiguous situations
- not intended for all subject-object interactions
- not a substitute for documenting specific reqs
- graphical format that shows intended behavior (ellipses) for actors (stick figures)

### Abuse cases (inside and outside adversaries)
- form of use case but for the specifically prohibited

#### SAFECode
- development and distribution use cases - free, published PDF

### Sequencing and Timing
- race conditions, infinite loops
- Means system is vulnerable to a Time of Check/Time of Use (TOC/TOU) attack
- To avoid race conditions, first identify race window and then design so processes are not called concurrently (mutual exclusion)
- caused by complex conditional logic with unhandled situations - all conditions in a nested loop should be handled in a positive fashion

### Secure Coding Standards
- Secure SDLC includes controlling processes and making repeatable
- Adopt secure development frameworks as part of SDLC
- each function should practice complete error mitigation
- logging standards for what, where, when
