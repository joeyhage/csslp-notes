# Risk Management
###### assess the impact if an adverse event were to happen decide what could be done to control that impact as deemed necessary

Well formed risk statement includes:
1. asset
2. threat
3. vulnerability
4. mitigation
5. impact
6. probability

## Risk
Systematic risk
- fire, theft, software bugs - mitigated through diversification
- predictable under stable circumstances
Unsystematic risk
- recession, epidemics, protocol design errors
- come from sources that are difficult to predict

### Business risk
- operation of a business as a business

Examples:
- Treasury management (financial risk)
  - holdings in bonds, futures, currencies, etc
- Revenue management
- Contract management
- Fraud
  - deliberate deception
- Regulatory 
- Business continuity
- Technology

### Technology risk
- technology used in development process as well as software functionality

Examples:
- Security - protective attributes
- Privacy - attributes that define access/sharing
- Project risk management
- Change management

### Risk controls
best method for managing risk

Understanding environment and applying controls should be owned by development team

Three classes:
1. Administrative
2. Technical
3. Physical


#### Preventative
- primary control
- proactive
- best mitigation
- **goal**: stop attack

Examples:
- separation of duties
- adequate documentation
- physical control over assets
- authorization mechanisms

#### Detective
- reactive
- **goal**: detect presence of attack

Examples:
- logs
- audits
- inventories

#### Corrective
- after a vulnerability is exploited
- **goal**: reduce total impact

#### Compensating
- when primary controls fail
- reactive
- defense in depth

Example: separation of duties is a preventitve control to prevent fraud, financial review of reports is an after the fact compensating control

#### Controls framework
- managing risk as part of a complete system

## Qualitative
###### Subjectively determine impact of an event - involves experts and group consensus 
Two aspects: impact and probability

### Qualitative matrix

### Failure mode effects analysis (FMEA)
- assess failures and effects on the system
- for each issue, elements are defined
- severity of risk is defined (1-10)
- probability (1-10)
- detectability (1-10)
- calculate product (over 200 / 1000 worth looking at)

## Quantitative
###### Objectively determine impact of an event - involves use of metrics and models
- use historical loss and trends to predict future loss
- highly dependent on historical loss data
- assuming constant risk rate is not an agreed upon concept

key info:
- important to come to consensus on values being used 
- use consistent values
- models can never replace judgement and experience, but can enhance decision making

### Single loss expectancy (SLE)
SLE = asset value * (exposure factor or duration)

### Annualized rate of occurrence (ARO)
ARO = number of events / number of years covered

### Annualized loss expectancy (ALE)
ALE = SLE * ARO

## Residual Risk Model
Absolute security is not achievable 
Example: 
- potential loss of $100k
- firewall blocks 95%
- IDS (intrustion detection system) is 80% effective
- IRT (incident response team) is 50% effective
- 100k * 95% + (5k * 80% * 50%) = 97k with 3k residual

### ROI
ROI % = (avoided loss - control cost) / control cost * 100
ROI time = avoided annual loss / annual control cost

## Governance, Risk, and Compliance
**Governance**: sum of exective actions that manage risk

need to comply with laws and regulations, so GRC terms are used synonomously

**Compliance**: activities associated with external requirements (contractual, policy, strategic, industry, regulations, laws)
**Conformance**: activities associated with internal requirements (org policies/standards)

Compliance gets priority over conformance 
- many reasons, primary being penalties

### Legal
Two key legal issues with significant risk
1. intellectual property
   - legal action provides some protection but not against unknown criminals
3. data breach

### Standards
- established norms
- **goal**: define rules to ensure specified level of quality

# Security Policies and Regulations

# Software Development Methodologies
