> [!info] TCP/IP
> Transmission Control Protocol / Internet Protocol

# Internet Protocol (IP)
*Not only on the Internet, also on home/office networks*

- Routes information across networks
- Provides an addressing scheme (**IP addessing**)
- Delivers packets from source to destination
- Serves as a network layer protocol
- IP supports **transport layer protocols** that have higher level responsibilities

**Main Transport Layer Protocols:**

- Transmission Control Protocol (TCP)
- User Datagram Protocol (UDP)

# Transmission Control Protocol (TCP)

- Is a connection-oriented protocol
- Guarantees delivery through acknowledgment
- Is widely used for critical applications (such as emails and websites)

### TCP Flags
--> 3-way Handshaking process
--> Flags that are contained within the TCP packets

- **SYN**: opens a connection
- **FIN**: closes a connection
- **ACK**: acknowledges a SYN or FIN request


![The three way handshake](https://muirlandoracle.co.uk/wp-content/uploads/2020/03/image-2.png)


# User Datagram Protocol (UDP)

Does not use the 3-way handshake
- Is not a connection-oriented protocol
- Is a lightweight, connectionless protocol
- Doesn't send acknowledgments or guarantee delivery
- Is used for voice and video applications

# OSI Model

![Table showing the OSI layers: Application, Presentation, Session, Transport, Network, Data Link, Physical](https://muirlandoracle.co.uk/wp-content/uploads/2020/02/OSI-Table.png)

See [[OSI Model]] for more information about each layer

**Application Layer**: User programs
**Presentation Layer**: Data translation and encryption
**Session Layer**: Exchange between systems
**Transport Layer**: TCP and UDP
**Network Layer**: Internet Protocol (IP)
**Data Link Layer**: Data transfers betwen two nodes
**Physical Layer**: Wires, radios, and optics



