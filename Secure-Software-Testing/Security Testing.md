# Security Testing

## Scanning
Passive in nature

Example: OS fingerprinting

### Attack Surface Analyzer
Microsoft tool to analyze how Windows is impacted when app is installed

## Pen Testing
- Active testing
- purpose: provide details to dev team so root cause can be fixed

Steps:
1. Recon (discovery, enumeration)
2. attack and exploitation
3. removal of evidence
4. reporting

### Fuzzing
- brute-force, large number of inputs
- network protocols, file protocols, web protocols
- most browser errors are found via fuzzing
- block-box, white-box, or grey-box
- tests input validation vulns (e.g. XSS, injection)
- both generation-based and mutation-based are used and have different advantages

## Simulation Testing
- test in a pre-prod env
- all aspects (config, firewall, OS, load/performance, etc)

## Testing for Failure
- most testing is testing for failure - also important to test for incorrect values

## Crypto Validation
- crypto random numbers are essential - best from crypto libraries

### FIPS 140-2
- Federal Information Processing Standards 
- selection of approved algorithms and implementation for federal gov

## Regression Testing
- more important as software gets older
- one of most time consuming parts of software patches
