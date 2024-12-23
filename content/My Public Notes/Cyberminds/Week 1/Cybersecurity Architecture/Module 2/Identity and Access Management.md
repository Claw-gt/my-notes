[[Cyberminds Academy/Week 1/Introduction to Cybersecurity Tools & Cyber Attacks/Module 4/Authentication and Access Control/Identity and Access Management|Identity and Access Management]]

#### Store and Sync

- [x] **DataBases**
```mermaid
flowchart LR
	Identities --stored in -->Directory
```

- [x] **Schema**
Oragnization/Representation of user's data

- [x] **Protocol**
Way to talk to the Directory (**LDAP**)

---

In  the real world, the are several directories --> need to **SYNC**
##### SYNC option

--> **Virtual Directory**. One directory that acts as index
```mermaid
flowchart LR
	Directory --> Dir_1
	Directory --> Dir_2
	Directory --> Dir_3
```
--> **Meta-Directory**. Prefetch only relevant information
```mermaid
flowchart LR
	Dir_1 --> Directory
	Dir_2 --> Directory
	Dir_3 -->  Directory
```

### Administration

##### User cases
- New employee at HR
- Employee request more access rights
- Remove access right to recently ex-employee
- 
**Infrastructure:**

```mermaid
flowchart LR
	New_user --> HR_Dir
	HR_Dir --> REQ
	REQ --> ROLE
	ROLE --> ACCT_1
	ROLE --> ACCT_2
	ACCT_1 --> APPR
	ACCT_2 --> APPR
	APPR --> DB
```

### Authentication

```mermaid
flowchart LR
	WHO? --> Know
	WHO? --> Have
	WHO? --> Are
```
--> *MFA*
--> *Password-less authentication*
--> *SSO*

### Authorization

```mermaid
flowchart LR
	WHAT? --> RBA/AA
```
[x] **Location**
[x] **Request-Time** 
[x] **Frequency**

#### PAM (Privileged Access Management)

~~Shared accounts, same passwords~~ --> Shared account without shared passwords with **PAM**

With PAM, users still only have to remember **1 password** and they have to use **MFA**, so it garanties **no repudiation** (MFA identifies user, *a shared password can be anyone*).

```mermaid
flowchart LR
	Admin1 --MFA -->PAM
	Admin2 --MFA -->PAM
	Admin3 --MFA -->PAM
	PAM --> System1_(PW1)
	PAM --> System2_(PW2)
	PAM --> System3_(PW3)
```


### Audit

Check logs status and changes.

--> **User Behaviour Analytics (UBA)** or **User Entity Behaviour Analytics (UEBA)**

Spot anomalies in log systems with Machine Learning


#### Federation Capability

Integrate with other security/identity domains
--> **Connection**


*Notes:*
CIAM (Costumer Identity and Access Management) --> IAM in customer-facing applications
Worforce Indentity --> processes, tools and stretegies used to manage workforce