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

- !! **input validation** !!

### Remote Code Execution

- consequence of architectural decision that there is no distinction between code and data

## Pervasive/Uniquitous Computing

- IOT - seldom have security capabilities
- each element/device of the system needs to be self-sufficient and self-reliant for security, safety, and stability

### Wireless

- developers need to take responsibility for security of transmitted data - not expect the network to be secure

### Location-Based

- A user's location can be abused
- not all sensitive data is easily identified as sensitive - need to consider how it could be abused

### Constant Connectivity

### Radio Frequency Identification (RFID)

- mostly used for contactless inventory
- range from few meters to hundreds of meters (active, battery powered transponders)
- radio frequency use has regulatory reqs (differs by country)

### Near-Field Communication (NFC)

- RF over very short distances (few inches)
- no setup for the user
- sometimes used to initiate/bootstrap higher bandwidth transfers

### Sensor Networks

- physical and environmental (rainfall, weather, communication efficiency, etc)
- individual elements are called nodes
- architecture depends on communication technology and objectives of network

## Mobile Applications

- built with consideration of native constraints of the device
- mobile apps can generally access a lot of information stored on the device

## Integration with Existing Architectures

- modern enterprise will never have one form of architecture
- cross-integration allows data reuse and increases utility of enterprise architecture

## Cloud Architectures

term is new, concept has been in use for decades

- on-demand self-service
- broad network access
- resource pooling
- rapid elasticity
- measured service

### Four cloud deployment models

1. Private cloud (one entity)
2. Public cloud
3. Community cloud (membership defined by shared concerns/use cases)
4. hybrid cloud (combination that remains separate but has common technology)

### SaaS

- need to plan for and consider vendor use/storage of client data

### PaaS

- can include SaaS and IaaS elements
- as scale increases, so does operational savings

### IaaS
