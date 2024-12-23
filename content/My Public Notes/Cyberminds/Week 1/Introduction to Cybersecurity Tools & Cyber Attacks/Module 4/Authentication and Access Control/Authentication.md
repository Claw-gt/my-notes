Validation of identity
Authentication protocols, servers and standards verify identity

#### Authentication protocols

- Set of digital rules and process systems
- Check digital credential

##### Examples

- **RADIUS (*Remote Authentication Dial-In User Service*)*

	Used in wireless networks and VPN
	Used for remote authentication
	Clients relay authentication messages via the Netwrok Access Server

- **CHAP (*Challenge Handshake Authentication Protocol*)***

	Verification through a three-way handshake process
	Remote access
	
- **EAP (*Extensible Authentication Protocol*)**

	Authenticates users in wireless networks
	Secures remote access point
	Support MD5-challenge, OTP, token card and TLS
	
- **Kerberos**
as Cerberos (the guardian three-head dog from the underground)
	Created by MIT
	Uses strong encryption to protect user credential passed between client and server
	Relies on third-party server --> Key Distribution Center (KDC)
		e.g. Microsoft Windows Active Directory
	👎Single Point of Failure
	BYOD are incompatible with Kerberos
- **TACAS+**

	For Network infrastructure devices

#### Authentication servers

- Manage user credentials
- Verify identities
- Grant or deny access
- Intermediaries between user and resource

##### Examples
- Active Directory
- LDAP servers
- RADIUS servers

#### Password authentication

⚠ Brute force to gain credential
⚠ Password update required

--> Solution: MFA or 2FA

#### Other methods of authentication

##### OTP (One Time Password)
- Valid for a single use -> prevents from brute force events
##### Biometric authentication
- Fingerprints
- Voice / Face recognition
##### Smart cards
##### Security tokens
##### Mobile push notifications