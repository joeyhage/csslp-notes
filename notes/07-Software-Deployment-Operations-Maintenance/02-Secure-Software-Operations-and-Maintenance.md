# Secure Software Operations and Maintenance

- **Sustainment**: post-coding operations and maintenance
- ISO 12207:2017 (software lifecycle processes) includes five processes
  - two of the five are operations and maintenance
  - better to combine operations and maintenance into one process

## Secure Software Operations

- operate software in intended environment
- one of the most expensive items in budget of an IT org

### Operations Process Implementation

1. monitor and assure effective everyday use
2. document and track problem reports and requests for change

#### Connecting operation to change

- operations reports issues or requests for change to the configuration management team and product stakeholders

#### Planning for secure operation

- secure sustainment of a product within a particular environment

#### Operational monitoring and control

- operations function is responsible for routine testing
- developer may need to operate new product concurrently with previous version for a specified period to ensure it conforms to requirements

#### Customer support

- operations provides advice and product support to customers as needed
  - can also include scheduled training
- each request and actions taken should be recorded as part of config mgmt process

#### Ensuring service operation

- demonstrate compliance with defined criteria/SLA
- should identify and monitor potential risks in performance

## Software Maintenance Process

- provide cost-effective modifications and support for all software in org's portfolio
- ad hoc services for org's stakeholders

📝 study security aspects of all maintenance activities

### Monitoring

- monitor system within target environment
- respond to incidents
- maintain trust among stakeholders that system is secure and operating correctly
- need to prioritize review of systems since it may be impossible to monitor everything completely
- professionals on review team should have a sustainment focus while also have technical aptitude to participate in design/code reviews
- also need to interpret existing test results to ensure they adhere to test plans
- software needs to expose alerts/logs in order to be monitored

### Incident management

- can be caused by anything from user errors to hacking/malicious activity
- reacting to unforeseen events add extra challenges because mitigation steps have not been planned in advance

#### Monitoring and incident identification

- initiated when a _potentially_ harmful event occurs
- purpose of incident identification: distinguish between vulnerability in code, exploit of software, and user error
- purpose of incident monitoring: identify as quickly as possible
  - can include tests, reviews, audits of logs, automated incident mgmt systems, dynamic testing tools, code scanners

#### Incident reporting and management control

- report incident type and assessed impact to incident manager
- routine code defects should be reported as well as intentional things like trapdoors
- incident response team: trained specialists (like fire dept) that follow a process to ensure the best possible response
  - also limit additional damage and study circumstances to prevent future occurrence

#### Anticipating potential incidents

- incidents are either potential or active
- Potential incidents: defects that don't appear to have a present threat, unforeseen flaws, security vulnerabilities in OS/vendor software (e.g. Microsoft)

#### Responding to active incidents

- incident response team handles and supervises patch/change to target system

#### Establishing a structured response

- essential to develop procedures for precise steps to be taken for passive and active incidents
- include who is authorized to initiate incident response and how much authority is required to direct a response

#### Ensure enough resources

- deploy appropriate response and not overreact
  - start with a subset of resources and then decide if it needs to be escalated

#### Managing the incident response team

- team should include:
  - experienced team manager
  - expert software analysts/programmers
  - cybersecurity and computer crime specialists
  - sometimes, legal/government/public affairs experts

### Problem management

- Type: corrective, improvement, preventative, adaptive action that might be required
- Scope: modification size, cost, time 
- Criticality: impact of change on performance, safety, security of org

### Change management

- primary purpose: protect enterprise from risk associated with changing functioning systems

#### Patching

- can be labeled as patches, hot-fixes, quick fix engineering (QFE)
- what does patch repair and is it necessary to do so in prod?
- patches are often bundled together in service packs or included in release schedule

### Backup, recovery, archiving

- important to backup software and data so it can be restored
- use encryption to protect backups
- retention cycle: complete set of backups needed to restore data
  - needs to be stored within retention period

## Secure DevOps

- frequent, smaller changes are faster to implement, faster to test, faster to correct
- high level of automation

## Secure Software Disposal
