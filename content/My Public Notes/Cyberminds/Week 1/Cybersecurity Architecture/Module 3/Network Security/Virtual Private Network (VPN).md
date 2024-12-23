
- Secure channel over an untrusted network (*tunnel*)
- Encryption --> Confidentiality
- Limited Inspection Capabilities

[[OSI Model]]
![Table showing the OSI layers: Application, Presentation, Session, Transport, Network, Data Link, Physical](https://muirlandoracle.co.uk/wp-content/uploads/2020/02/OSI-Table.png)

The security measures are inherited by the upper layers:
*If you add encryption in Netwrok layer, the above layers will have encryption*

- Application Layer --> **SSH**
- Transport Layer --> **TLS/SSL**
- Network Layer --> **IPSec**
- Data Link Layer --> **PPTP/L2TP**

#### Types of VPN

**Broad VPN**
--> Net based
[x] Simple
[x] Catch-all (inheritance by layers)

**App Specific**
[x] Granularity
[x] Control