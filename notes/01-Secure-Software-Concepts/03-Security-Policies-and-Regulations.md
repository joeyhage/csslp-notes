# Security Policies and Regulations

- **All hazards**: senior management is responsible for security, compliance, all exercises in risk management

## FISMA

- **Federal Information Security Management Act of 2002**
- 📝 Primary governing law for federal computer systems

- Requires each federal agency to implement a security program
- NIST (National Institute of Standards and Technology) developed guidelines
- Risk Management Framework (RMF) was published by NIST
  - Initial framework included:
    - Inventory of systems
    - Categorize information and systems according to risk level
    - security controls
    - Certification/accreditation of systems (risk assessment and security plans)
    - Training
- Information Security Automation Program
- Security Content Automation Protocol (SCAP)

NIST six steps for a RMF:

1. Categorize systems
2. Select security controls
3. Implement controls
4. Assess Controls
5. Authorize information systems
6. Monitor controls

## Sarbanes-Oxley (2002)

- financial accounting information systems must have control over integrity

## Gramm-Leach-Bliley Act / Financial Modernization Act of 1999 (GLBA)

- Protect PFI (personal financial information)
  - act specifies rules for collection, processing, storage, and disposal of PFI

Primary rules:

1. Financial Privacy Rule - collection and disclosure of PFI
2. Safeguards Rule - applies to financial institutions - covers design, implementation, and maintenance of safeguards to protect PFI
3. Pretexting Protections Rule - address pretexting (falsely pretending) to obtain PFI

## HIPAA and HITECH

- HIPAA - (Healthcare Insurance Portability and Accountability Act)
  - Protect PHI (personal health information)
- HITECH - (Health Information Technology for Economic and Clinical Health Act)
  - enhance privacy of electronic PHI records

## Payment Card Industry (PCI)

Industry group established to secure cardholder data

### Data Security Standard (PCI DSS)

Industry group members that accept and process bank cards are required to protect cardholder data

### Payment Application Data Security Standard (PA DSS)

Standard to validated that a payment application is compliant with PCI DSS

### PIN Transaction Security (PTS)

Applies to PIN Entry Devices (PEDs)

## Legal Issues

### Intellectual Property

1. Patents
   1. Exclusive right for a specified time
   2. protect rights in exchange for disclosure of invention
   3. Varies by country but in the US, invention must be new, useful, and nonobvious
   4. Prevent others from using invention
   5. Patent must be applied for prior to disclosure
   6. challenging and expensive
2. Copyrights
   1. Protection of an idea or information for a specified time
   2. right to be credited, who may adapt, who may perform, who may financially benefit, etc
   3. governed internationally by Berne Convention
   4. straightforward and affordable
3. Trademarks
   1. recognizable quality of product/firm
   2. used to build brand association
   3. can be common-law or registered - registered provides more legal protection and recovery
   4. managed internationally through World Intellectual Property Organization
4. Trade Secrets
   1. best time-based protection
   2. protected by many laws as long as company makes a reasonable attempt to keep it secret
   3. if secret is independently discovered (e.g. recipe), then secret holder has no recourse
   4. US Digital Millenium Copyright Act prohibits reverse-engineering of security safeguards
5. Warranty
   1. hardware often has a warranty to perform at the specified level
   2. software does not and is generally sold as is

## Privacy

- To obtain certain goods, users must consent to share certain information
- One main issue with privacy is data disposition
- 📝 founded on notice, choice, and security

### Privacy Policy

Internal privacy policy details the firm's responsibilities to protect information

External privacy policy, or privacy disclosure statement, informs customers how data is protected, used, and disposed of

In financial sector, Gramm-Leach-Bliley Act mandates firms clearly state how information is shared

### PII

### PHI (Personal Health Information / Protected Health Information)

Highly valued by cybercriminals

### Breach notifications

- Incident response (what happened, how, what was lost)
- Most states have disclosure laws, no federal law

### Data Protection Principles

