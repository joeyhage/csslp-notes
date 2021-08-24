# Common Software Vulnerabilities and Countermeasures

## CWE (Common Weakness Enumerations)/SANS Top 25 Vuln Categories
- hasn't been updated since 2011 but still relevant

## OWASP Vuln Categories
- dedicated to web applications

### Common Vulns and Countermeasures

#### Injection Attacks
- SQL Injection
  - safest method is stored procedure
- OS Command Injection
- Integer overflow/wraparound
- path traversal
- XSS
- CSRF
- LDAP 
- XML

#### Cryptography
- pay attention to algorithms and key length

#### Input Validation
- **buffer overflow**
  - estimated that nearly half of historical exploits stem from buffer overflow


## Embedded Systems
- generally targeted for information disclosure or DoS 

## Side Channel Attack
- comes from cryptographic world - attack against implementation, not algorithm
- **use byproduct of a system**

Types:
- timing attacks and power attacks
  - analyze power/time used to make determination about what is happening
- data remanence attacks
  - cooling RAM to access data after power turned off
- electromagnetic attacks/acoustic attacks
  - reproduce what is on the screen or was typed on a keyboard

