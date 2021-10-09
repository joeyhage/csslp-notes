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

### 3.8 Perform Security Architecture and Design Review

### 3.9 Define Secure Operational Architecture

### 3.10 Use Secure Architecture and Design Principles, Patterns, and Tools

## 4. Secure Software Implementation

## 5. Secure Software Testing

- ISO 9216
- SSE-CMM
- OSSTMM

## 6. Secure Software Lifecycle Management

## 7. Secure Software Deployment, Operations, and Maintenance

- maintenance activities

## 8. Secure Software Supply Chain
