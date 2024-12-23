IP is a Layer 3 protocol that uses IP headers to identify and process network traffic in the form of packets
## IP header : Components

^e248f7


<img src="https://media.geeksforgeeks.org/wp-content/uploads/20220222105138/geekforgeeksIPv4header.png">

##### Version
- Declares protocol version first
- Interprets IPv4 and IPv6 headers
##### Time To Live (TTL)
- Sets TTL to limit hops
- Decreases TTL per hop
- Drops packet at TTL zero
- Prevent internet congestion
- Recommends TTL value (64)
##### Protocol ID
- Identifies each protocol with ID number
##### Source IP
- Identifies the sender
##### Destination
- Receives the packet
##### Payload / Data
- Contains the message content

**Packet analysis with:** Wireshark
## [[Mapping#^822a4b|Wireshark]]
Captures packets

## Network mask
Defines network and subnet information
- /24 notation indicates the network portion
- Accomplishes division of an IP address

## Broadcast IP address
The opposite of a network mask

<img src="https://digitalmediaglobe.com/wp-content/uploads/2020/09/Network-address-Broadcast-address.jpg">

- Broadcast IP address has all the octets
- Original IP address with the octets
- Bits of the host portion are on (set to **1**)

## Default gateway
Helps to send the packet outside the local network
