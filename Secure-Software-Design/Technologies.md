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
- Federated ID systems allow connection to systems through known systesm (Facebook, Microsoft, etc)
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
