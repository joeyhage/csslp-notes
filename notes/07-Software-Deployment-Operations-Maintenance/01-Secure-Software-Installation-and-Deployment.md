# Secure Software Installation and Deployment

## Installation

- SDLC is broken into two phases: development and sustainment
- Sustainment includes: installation, deployment, operations, maintenance

### Installation V&V

- Use MITRE's Common Weakness Enumeration (CWE) to evaluate code

### Planning for Operational Use

#### Bootstrapping

- set of ops that properly launch function and ensure continuing correctness
- 📝 aka booting - e.g. PC power on self-test (POST)
  - integrity is mandatory
- implement error detection and correction

- 📝 version control: labeling software releases so end user knows what they are using

## Configuration Management

- 📝 exercise rational control over changes to software

### Organizing the Configuration Management Process

Three separate roles

1. **customer role**: maintenance of product after release
2. **supplier role**: managing configuration prior to release
   1. writes configuration management plan in conjunction with customer org
3. **subcontractor role**: if product developed through supply chain

### Configuration Management Plan

- should specify change management, baseline management, and verification management roles

### Configuration Management Process

- **purpose**: establish and maintain integrity of software items

- 📝 common way of tracking changes is through a configuration management database (CMDB)
  - also called configuration management system (CMS)
  - CMS is required for ISO/IEC 15408 (common criteria) accreditation

#### Process implementation

- create a fully documented plan for the entire lifecycle of the configuration management process

#### Configuration identification

- identify software items included in baselines
- create formal documentation with baseline version designations for each software item

#### Configuration control

- change management
- need authorization before changes are incorporated into baseline
- required for auditing

#### Configuration status accounting

- status and history for all controlled software items, including baselines

#### Configuration evaluation

- certify correctness of change after change is complete
- use statement of work (SOW) to verify

#### Release management and delivery

Product Baseline Repositories:

1. Controlled: current baseline, strictly controlled
2. Dynamic: un-trusted baselines being developed by programmers
3. Archive: past baselines, collective memory of the IT function