- data protection - European Union
- European Union Data Protection Directive (EUDPD) - old
- General Data Protection Regulation (GDPR)
- In US, consumers must opt-out

#### European Union Privacy Law

- consumers must opt-in
- three conditions must be met for processing personal data:
  - transparency: consent, including purpose and recipients
  - legitimate purpose
  - proportionality

#### Safe Harbor Principles

- Non-EU firms can meet EUDPD requirements by:
  - **Have been replaced, still helpful to understand**

1. **Notice**: inform customers of data collection and purpose
2. **Choice**: can opt out of collection and transfer of data
3. **Onward transfer**: third parties must follow principles
4. **Security**: Reasonable efforts to prevent loss of data
5. **Data integrity**: Relevant and reliable for purpose it was collected
6. **Access**: Customers can access data and correct/delete
7. **Enforcement**: Effective means for enforcing rules

### GDPR (2018)

Several major changes:

1. Personal Data elements are anything that can be linked back to a subject, including cookies
2. Individuals must have full access to how data is processed in a clear manner
   1. who is asking for the data
   2. what the data will be used for
   3. how long can it be kept
   4. if and where it will be transferred internationally
   5. right to access, correct, or erase
   6. right to withdraw consent, even after collection
   7. right to lodge a complaint

### California Consumer Privacy Act of 2018 (AB 375)

Similar to GDPR

individuals still must opt out but they have rights:

