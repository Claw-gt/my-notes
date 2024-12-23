# Firewalls
## Types of Firewalls

#### Stateless firewall
Examine packet **headers** only

#### Stateful firewall
Monitor active connections

#### Application-level firewalls
Operates at the applcication layer of the OSI model
Inspect packet **payload**
Enables granular control

>[!warning] Firewalls provide little protection against internal threats

>[!warning] Firewalls cannot prevent an attack if the vulnerability is not yet identified (zero-day exploits)


>[!warning] Firewalls have difficulty handling encrypted traffic

---
# Intrusion System


|          System type          | Network-based                                                                           | Host-based                                                                                                       | 👍                                       | 👎                                                                                          |
| :---------------------------: | :-------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------- | :--------------------------------------- | :------------------------------------------------------------------------------------------ |
| Intrusion detection<br>(IDS)  | - **Monitors** network-wide traffic patterns<br>- Flags anomalies and potential threats | - Monitors individual hosts and devices<br>- Scrutinized system logs, file modifications, and process activities | Comprehensive capabilities               | - Can suffer from **overload** from the volumen of alerts<br>- High rate of false positives |
| Intrusion prevention<br>(IPS) | - Scrutinizes incoming and outgoing traffic, **neutralizing known threats**             | - Thwarts system activities in real time to stop unauthorized file modifications or malware execution attempts   | Immediate threat prevention and response | - Risk of false positives<br>- Requires meticulous configuration                            |

---

# Intrusion System + Firewalls


| Firewalls               | Intrusion Detection Systems                 | Intrusion Prevention Systems                         |
| ----------------------- | ------------------------------------------- | ---------------------------------------------------- |
| Block known threats     | Alert admins to potential security breaches |                                                      |
| Filter incoming traffic |                                             | Actively inspect and neutralize threats in real-time |
|                         |                                             |                                                      |

>[!warning] Lack of application layer inspection
>Vulnerable to SQL injection, XSS

