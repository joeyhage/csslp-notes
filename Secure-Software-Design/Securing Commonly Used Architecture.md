# Securing Commonly Used Architecture

## Distributed Computing
- affordable, smaller, powerful computing solutions led to more distributed computing architecture

### Client Server
- server: processing and storage for numerous users
- client (thin or thick/fat): single user, fat clients do most of processing themselves
- multiple machines for processing increases need for security
- "n-tier" model (n = # of application levels doing work)
  - user level, presentation level, business level, data access level, database level
- cloud computing is an extreme case of client server. n-tier model can be implemented in different cloud models (SaaS, PaaS, IaaS)

### Peer-to-peer
- file sharing and communication based systems

### Message Queuing
- helps manage throughput and guarantee delivery
- can also help with logging, security, and poiint to multipoint

## Service-Oriented Architecture (SOA)
- distributed with specific characteristics
  - platform neutrality
  - interoperability
  - modularity and reusability
  - abstracted business functionality
  - contract-based interfaces
  - discoverability
- several technologies like WS
- most SOA uses XML
- SOAP and REST and two common protocols for messaging in the ESB (enterprise service bus)

### Enterprise Service Bus
- monitors and controls message routing
- centralized architecture for communication between producers and consumers
- can translate/transform communications
- can convert between protocols (REST, JAVA, SOAP, etc)
- handle defined events
- perform message queuing and data flow mapping

### Web Services
- machine readable description of the interface - web services description language (WSDL)

#### REST
- stateless manner

#### JSON

#### Universal Description, Discovery, and Interace (UDDI)
- universal, platform-independent 
- dynamically discover and invoke web services
- XML, protocol based registry that services can list themselves on worldwide
- never widely adopted, generally only found inside orgs

## Rich Internet Applications (RIAs)
- application with characteristics of a desktop application delivered over the internet (Facebook, many websites today)

### Client-Side Exploits/Threats
- input validation
