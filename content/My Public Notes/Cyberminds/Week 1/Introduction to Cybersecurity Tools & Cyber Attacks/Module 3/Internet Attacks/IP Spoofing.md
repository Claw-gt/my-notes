[IP Spoofing & Spoof Attacks](https://www.kaspersky.com/resource-center/threats/ip-spoofing)

---
#### Network communication

- Relies on IP packets exchange
- Backbone of internet interactions
- Packet contains a header with routing data -> Source and Destination addresses
---

- Manipulate packet headers
- Conceal sender's origin
- Alter source address


##### IP Spoofing can be used for other attacks:

-> **Distributed DoS attacks**
Alter the source IP address to overload a service

-> **Botnet devices**
Shield the botnet's activities by assigning fictitious IP addresses

-> **Man-in-the-middle attack**
Intercepts the exchange between two systems, modify the packets, and then forward them undetected by the authentic communicator or recipient

#### Security strategies

✅Ingress filtering
- Type of packet filtering --> scrutinize incoming IP packets and inspect source IP header
- Establishes a critical network security measure
- Allows only authentic and legitimate traffic
- Network's perimeter acts as a barrier

✅Egress filtering
- Network protection technique
- Scrutinizes outgoing IP packets
- Verifies authencity of source headers