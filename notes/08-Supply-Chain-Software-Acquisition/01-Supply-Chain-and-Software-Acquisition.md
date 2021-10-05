# Supply Chain and Software Acquisition

- avg four levels in supply chain

## Supplier risk assessment

- **purpose**: identify and maintain appropriate set of risk controls within supply chain
- 📝 **contents**: specific threats to org's supply chain, likelihood of occurrence, impact if realized

### Supply chain threat categories

1. installation of malicious logic in hardware/software
2. installation of counterfeit hardware/software
3. failure/disruption in production/distribution of critical product/service
4. reliance on malicious/unqualified service provider for technical service
5. installation of unintentional vulns in software/hardware

### Risk assessment for code reuse

- reuse is more cost effective and ensures higher quality
- however, failures have a bigger footprint (leveraging existing components)
- define when reuse is safe and legitimate

#### Creating a practical reuse plan

- terms of use and negotiated liability for loss/damage should be stated in contracts
- **Strategic planning activity**
  - part of risk mgmt plan
  - define types of reuse and plans for reuse
  - will reuse include open-source or other code/products/services?

### Intellectual property

- true value of IP is abstract - strictly in the eye of the beholder
- difficult for legal system to assign value to creativity and beyond material investment/time spent

#### Copyrights

- gives creator right to determine who can use and conditions for use
- can apply to source code
- time limited
- **Regulations**
  - Computer Software Rental Amendments Act of 1990: rental, lease, lending without authorization is forbidden
  - Copyright Law: distribution of copies w/o authorization is illegal

#### Patents

- novel inventions
- not a secret
- time limited

#### Trademarks

- protect image, phrase, name, branding
- doesn't usually apply to code, but to program names/elements

#### Trade secrets

- difficult to employ because code can be reverse engineered

#### Licensing

- used to protect IP
- agreement between owner (licensor) and user (licensee) for payment (fee/royalty)

#### Code escrow

- form of protection for the customer
- copy of code is given to a neutral third party (escrow agent)
- access to code is only given under specific circumstances (business failure of supplier, termination of product line)

### Legal Compliance

- failure to comply can result in legal, financial, reputational, criminal consequences
- issue is not ensuring controls exist but rather supplying objective evidence of compliance to legal/regulatory entities

### Supplier prequalification

- product assurance
- suppliers need to prove they are capable of developing/integrating a secure product
  - what is the supplier's history with similar projects?
  - what is their documented ability to adopt good software engineering practices?
  - do they employ trustworthy subcontractors?

#### Assuring a black box: COTS

- need mutually agreed upon approach between customer/supplier to determine which vendors can be trusted in a supply chain
- customer needs to determine precise form of each supplier's dev process
- which trusted third-party should provide the prequalification?

#### ISO 15408: The Common Criteria

- National Information Assurance Program (NIAP) in the US is a third-party registry system
  - built around common criteria

##### Benefits

1. acquisition community has objective, independent assurance of trust
2. supplier can gauge own capability and improve

## Supplier Sourcing

## Software Development and Testing

## Software Delivery, Operations, and Maintenance

## Supplier Transitioning
