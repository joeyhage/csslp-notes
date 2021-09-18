# Defensive Coding Practices

## Declarative vs Programmatic (imperative) Security
- early design decision
- Declarative
  - define the what
  - Security is defined in the deployment, not the code itself
  - Managed by ops team, not dev team
  - more flexible security
- Imperative  
  - embedded into code 
  - less flexible/portable/reusable but allows for greater granularity
  
### Bootstrapping
- startup process when computer/program starts

### Cryptographic Agility
- allow for changes in crypto function (e.g. algorithm) without changing code
- also assists with international cryptography reqs
- early design decision
- **important to use secure sessions**

### Handling Configuration Parameters
- securing config files is an important design decision

## Memory Management
- shared responsibility between app and OS
- managed code applications (.NET, Java) handle memory management

### Type-safe Practice
- type safety is linked to memory safety: cannot access arbitrary locations of memory

### Locality
- when a program references memory, other references are generally predictable and in close proximity
- several memory attacks take advantage of locality

## Error Handling

### Exception Management
- if left to the OS to handle, privilege escalation and other issues can occur

## Interface Coding
- need appropriate AuthN and AuthZ
- audit externally exposed, privileged operations

## Primary Mitigations
- standard best practice mitigations:
  - lock down env
  - establish/maintain control of inputs
  - establish/maintain controol of outputs 
  - assume external components can be undermined
  - assume code can be read by anyone
  - use libraries and frameworks that avoid introducing weaknesses
  - use industry-accepted security features
  - integrate security into the entire SDLC
  - use mix of methods to find and prevent weaknesses

### Defensive Coding
Foundational:
- attack surface reduction
- understand common coding vulns
- implement standard mitigations

Other:
- code analysis
- code review
- versioning
- crypto agility
- memory mgmt
- exception handling
- interface coding
- managed code

Exam tips:
- controlling concurrency (access to shared objects/race conditions)
- tokenization for sensitive data

## Learning from Past Mistakes
- security team should regularly update security reqs while considering errors from other companies
