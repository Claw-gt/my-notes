
# IPv4

- 32-bit addressing schema
- Divided into four octets
- Represents binary digits
- Ranges from 0 to 255 in decimal
- Provides 4,294,967,296
see [[IP addresses and DHCP#^97008b|Subnets]]
### Network
- Assigns a unique identifier
- Identifies the network class
- Is common to all attached devices

### Host
- Identifies each machine uniquely
- Varies for each host
- Attached to a particular device
- The size of the host portion **determines the number of endpoint a network segment can support**

### Subnet number
- Divides large networks into sbnets
- Assigns subnet numbers

## Classful addressing schema

### Class A networks
- Range from 0.0.0.0 to 127.255.255.255
- The default subnet mask is 255.0.0.0
- First octet for **network portion**
- Last three octets for *host*

### Class B networks
- Range from 128.0.0.0 to 191.255.255.255
- The default subnet mask is 255.255.0.0
- Use the first two octets for **network**
- Use the last two octets for *host*

### Class C networks
- Range from 192.0.0.0 to 223.255.255.255
- The default subnet mask is 255.255.255.0
- Use the first three for the **network**
- Use last octet for *host*

### Class D networks
- Range from 224.0.0.0 to 239.255.255.255
- Reserved for multicast

### Class E networks
- Range from 240.0.0.0 to 255.255.255.255
- Reserved for future use

## Addressing schema

### Unicast
- Communicates one-one
- Identifies a single node
- Sends and receives data
- Supports both IPv4 and IPv6
### Broadcast

^3d9e6f

- Communicates with all
- Holds the same network portion as other computers
- Host portion bits are set to 1 to send packets to all endpoints
### Multicast
- One-many arrangement
- Systems subscribe to a multicast address
- Uses addresses from 224.0.0.0 to 239.255.255.255

## [[IP routing#^e248f7|IP header]]

---

# IPv6

> [!info] Benefits of IPv6
> - Increased address space
> - Built-in security
> - Improved efficiency

- 128 bits long
- Uses hexadecimal numbers
- No shortage of IP addresses

## Addressing schema

### Unicast
- Same as in IPv4

### Multicast
- Same as in IPv4

### Anycast
- [[#^3d9e6f|Broadcast]] is replaced by Anycast
- Assigns to more than one interface
- The address belongs to various endpoints

## IPv6 header

<img src="https://docs.oracle.com/cd/E23823_01/html/816-4554/figures/HeaderFormat.png">

##### Source and IP addresses
128 bits long

### Rules for IPv6 header

> [!info]+ Double colon to represent consecutive zeros
> **Example:**
> 0:0:0:0:0:0:0:1 --> ::1
> *It can be only applied once for a single IP address*

 >[!info]+ Used mixed notation for compatibility
> **Example:**
> ::ffff:192.0.2.128

>[!info]+ Compress consecutive zeros
> **Example:**
> 2001:0:0:1:0:0:0:1 --> 2001::1:0:0:0:1

---

### Creating subnets

$2^n$ subnets, where $n$ are the bits borrowed from the host sections
The borrowed bits are used for broadcast and network addresses