# 1. Security Policies

##### Policies must make general statement to pass the test of time
 - Data Life Cycle
	 - Data Retention Policies
	 - Data Disposal Policies
- Data Storage
- Acceptable Use Policy (AUP): appropiate way to use IT resource
- IR policies
- SDLC policies
##### Standards provide specific details of security controls => CIS Benchmarks
Meet specific technical requirements
- Password standard
- Access control standard
- Physical security standards
- Encryption standard

=> **Policies and standards are mandatory** (compliance)
##### Guidelines provide advice, follow best practices

=> **Guidelines are optional**
##### Procedures are a step-by-step documentation
- Change management procedures ([[Fundamental Security Concepts#^40756b|SOP]])
- Onboarding and offboarding procedures
- Playbooks (for IR team)

=> **Procedures can be optional or mandatory depending on organization and procedure**

![[image-1 1.png]]

Regular reviews identify inconsistency and gaps
Adapt policy documents as laws and regulations changes

>[!important] **Continuos monitoring**
# 2. Security Governance

Governance ensures that all parts of the organization align with its strategic goals
Shareholders elect a borad of directors to represent them
#### 2.1. [[2. Risk Management#^c2a1b9|Data Roles]]
#### 2.2. Security Governance Structures
Each person should be **independent** from the organization. The borad appoint a CEO.
CEO delegates security responsibility to a CISO
![[image-1.png]]

- **Centralized Government**: top-down approach in which a central authority creates policies and standards
- **Decentralized Government**: bottom-up approach in which individual business units are delegated the authprity to achieve cybersecurity objectives
# 3. Risk Analysis
#### 3.1. [[1. Risk Assesment|Risk Assessment]]
#### 3.2. Business Impact Analysis

##### see [[Incident Response and Recovery#^ea97b2|BIA]]
Cost-Benefit Analysis
#### 3.3. [[2. Risk Management#^b1580b|Risk Treatment Options]]

#### 3.4. Security metrics
##### Control Assessments
Test control effectiveness (both technical and operational)

##### Security Metrics
- **Key Performace Indicator (KPIs)**: demonstrate the success of the security program based on their objectives (evaluates the past)
- **Key Goals Indicator (KGIs)**: measure progress toward defined goals
- **Key Risk Indicatior (KRIs)**: quantify security risk facing an organization. Look forward. They quantify the risks that may jeopardize the organization

##### ITIL Security KPIs
9 clauses:
- Decrease in breaches
- Decrease in breach impact
- Increase in strong SLAs
- Number of new controls
- Time to implement controls
- Numbe rof major incidents
- Number of incident-related outages
- Number of training events
- Number of shortcoming

##### KRI Criteria
- Business impact
- Effort to implement, measure, and support
- Reliability
- Sensitivity

# 4. Supply Chain Risk

Ensure that vendor security polciies ar *at least* as stringetn as your own 
see [[3. Supply Chain Risk#^721ba4|Vendor Management Life Cycle]]
- [[Risk Management#^29d2e8|Service Level Requirement]]
e.g. Availability, data preservation
**Document SLRs in a service-level agreement (SLA)**

##### User Access Review
Validate rights and permissions