# Data Classification and Categorization

## Data Classification
types of classification:
- state
- use
- importance

**classification is for risk management** - reduce costs associated with protecting data
- match level of protection and cost with value of asset

### Data States
- at rest
- being created
- in transit
- being changed/deleted

data storage location should be considered as well

### Data usage
- determining how it is used can help determine how it should be shared (or not)

Usage classifications
- **Internal** - created, computed, stored (in memory) within application
- **Input** - read into system and possibly stored
- **Output** - written to output destination

Sensitivity categories
- **Security-sensitive** - subset of data, very valuable to attacker
- **PII**
- **Hidden** - concealed using obfuscation to protect from unauthorized disclosure

### Data Risk Impact
labeled according to risk if lost (high, medium, low)
- will differ from firm to firm

impact considerations include cost, operation impact, and people impact

## Data ownership
- data is not owned by a person, it is owned by the enterprise
- data is assigned to people for stewardship/ownership for practical reasons
- **ownership is business driven**

### Owner
- acts in the interests of the enterprise
- determines who has what access
- owner != custodian (e.g. CFO owns accounting records but DBA can make direct changes)
- owner defines classification, authorization, and security controls

### Custodian
- ensure processes safely transport, manipulate, and store data
- ensure data management processes (set by owner) are followed
- perform backups, data retention, disposal
- manage anything else (e.g. security controls) defined by owner
- custodians may not need read access

## Labeling

### Sensitivity
- built around business purpose

### Impact
- wider concern than sensitivity
- includes loss, disclosure, and alteration
- three levels (high, medium or moderate, low) - each level should be clearly defined
- NIST FIPS 199 and SP 800-18 provide framework for classifying based on CIA

#### Clearly Definining levels
- high: set high enough that a small number of data elements are included
- financial limits and customer impact vary, each company needs to decide for itself
-  
