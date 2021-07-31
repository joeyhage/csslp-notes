# Design Processes

## Attack Surface Evaluation
- includes code, input fields, protocols, interfaces, files, and services
- higher attack surface != bad code, it's just a measure of how many things can be attacked
- turning off unused/unneeded features will minimize attack surface

### Attack Surface Management
- measure # of ways it can be accessed
- root cause of old/prev vulns can help fix them, prevent future, and determine attack surface
- elements are not necessarily vulns, but hackers will attempt to compromise
- cannot compare between software

### Attack Surface Minimization
- turning off unnecessary elements (off by default)
- only on when needed (certain users/times)
- least privilege
- document minimization throughout dev process
  - help lower defaults at deployment
  - allow customer to make decisions about options

## Threat Modeling
- **team effort**
- identify and document threats
- describe mitigations

### Threat Model Development

#### Identify Security Objectives
- security AND privacy
- business rationale for obtaining/storing data
- dev team should not decide if/how to protect data - won't have visibility/breadth to know all threats

#### System Decomposition
- model system design using security reqs/objectives (data flow diagram is best)
- include all processes, data stores, data flows
- call out trust boundaries (where privilege changes)
- for larger systems, break down DFD into scenario-based pieces
- list/describe assumptions and dependencies

#### Threat Identification
- use STRIDE to create threat model

Threat                 | Security Property
---------------------- | ----------------- 
Spoofing               | Authentication
Tampering              | Integrity
Repudiation            | Nonrepudiation
Information Disclosure | Confidentiality
Denial of Service      | Availability
Elevation of Privilege | Authorization

#### Mitigation Analysis
- Four types (in order of best to worst): 
   1. redesign to eliminate (generally early in SDL)
   2. apply standard mitigation (e.g. ACL)
   3. invent mitigation
   4. accept vuln
- attack tree model: help one understand threat
- also need to prioritize threats
- DREAD (damage potential, reproducibility, exploitability, affected users, discoverability) - 0 to 10
- can be mapped to probability impact model (reproducibility + exploitability + discoverability) and (damage potential + affected users)

#### Threat Model Validation
- validate threat model at each SDL gate
- do threats describe the attack and impact in detail relevant to app?
- are mitigations associated with a threat and described in detail relevant to app?
- dependencies
- security functions of deps
- assumptions documented

## Control Identification and Prioritization
- prioritize enterprise security controls - it is more efficient (eliminates duplicate efforts)
- use security of existing protocols (HTTPS, SSH)

## Risk Assessment for Code Reuse
- using old code/libraries should be scrutinized just like new code

## Documentation
- threat modeling and attack surface minimization docs can be very valuable if kept up to date

## Design and Architecture Technical Review
- is the SDL achieving the desired objectives?
