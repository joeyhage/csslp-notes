## Security Design Principles 

Must be designed into information systems, not done at the end of the project. 
This includes applications, networks, host, and databases

## Controls 
Allow implementation of security principles 

### Controls are:  
- Designed 
- Developed 
- Implemented 
- Configured 
- Operated 
- Monitored 
- Improved 

### Justification for Controls – Risk 
Likelihood of a threat exploiting a vulnerability and causing damage to an asset 
Level of risk drives level of control 

### Types of Controls 
1. Administrative 
2. Technical/Logical 
3. Physical/Environmental/Operational 

### Control Resistance 
A control can be considered a limitation, a hindrance, and a cost to the business 

## Integrating Security 
Dev teams need to be conscious of security at all phases of SDLC (define, design, develop, deploy) 

## Confidentiality 
###### Protect sensitive data from improper disclosure, whether intentional or accidental 
- Privacy usually relates to an individual 
- Secrecy usually relates to government or organization 

### Overt vs covert channels 
- Overt – obvious 
- Covert – hidden 
  - Unauthorized release of information through a hidden channel 
- Timing 
- Storage 

### Preservation of confidentiality 
- Masking (e.g. credit card, SSN) 
- Obfuscate 
- Tokenization (replace sensitive info with another value) 
- Encryption 

## Integrity 
###### Protection of data and processes from accidental or intentional modification 
- Accuracy 
- Completeness 
- Precision (e.g. round up, round down, truncate) 
- Reliability 

### Within applications 
- Edit checks – format, range, value limits, access levels (read-only)

### Integrity Implementations 
Message -> Hash function -> Hash/Digest 

### Hashing 
- MD5 
- SHA 1, SHA 256, SHA 384, SHA 512 
- Keccak (SHA3) 
- Haval 

### Encrypting Hash  
- HMAC (keyed hashing) 
  - Take hash/digest and use shared secret key in a symmetric encryption algorithm 
- Digital Signatures 
  - Use sender's private key to encrypt (asymmetric algorithm) 

### Authenticity 
e.g. Downloads, patches, source, APIs, drivers and utilities 

## Availability 
###### Ensure systems, information, networks, personnel, and software are available when required 

### Depends on the criticality of the resource 
- Fault tolerance (e.g. redundancy) 
- Failover 
- Backups 
 
### Within applications 
- Resilience – withstand attacks they will face 
- Error handling 
- Scalability 
  - Number of users 
  - Transaction volume 

### Reliable supporting infrastructure 
- Storage 
- Memory 
- Operating environment 
  - HVAC 
  - Dust 
  - Liquids 

### Distributed computing 
- Multiple operating locations 
- Disaster recovery planning 

### Replication 
- Hardware - isolation and cooperation (e.g. clustering) 
- Software (backups, OS) 
- Data (RAID, database shadowing) 


###### https://app.pluralsight.com/course-player?clipId=c580f473-0940-4297-bf41-c814397c9d5a
