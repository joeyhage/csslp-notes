# Security Quality Assurance Testing
quality = fitness for use according to requirements

## Standards for Software Quality Assurance

### ISO 9216
- primary focuses: functionality, reliability, usability
- other: efficiency, maintainability, portability

### SSE-CMM
- **systems security engineering capability maturity model (aka ISO/IEC 21827)**
- de facto standard for evaluating security engineering capability in an org

### OSSTMM 
- **Open Source Security Testing Methodology Manual**
- peer-reviewed, scientific methodology
- five sections:
   1. data networks
   2. telecommunications
   3. wireless 
   4. human (e.g. social engineering, security awareness training)
   5. physical security 
- training classes exist
- methodology can assist in auditing

## Testing Methodology
**Test harness**: means of documenting software, tools, test data, expected output, and configurations
- break testing into test suites for reuse

## Functional Testing
- assess functionality as expected by end user

### Steps
1. Identify functions (reqs)
2. create test data 
3. determine expected output
4. execute tests corresponding to functional reqs
5. compare actual and expected

### Functional Testing Areas
- reliability
- logic
- performance
- scalability

### Unit Testing
- functional logic
- understandable code
- reasonable vuln control and mitigation
- **done early by dev team before dev phase is over**

### Integration/Systems Testing
- includes secure and proper data transfer between components in a system

### Performance Testing
- **load testing**: performance under normal conditions
- **stress testing**: performance under overload conditions
- **Recoverability**: app's ability to restore itself to expected functionality after security is breached/bypassed

### Regression Testing

## Security Testing

### White-Box testing
- full knowledge of code and components
- done early in dev cycle
- focus on structure of software and use/misuse
- high false positives

### Black-Box testing
- common for system-level tests and pen testing
- focus on behavior of app
- high false positives

### Grey-Box Testing
- not total access to source code but understanding of inner workings
- rare outside of internal testing

## Environment
- interoperability of all components including:
   - credentials
   - permissions
   - access tokens
   - data movement across trust boundaries
   - etc

## Bug Tracking
- four types (same as options associated with risk):
   - removal of defect
   - mitigation
   - transfer of responsibility
   - ignore
- track bugs so they eventually get addressed
- logging bugs also provides metric of code quality
- defect categories:
   - bugs (coding errors)
   - flaws (design error)
   - behavioral anomalies (how app operates)
   - errors/faults (outcome-based from other sources)
   - vulns (things that can be manipulated to misuse system)

### Defects
- create defect database to track past and present issues
- help understand what not to do/what not to repeat
- provide testers with suggestions when looking for defects

### Bug Bar 
- set minimum level of quality for security at beginning of project

## Attack Surface Validation
- document actual attack surface through SDLC

## Test Data Lifecyle Management
- anonymization of production data is very challenging and requires planning
