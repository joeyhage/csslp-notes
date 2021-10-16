# Exam Outline Review

## 1. Secure Software Concepts

### 1.1 Core Concepts

- **Confidentiality**
  - Covert channel: communication path that is intentionally hidden. Leaves almost no trace. Receiver has to be actively listening for message
  - Overt channel: communication path that is not hidden. Leaves evidence behind but receiver doesn't have to be listening for message
  - Side channel: unintentional communication. Think power consumption changes to get information about encryption used
- **Integrity**
  - Also includes stability and reliability for authorized subjects
- **Availability**
- **Authentication**
- **Authorization**
- **Accountability**
- **Nonrepudiation**

### 1.2 Security Design Principles

- **Least Privilege**
- **Separation of duties**
- **Defense in depth**
- **Resiliency**
  - fail safe, fail secure, no single point of failure
- **Economy of mechanism**
  - less complexity is better
  - eliminate nonessential services and protocols
- **Complete mediation**
  - authorization cannot by bypassed
  - authorization checked every time subject requests access to an object
- **Open design**
  - security of a system is independent of the design (don't rely on security by obscurity)
  - Kerckhoffs's principle: security of a cryptosystem is reliant on choice of keys, not algorithm
- **Least common mechanism**
  - isolation to protect against sharing of information
- **Psychological acceptability**
- **Component reuse**
- **Diversity of defense**
  - layers of defense should be diverse
- **Safeguard**
  - _Proactive_ controls to protect assets
  - controls can be physical, administrative, or technical
- **Countermeasure**
  - _Reactive_ controls to protect assets
  - controls can be physical, administrative, or technical

## 2. Secure Software Requirements

### 2.1 Define Software Security Requirements

- **Functional**
  - business requirements
  - use cases
  - user stories
- **Non-functional**
  - operational
  - deployment
  - systemic qualities

### 2.2 Identify and Analyze Compliance Requirements

- **FISMA**
  - an agency-wide information security program is required for federal agencies
- **Sarbanes-Oxley**
  - internal control measures for financial accounting
- **Gramm-Leach-Bliley**
  - protection of PFI (Personal Financial Information)
  - protects against falsely pretending to obtain PFI
- **HIPAA and HITECH**
- **Payment Card Industry Data Security Standard (PCI DSS)**

### 2.3 Identify and Analyze Data Classification Requirements

- **Data ownership**
- **Labeling**
  - sensitivity and impact
  - primarily driven by cost
- **Types of data**
  - structured, unstructured
  - categories: security sensitive, PII, hidden
- **Data life-cycle**
  - if persistent, data needs to be classified, labeled, assigned retention policy
  - retention policies include backups, DR sites, legal holds
  - legal hold data is excluded from normal disposal procedures

### 2.4 Identify and Analyze Privacy Requirements

- **Data anonymization**
- **User consent**
- **Disposition**
  - right to be forgotten
- **Data retention**
- **Cross borders**

### 2.5 Develop Misuse and Abuse Cases

- **Use cases**
  - helpful for clarifying complex/confusing/ambiguous situations
  - not intended for all subject-object relationships

### 2.6 Develop Security Requirement Traceability Matrix (STRM)

- document relationships between security requirements, controls, and test/verification efforts

### 2.7 Ensure Security Requirements Flow Down to Suppliers/Providers

## 3. Secure Software Architecture and Design

### 3.1 Perform Threat Modeling

- **Understand common threats**
- **Attack surface evaluation**
- **Threat intelligence**

### 3.2 Define the Security Architecture

- **Security control identification and prioritization**
- **Distributed computing**
- **Service-oriented architecture**
- **Rich internet applications**
- **Pervasive/ubiquitous computing**
  - IOT
  - RFID
  - NFC
- **Embedded**
  - Field-programmable gate array (FPGA) security features
- **Cloud architecture**
- **Mobile applications**
- **Hardware platform concerns**
- **Cognitive computing**
  - machine learning, AI
- **Control systems**

### 3.3 Performing Secure Interface Design

- **Security management interfaces, out-of-band management, log interfaces**
- **Upstream/downstream dependencies**
- **Protocol design choices**

### 3.4 Performing Architectural Risk Assessment

### 3.5 Model (Non-Functional) Security Properties and Constraints

### 3.6 Model and Classify Data

### 3.7 Evaluate and Select Reusable Secure Design

- **Credential management**
- **Flow control**
  - proxies, firewalls, protocols, queueing
- **Data loss prevention**
- **Virtualization**
- **Trusted computing**
- **Database security**
- **Programming language environment**
- **Operating system controls and services**
- **Secure backup and restoration planning**
- **Secure dat retention, retrieval, and destruction**

### 3.8 Perform Security Architecture and Design Review

### 3.9 Define Secure Operational Architecture

### 3.10 Use Secure Architecture and Design Principles, Patterns, and Tools

## 4. Secure Software Implementation

### 4.1 Adhere to Relevant Secure Coding Practices

- **Declarative vs imperative (programmatic) security**
- **Concurrency**
- **Output sanitization**
- **Error and exception handling**
- **Input validation**
- **Secure logging & auditing**
- **Session management**
- **Trusted/Untrusted APIs and libraries**
- **Type safety**
- **Resource management**
- **Secure configuration management**
- **Tokenizing**
- **Isolation**
- **Cryptography**
- **Access control**
- **Processor micro-architecture security extensions**

### 4.2 Analyze Code for Security Risks

- **Secure code reuse**
- **Vulnerability databases/lists**
- **Static application security testing**
- **Dynamic application security testing**
- **Manual code review**
- **Look for malicious code**
- **Interactive application security testing**

### 4.3 Implement Security Controls

### 4.4 Address Security Risks

- **Risk response**

### 4.5 Securely Reuse Third-Party Code or Libraries

### 4.6 Securely Integrate Components

- **Systems-of-systems integration**

### 4.7 Apply Security During the Build Process

- **Anti-tampering techniques**
- **Compiler switches**
- **Address compiler warnings**

## 5. Secure Software Testing

### 5.1 Develop Security Test Cases

- **Attack surface validation**
- **Penetration tests**
- **Fuzzing**
- **Scanning**
- **Simulation**
- **Failure**
  - break testing
  - fault injection: introducing faults to see how software behaves. Test error handling code paths
- **Cryptographic validation**
- **Regression tests**
- **Integration tests**
- **Continuous**
  - synthetic transactions: write code to mimic user behavior using a browser
  - real-user monitoring: collect data based on actual user data (e.g. Google Analytics)

### 5.2 Develop Security Testing Strategy and Plan

- **functional security testing**
- **nonfunctional security testing**
  - reliability
  - performance
  - scalability
- **testing techniques**
  - white box
  - black box
- **environment**
- **standards**
  - ISO
  - Open Source Security Testing Methodology Manual (OSSTMM)
  - Software Engineering Institute (SEI)
- **crowd sourcing**
  - bug bounty

### 5.3 Verify and Validate Documentation

### 5.4 Identify Undocumented Functionality

### 5.5 Analyze Security Implications of Test Results

### 5.6 Classify and Track Security Errors

- **Bug tracking**
- **Risk scoring**
  - CVSS

### 5.7 Secure Test Data

- **Generate test data**
- **Reuse of production data**

### 5.8 Perform verification and validation testing

## 6. Secure Software Lifecycle Management

### 6.1 Secure configuration and version control

### 6.2 Define strategy and roadmap

### 6.3 Manage security within a software development methodology

### 6.4 Identify security standards and frameworks

### 6.5 Define and develop security documentation

### 6.6 Develop security metrics

### 6.7 Decommision software

- **End of life policies**
- **Data disposition**

### 6.8 Report security status

### 6.9 Incorporate integrated risk management (IRM)

### 6.10 Promote security culture in software development

### 6.11 Implement continuous improvement

## 7. Secure Software Deployment, Operations, and Maintenance

### 7.1 Perform operational risk analysis

- **Deployment environment**
- **Personnel training**
- **Safety criticality**
- **System integration**

### 7.2 Release software securely

- **Secure continuous integration and continuous delivery pipeline**
- **Secure software tool chain**
- **Build artifact verification**

### 7.3

- **Credentials**
- **Secrets**
- **Keys/certificates**
- **Configurations**

### 7.4 Ensure secure installation

- **Bootstrapping**
- **Least privilege**
- **Environment hardening**
- **Secure activation**
- **Security policy implementation**
- **Secrets injection**

### 7.5 Perform post-deployment security testing

### 7.6 Obtain security approval to operate

### 7.7 Perform information security continuous monitoring (ISCM)

- **Collect and analyze observable data**
- **Threat intel**
- **Intrusion detection/response**
- **Secure configuration**
- **Regulation changes**

### 7.8 Support incident response

- **Root cause analysis**
- **Incident triage**
- **Forensics**

### 7.9 Perform patch management

### 7.10 Perform vulnerability management

### 7.11 Runtime protection

### 7.12 Support continuity of operations

- **Backup, archiving, retention**
- **Disaster recovery**
- **Resiliency**

### 7.13 Integrate service level objectives and service level agreements

## 8. Secure Software Supply Chain

### 8.1 Implement software supply chain risk management

- **Identify**
- **Assess**
- **Respond**
- **Monitor**

### 8.2 Analyze security of third-party software

### 8.3 Verify pedigree and provenance

- **Secure transfer**
- **System sharing/interconnections**
- **Code repository security**
- **Build environment security**
- **Cryptographically-hashed, digitally-signed components**
- **Right to audit**

### 8.4 Ensure supplier security requirements in teh acquisition process

### 8.5 Support contractual requirements