- right to know (access to data and how it's used)
- right to delete (some exceptions)
- right to opt out of sale of information
- right to non-discrimination if they don't want data sold

## Security Standards

### ISO (International Organization for Standardization)

- five year review cycle

Relevant area is under JTC 1 - Information Technology

- Subcommittee 7 (Software and Systems Engineering)
- Subcommittee 27 (IT Security Techniques)

Prominent ISO Standards for CSSLPs - **See page 64**

### ISO 2700X Series

For information security

Includes vocabulary, code of practice, implementation guidance, metrics, and risk management

### ISO 15408 Common Criteria / Evaluation Assurance Levels (EAL)

Functional and assurance requirements

Claims can be made about the product that can be evaluated and verified

- **TOE**: Target of Evaluation - product or system being evaluated
- **ST**: Security Target - security properties of a TOE
- **PP**: Protection profile - set of security requirements associated with a certain class of product
  - products in the same class can be compared more easily

higher EAL != better security

### ISO 9126 Software Engineering Product Quality

- four parts to define a quality model
- Quality of use metrics for specific scenarios
  - Functionality
  - Reliability
  - Usability
  - Efficiency
  - Maintainability
  - Portability

### ISO 12207 Systems and Software Engineering - Software Life Cycle Processes

- set of processes each having its own activities, tasks, and outcomes

### ISO 15504 Information Technology - Process Assessment

SPICE/SPICD - Software Process Improvement and Capability Determination

### NIST

National Institute of Standards and Technology

Computer security division

- Federal Information Security Management Act of 2002 (FISMA)

Information Technology Laboratory (ITL)

- Security bulletins 6x/yr
- Interagency/internal reports (NISTIRs): technical research

#### Federal Information Processing Standards (FIPS)

- mandatory reqs on fed agencies and specific contractors
- few but broad in authority and scope
- Since FISMA, all aspects are mandatory and waivers are not allowed

#### NIST SP 800 Series

- more commonly used by industry
- communicate results of research/guidelines assoc with securing systems
- incl. cryptographic protocols, security reqs, risk mgmt framework, governance, etc

#### Industry

- SAFECode
  - Industry-backed
  - increase comm. between firms on software assurance
  - share best practices that have been successful
  - **SAFECode Releases Software Security Guidance for Agile Practitioners**
  - valuable to large and small firms

## Secure Software Architecture

### Security Frameworks

#### COBIT - Control Objectives for Information and Related Technology

Published by ISACA (Information Systems Audit and Control Association)

- bridge gap between control reqs, tech issues, and business risks
- Latest is COBIT 2019 (book explains COBIT 5)

##### COBIT 5 Principles

1. Meeting stakeholder needs
2. covering the enterprise end to end
3. applying a single, integrated frmwrk
4. enableing a holistic apprch
5. separating governance from mgmt

#### COSO - Committee of Sponsoring Organizations of the Treadway Commition

- five private-sector orgs in response to Treadway Commisions report on fraudulent financial reporting
- Enterprise Risk mgmt integrated frmwrk to assess control systems
- five components/principles
  - control env
  - risk assmnt
  - cntrl activities
  - info and communication
  - monitoring

#### ITIL - Information Technology Infrastructure Library

- aligning IT services with bus. needs

##### Five volumes

1. ITIL Service Strategy
2. ITIL Service Design
3. ITIL Service Transition
4. ITIL Service Operation
5. ITIL Continual Service Improvement

#### Zachman

- matrix frmwrk to define an enterprise

#### SABSA - Sherwood Applied Business Security Architecture (SABSA)

- frmwrk and methodology for risk-driven enterprise infosec architectures
- similar to Zachman
- Goal: all reqs, including security reqs, can be derived from business reqs
- Works well with SDLC

#### SDLC

Using some kind of process-based lifecycle results in greater security

- partly due to models
- partly due to opportunities for process improvement on models

#### SEI CMMI (Software Engineering Institute - Capability Maturity Model Integration)

- rates process maturity on a 1-5 scale
- Three primary areas: product/service dvlpmnt, service establishment/mgmt, product/service acquisition
- **framework for business process improvement**: improving operational processes

##### Process Maturity Levels 📝

1. **Initial:** uncontrolled, results unpredictable
2. **Managed:** established, typically reactive
3. **Defined:** characterized for org, proactive
4. **Quantitatively Managed:** measured and controlled
5. **Optimizing:** process improvement

#### OWASP - already familiar with :)

#### OCTAVE - Operationally Critical Threat, Asset, and Vulnerability Evauluation

- tools, techniques, methods for risk-based infosec assmnt
- Three phases: build asset-based threat profiles, identify infra vulns, dvlp security stratgy

#### BSI - Build Security In

- US Dep of Homeland Security
- info on research, best practices, generic principles for software security
- collaborative effort for devs, architects, infosec practitioners to build security into SDLC

## Trusted Computing

- developed and promoted by trusted computing group (TCG)
- Has a trusted platform module (TPM) with encryption key that is only accessible through the TPM chip
- controversy: could the machine be secured from its owner?

### Principles

1. security
2. privacy
3. interoperability
4. portability of data
5. controllability
6. ease of use

#### Ring Model

- system method
- protect data/functionality from errors and malicious behavior
- ring can only interact within itself or with adjacent rings

#### Reference Monitor (reference validation mechanism)

- access control methodology
- mediates interaction between subjects/objects
- 📝 three qualities are req:
  - no path around it, always invoked (complete mediation)
  - tamper-proof
  - small enough to be verifiable

#### Protected Objects

- existence may be known, cannot be interacted with directly
- must use protected subsystem with specific procedures and a security policy

### Trusted Computing Base (TCB)

- combination of software/firmware/hardware to ensure security
- includes kernel and reference monitors, **not applications**
  - if application becomes compromised, it would not affect TCB

### Trusted Platform Module (TPM)

- secure storage of crypto. keys and platform auth - on a chip

### Microsoft Trustworthy Computing Initiative (2002)

Four pillars:

1. security (including social dimension)
2. privacy
3. reliability
4. business integrity

## Acquisition

Terms:

- Commercial off-the-shelf (COTS)
- Government off-the-shelf (GOTS)

### Build vs buy

- some things are best purchased (database software)
- mission-critical or proprietary business info is best built

### Outsourcing

- can find cheaper programmers/people but most of a project's cost is not from the coders
- has challenges due to geographic separation

### Contractual Terms and SLAs

- should include references to security cntrls/standards
