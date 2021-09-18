# Secure Lifecycle Management

## Introduction to Acceptance

### Software Qualification (Acceptance) Testing
- customer determines if software meets acceptance criteria
- assess contract, standard, and legal reqs under both normal and abnormal conditions

### Qualification Testing Plan
- scope, approach, resources, schedule
- design and execution of tests is normally defined in the contract
- **goal**: smallest # of test cases to sufficiently affirm quality and security of product
- seven things:
  - required features to test
  - requisite load limits
  - number/types of stress tests
  - risk mitigation and security tests
  - required performance levels
  - interfaces to be tested
  - test cases to address:
     1. who generates test designs/cases/procedures?
     2. who executes the tests?
     3. who builds/maintains test bed?
     4. who manages config?
     5. what are criteria for stopping testing?
     6. what are criteria for restarting testing?
     7. when will code be under change control/freeze?
     8. which tests will be under config mgmt?
     9. what level will anomaly reports be written for?

### Qualification Testing Hierarchy
- activities at acceptance level:
  - design traceability anlsys
  - design evaluation
  - design interface anlsys
  - test plan generation
  - test design generation
- evaluate documentation of each unit

## Pre-release Activities
- total product assurance is not necessarily achievable due to complex and dynamic nature of software

### Implementing Pre-release testing process
- software test plan describes objectives, scope, approach, and focus 
- helps people outside testing group understand why and how
- detailed enough to be useful but not so much that those outside group cannot understand

### Completion Criteria
- progress milestones are used as evidence of readiness for delivery
- tangible outcome or action
- criteria can be decomposed into metrics
- ISO 9126
  - functionality
  - reliability
  - usability
  - efficiency
  - maintainability
  - portability

### Risk Acceptance
- properties to consider to stay secure within acceptable limits:
  - implicit/explicit safety reqs
  - implicit/explicit security reqs
  - degree of complexity
  - performance factors
  - reliability factors
- evaluation process should answer two questions
   1. what is level of certainty of risk (likelihood)? 
   2. what is anticipated impact (loss)?
- risk assessment requires detailed knowledge of risks and consequences of software. Included in threat model which is created as part of SDLC
- **threat picture/situational assessment:** targeted risk assessments that only apply to known vulns at a specific time

## Post-release Activities
- typically not done by dev team
- best described as config mgmt
- first, perform complete audit of installed config

### Validation and Verification
- also apply to all stages of software lifecycle
- activities are documented in the software validation and verification plan (SVVP)
- **validation**: are we building the correct product? (i.e. meets user reqs)
- **verification** are we building the product correctly? (i.e. proper software construction)
- the SVVP should specify administrative reqs for:
  - anomaly resolution and reporting
  - exception/deviation policy
  - baseline and config control procs
  - standards practices and conventions adopted for guidance
  - form of relevant docs, including plans, procs, cases, and results

#### Management V&V
- examine plans, schedules, reqs, methods for assessing suitability
- supports decisions about corrective actions, allocation of resources, and project scoping
- support mgmt personnel who are responsible for system
- discover and report variations from plans/procs
- may involve the following mgmt roles:
  - decision maker
  - review leader
  - review recorder
  - mgmt staff
  - tech staff
  - customer/user rep

#### Technical V&V
- eval product, reqs/design docs, code/test/user docs/manuals/release notes, build/install procs
- does product conform to specs? adhere to regs, standards, and plans? correctly implemented/changed?
- support customer's/supplier's technical/mgmt personnel
- discover/report defects and anomalies
- may involve following mgmt roles:
  - decision maker
  - review leader
  - review recorder
  - tech staff/tech managers
  - customer/user tech staff
- should be scheduled as part of initial project planning
- ad hoc reviews may also be scheduled

### Independent Testing
- carried out by disinterested third party so customer and supplier trust integrity
- often called IV&V (audit)
- ensure customer/supplier have no influence over findings of testers
- items that may be audited:
  - plans
  - contracts
  - complaints
  - procs
  - reports/docs
  - source code
  - deliverables
- conducted by single person (lead auditor)
- audit usually not initiated by producer
- closing meeting report includes:
  - prelim conclusions
  - problems
  - recommendations for remediation
- once closing report is accepted, final report itemizes:
  - purpose and scope
  - name of audited org
  - software audited
  - applicable regs/standards
  - audit eval criteria
  - observation list classifying anomalies as major/minor
  - timing of audit follow-up activities

