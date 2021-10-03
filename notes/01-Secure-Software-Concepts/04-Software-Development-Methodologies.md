# Software Development Methodologies

## Secure Development Lifecycle (SDL)

- add process checks to development process to include necessary security elements

### Principles

- SMART - Specific, Measurable, Attainable, Realistic, Time bound

### Security vs Quality

- quality = fitness for use or absence of defects
- high quality != secure but low quality with lots of defects will have security issues from basic mistakes

### Security Features != Secure Software

- encryption, authentication, and other security features can improve usability
- secure software development is different: ensure all elements of software operate securely
- adding security features may make software more marketable but secure software means it does what it was designed to do and only what it was designed to do

## Secure Development Lifecycle Components

### Software Team Awareness and Education

- Basic knowledge
  - all should have
- Advanced topics
  - only certain people need

### Gates and Security Reqs

- eventually, if conducted in a firm and uniform manner, security is included as part of the normal business process

### Bug tracking

- sometimes, bugs can be exploited and result in a potential security bug
- 📝 DREAD (1-10 scale)
  - Risk = Impact \* Probability
    - Impact = Damage (in terms of CIA) and Affected Users (quantity)
    - Probability = Reproducibility (difficulty/scriptable?), Exploitability (attack difficulty), discoverability (difficulty to find)
  - detailed scoring is subjective and unreliable due to context/point of view
- better to use a defined set of severities (critical, important/high, moderate/medium, low)
- Bug bar - level at which a bug must be fixed in the current release
  - bugs are fixed based on risk, not ease of closure

### Threat modeling

- basically an ARA
- best performed during design phase
- focused on how data moves through app
- Threat model needs to include: app as a whole, security/privacy features, features that have security/privacy implications when they fail, features that cross trust boundaries
- 📝 STRIDE (spoofing, tampering, repudiation, info disclosure, DoS, elevation of privilege)
- Threat trees - graphical representation of what needs to exist for a threat to be realized (uses logical AND/OR)

### Fuzzing

- random input
  - scan for buffer overflows, system crashes, etc
- structured input
  - scan for injection vulns, XSS, input specific (arithmetic overflow, XXE, etc)
- mutation
  - use sample data
- input generation
  - based on models of system

### Security Reviews

- audit process to verify functioning as desired
  - use at key places (between stages in SDL)
- purpose: **NOT to test for security**, but to ensure steps are being done properly

### Mitigations

Standard Techniques:

1. Do nothing
2. Warn user
3. Remove problem
4. Fix problem

## Software Development Models

### Waterfall

- based on manufacturing design - each step completed before next step
- linear, sequential, no repeating
- useful for small pieces (incorporated into spiral/agile methods)
- non-workable in practice

### Spiral

- iterative, steps can be repeated iteratively
- things are built incrementally
- suited for large projects (may have several interconnected spirals)
- smaller-scale version can be seen in some agile methods

### Prototype

- based on manufacturing
- throwaway - gain information on subset
- evolutionary - build system through testing and adding features through accretion
  - vertical prototype - add more functionality (add back-end/database to front-end)
  - horizontal prototype - framework/infrastructure - adds features to one layer (build out entire front-end)
    - commonly used for software because it is modular
- limits resources to test major elements and reduce risk
- can be used in spiral/agile

## Microsoft Security Development Lifecycle

- Goal: produce software that is secure, not software that performs security or has specific security features
  - Reduce # of security vulns
  - reduce severity of security vulns that remain
- 2004 SD3+C
  - Secure by Design
  - Secure by Default
  - Secure in Deployment
  - Communications

### Secure by Design

- review detailed designs
- develop mitigations for all identified threats
- consider legacy code and protocols
- deprecate elements that are no longer secure

#### Privacy by design

- end-user control: enable end-user to make informed decisions about data collected, stored, shared
- only collect and retain required info
- use encryption to mitigate data loss issues
  - modular fashion in case it needs to be changed
  - proper crypto libraries/functions
  - proper key protection/rotation

### By Default

- default config is as secure as possible
- default config with privacy in mind
- limit features turned on by default
  - if less than 80% will use, turn off by default
- software should only operate with elevated rights when required
- minimize attack surface by default
- notify user if default config changes
- limit services/daemons running by default

### In Deployment

- one of last major touchpoints where config/settings are routinely modified
- develop prescriptive deployment guides
  - How
  - Implications
  - options available to user
- patching/upgrades should be built into deployment and give users control

### Communications

- efficient channels between security response and dev teams
- channel where dev team is connected to info sources like end-user issues/reports
- communicate security changes to end-users
- media/trade outlets to customers/prospective customers
- White papers/technical documentation can improve effectiveness of security effort by reducing concerns/issues from customers (transparency)
  - Open communication = increased cooperative/coordinated efforts
  - Open communication != increased risk

## Microsoft SDL Components

- started in 2002

### Training

- targeted security training for all
- training hour requirements
- includes:
  - core training - prereq, basic knowledge
  - specialized modules for specific roles
  - new developments/practices in industry
    - may become part of core if becomes mainstream

### Requirements

- establish security and privacy reqs for software
- create quality gates and bug bars
- develop security/privacy risk assessments

### Design

- risk and privacy analyses
- mitigated by design
- attack surface reduction techniques
- threat modeling for known and potential threats

### Implementation

- approved languages, functions, libraries
- remove deprecated functions
- recode legacy code
- static program checkers to maintain code standards

### Verification

- known and potential vulns
- review attack surface: does it match design
- fuzz testing against inputs

### Release

- prepare for potential issues coming in
- prepare incident response plan
- confirm all security elements completed and documented

### Response

- collect error reports and handle per incident response plan
  - current release bug fixes through patches
  - future releases: mitigation
