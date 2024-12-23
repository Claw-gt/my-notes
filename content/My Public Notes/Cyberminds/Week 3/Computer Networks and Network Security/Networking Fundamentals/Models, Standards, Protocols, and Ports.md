
## Networking models

Describes:
- Architecture
- Components
- Design

### OSI Model
Conceptual framework used to describe the functions of a networking systems

<img src="https://www.manageengine.com/network-monitoring/images/network-protocols-osi.jpg">
### TCP/IP Model
Set of standards that allow computers to communicate on a network
The TCP/IP is based on the OSI Model

<img src="https://1.bp.blogspot.com/_FRSoY4n-eek/S21qmcKw5UI/AAAAAAAAAf4/mYCB2024Yrs/w1200-h630-p-k-no-nu/TCPIP+Diagram.jpg">

## Network standards
Network standards define the rules for data communications needed for interoperability of networking technologies and processes
##### Key standards organizations: ISO, ITU, DARPA, IEEE, W3C, and IETF

### *De jure* or fomal standards
Developed by an official industry or govenrment body

e.g. **HTTP, HTML, IP, Ethernet 802.3d**

### *De facto* standards
De-facto standards result from marketplace domination or practice

e.g. **Microsoft Windows, QWERTY keyboard**

## Protocols
A network protocol is a set of rules that determines how data is transmitted between different devices in the same network. They cover: **security**, **communication**, and **netwrok management**

### TCP
- Slower but more reliable
- Applications: FTP, Web browsing, Email
### UDP
- Faster but not guaranteed
- Applications: Live streaming, Online games, calls over the internet

### TCP/IP
Is a collection of protocols

### IoT
Uses diverse protocols for communication

### Crypto Classic
Designed for secure, and efficient blockchain-based payments

- **Bitcoin protocol**
- **Blockchain protocol**

## Ports
see [[Transport Encryption#^c189f9|Ports]]
First and last stop for information sent across a network
- Endpoint of a communication
- A port always has an associated protocol and application
- The protocol is the path that leads to the application's port
- Default protocol ports do not change

| Port            | Connection | Protocol                  |
| --------------- | ---------- | ------------------------- |
| 20              | TCP        | FTP data                  |
| 21              | TCP        | FTP control               |
| 22              | TCP        | SSH                       |
| 23              | TCP        | Telnet                    |
| 25              | TCP        | SMTP                      |
| 53              | UDP,TCP    | DNS                       |
| 67, 68          | UDP        | DHCP                      |
| 69              | UDP        | TFTP                      |
| 80              | TCP        | HTTP                      |
| 110             | TCP        | POP3                      |
| 161             | UDP        | SNMP                      |
| 443             | TCP        | SSL                       |
| 16, 384-32, 767 | UDP        | RTP-based voice and video |

## Sockets
A socket is a two-way communication channel
Is made up of:
- A source IP address
- A protocol
- A port number
- A destination IP address

*You use a socket whenever you send data over your local network or over the Internet*