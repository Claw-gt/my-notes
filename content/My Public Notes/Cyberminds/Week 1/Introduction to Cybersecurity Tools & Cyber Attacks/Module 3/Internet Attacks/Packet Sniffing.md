Unauthorized access to transmitted information

- Uses software to analyze data packets
- Collects various data points by intercepting traffic

Packet sniffers operate by placing NIC (*Network Interface Card*) and protocols like IP, TCP, UDP and HTTP
- NIC attends traffic only addressed to it
- NIC in **promiscous mode** captures all traffic ^58f278

##### IT Professionals

**Network diagnosis**
- Identify suspicious activity
**Performance monitoring**
- Provide critical data on bandwith consumption
**Web activity monitoring**
- Tracking visited websites
- Oversees communication exchanges

##### Sniffing attack
- Intercept unencrypted packets
- Examines personal and financial data
**Address Resolution Protocol (ARP)** tampering
**Domain Name System (DNS)** falsification
**SQL injection**

>[!info]
>Types of sniffing attacks
>
>**Passive sniffing**
>- Involves multiple connecting networks
>- Monitor data on LANs or Wi-Fi
>- Mimics spying, making detection challenging
>*Attacker connects to a HUB which is connected to a network of computers inside a LAN*
>
>**Active sniffing**
>- Manipulates network traffic
>- Targets switched networks by introducing additional traffic
>*Attacker generates extra network activity, causing switches to broadcast data widely, enabling the interception of specific packets*

#### Network Security strategies

✅Update software and systems
✅Strengthen login measures --> strong passwords and 2FA
✅Exercise caution with emails
✅Browse privately with a VPN
✅Navigate to HTTPS-secured websites

---
#### Packets
Units of data transmitted over networks
###### Header
Initial point of reference (24 bytes)
Serves as the packet's postage label
Contains source, destination, packet number

- Source IP identifies sender
- Destination IP specifies recipient
- Packet number aids reassembly
###### Payload

Substantive content of the packet
Carries teh actual data being transmitted

---