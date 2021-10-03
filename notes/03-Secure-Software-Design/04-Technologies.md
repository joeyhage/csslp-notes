# Technologies

## Authentication and Identity Management

### Identity Management (IDM) and Identity and Access Management (IAM)

- policies, processes, technologies used to manage identity info
- provisioning, mgmt, and deprovisioning of identities
- a foundational element is protecting the secret yet making it usable
- **audited annually under SOX section 404**

### Authentication

- typically authentication system is the underlying operating system aspect, not a third party application
- integrates with AuthZ system once successful
- Federated ID systems allow connection to systems through known system (Facebook, Microsoft, etc)
  - Relying party (RP) and Identity Provider (IdP)

## Credential Management

- all activities should be logged

### X.509 Credentials

- manipulating certificates used to transfer asymmetric keys
- IETF PKIX (public key infrastructure X.509)

### Single Sign-On

- two most popular are Kerberos (LDAP domain) and SAML - OpenID is also a proven protocol for SSO
- primary objective of SSO is convenience

## Flow Control (Proxies, Firewalls, Middleware)

### Firewalls

- network level firewall (stateless) - think VPC/intranet
- next-generation firewalls (often stateful and look at multiple packets) - more granularity
- firewalls operate on a packet level
- can be stateless or stateful
- limited by network architecture (e.g. if numerous paths for traffic to flow, difficult or even impossible to place firewalls)

### Proxies

- security device like a firewall, but can also have a wide range of capabilities
- can include caching for performance
- can work at the protocol level (HTTP) whereas firewalls only know IP, TCP, UDP

### Application Firewalls

- firewall proxy
- PCI Data Security Standard req: web apps either need a WAF or code reviews
- most can work on ingress and egress traffic

### Queuing Technology

- synchronous or asynchronous
- guaranteed transport or best effort (TCP and UDP, respectively)

## Logging

- challenges: what to log, how to store
- must meet compliance criteria (HIPAA, SOX, PCI DSS, EOC)

### Syslog

- IETF approved protocol
- UNIX format for sending logs across network

## Data Loss Prevention

- protect against exfiltration of data
- look for specific traffic (size, destination, data elements, etc)
- attackers often use encryption to make it difficult to view what data is being stolen

## Virtualization

- reduced cost of servers by consolidating
- improved efficiencies from administrative ease
- portability and isolation
- operational agility (e.g. scaling in the cloud)

## Digital Rights Management

- technology used to protect intellectual property
- copy protection, usage rights, authenticity, integrity

### three entities in DRM

1. users
2. contents
3. rights

- DRM uses Rights Expression Language (REL) - XML, machine readable
- not perfect, still has issues balancing protection and usability

## Trusted Computing

- ensure computer behaves consistently as expected

### TCB (trusted computing base)

- focused mainly on privilege escalation
- each element should require authorization to receive an increase in privilege

### TPM (trusted platform module)

- hardware implementation of cryptographic functions on motherboard
- level of security deeper than OS and virtually tamper-proof
- controversy: could secure machine from owner or regulate permitted software

### Malware

- software with malicious intent
- can be designed so that it is not observable by the user and is virtually undetectable
- malware requires a vuln in a software system

### Code Signing

- digital signature
- verify author, integrity, etc
- mature technology

## Database Security

- capabilities include those below as well as
  - stored procedures - access to specific elements based on rules
  - backup and replication

### Encryption

- using DBMS functions or external tools
- primary keys cannot be obfuscated/encrypted - don't use PII/PHI as keys
- things to consider for encryption strategy
  - level of risk classification for data
  - usage pattern of data and protection in transit and use
  - risk classification for specific elements of data - does it differ?
  - how encryption is used across enterprise
  - what encryption options are available to dev team?
- members of dev team need to know which data elements have regulations around encryption

### Triggers

- trigger scripts based on database activity

### Views

- type of data structure to give different access based on subject

## Programming Language Environment

- language used for development is rarely what is used on the target computer (compilers, interpreters, or both affect this)

### Compilers

- faster execution

#### two sub-processes

1. **compiling**: convert source code into processor-specific codes
2. **linking**: connect libraries, dependency files, resources
   1. static linking: increased executable size, everything is copied into it
   2. dynamic linking: place names and locations of dependencies which are resolved at runtime
      1. creates risk for hijacked dependent programs

### Interpreters

- intermediary program to execute source code on target machine
- slower execution but fast change between revisions (no compiling/linking)
- converted into executable line by line at runtime

### Hybrid

- compiled into intermediary stage to be interpreted at runtime

#### CLR (.NET)

- application can be built with multiple languages and compiled with just-in-time compiler
- CLR adds garbage collection, type safety, index checking, sandboxing, more

#### JVM

- Java is compiled into byte code
- JRE contains JVM and standard libs

### Compiler Switches

- manage memory, stack protection, exception handling, etc
- security team should define compiler switch options for use in SDLC

### Sandboxing

- isolate code from direct contact with target system
- execute un-trusted code, code from guests, unverified programs
- operate like a VM
- protection depends on level of isolation and mediation

### Managed vs Un-managed code

#### Managed

- executed in a intermediate system that has controls (Java, .NET)

#### Un-managed

- executed directly on target
- compiled for specific system
- significant performance advantages but things like memory, type safety, garbage collection, need to be managed by developer
- un-managed is more prone to risks

## OS

- functional interface between applications and hardware
- real-time and embedded systems are simpler and leaner

## Embedded Systems

- hardware and software are coupled for a specific purpose
- PCs and servers are general purpose
- examples: watches, audio/video players, vehicles, etc

### Control Systems

- a type of embedded system for automated control of equipment
- many names - SCADA, Industrial Control Systems, Operational Technology

### Firmware

- software code held in a device
- wired in software so it is difficult to update or change
  - in many cases, is never updated or changed
- held in nonvolatile memory, read-only memory, erasable programmable read only memory, or flash memory
- firmware holds operational code base
- in computers, firmware is the first step in startup process (BIOS - basic input output system)
  - BIOS is the interface between OS and hardware
  - most computer makers replaced BIOS with more advanced version (UEFI - unified extensible firmware interface) around 2010
