# Terms and basics

**Layer 2 (data link layer)**
- Transmission of frames between devices
- Bridged VPM
- Layer 2 virtual devices are called TAP (tap0, tap1)

**Layer 3 (network layer)**
- Transmission of packets (IP)
- Routed VPN
- Layer 3 virtual devices are called TUN (tun0, tun1)

### PPP
Point-to-Point Protocol (Layer 2)
Creates a connection between two hosts with a virtual network adapter at each end
Used in DSL modems and most VPN protocols

### Key Exchange
VPN peers exchange encryption information to establish a secure connection
- Some protocols use a PSK (*pre-shared key*) and others agree on what security keys to use when a connection is started

### Forward Security
Also "Perfect Forward Security"
New keys are generated for each session
⚠ Session keys **guarantee** that previous communications can't be decrypted by using later keys or leaked master keys

### Ports
Ports used by VPN protocols are the ports on the server
Client choose a local port to connect from
Ports need t be openeed on the server's firewall and on any firewalls between it and the internet

# PPTP
*Point-to-Point Tunneling Protocol*

⚠ Considered **obsolete** because most of the ciphers it uses are easily broken
Uses TCP port 1723 to set up a GRE tunnel, through which a PPP connection (Protocol 47) transfers encrypted packets
Most routers pass PPTP traffic without a problem

# L2TP/IPsec

Layer 2 Tunneling Protocol over IPsec (IP security)
IPsec creates a secure channel through which an L2TP tunnel transfers data

**L2TP**
- Encapsulates Layer 2 traffic to travel over Layer 3 (IP)
- Allows Ethernet bridging over the internet
- No security
**IPsec**
- Creates a secure connection
- Only carries IP traffic

**L2TP/IPsec Connection**
- IPsec uses **IKE** (*Internet Key Exchange*) via UDP port 500 to negotiate a **Security Association** (SA)
- UDP port 4500 for NAT traversal mode
- SA sets up **ESP** (*Encapsulating Security Payload; protocol 50*) to encrypt packets
- L2TP tunnel is established through TCP port 1701, to pass traffic protected with ESP
- PPP establishes virtual network interfaces with IP addresses at each end
- Uses user authentication and machine-level shared secret or certificate
- Useful if you need to transfer Layer 2 data insteas of just Layer 3 data

# IKEv2

Internet Key Exchange, version 2
- IKEv2 manages the SA for an IPsec connection
- Uses UDP port 500, and UDP port 4500 for NAT traversal
- IPsec provides Layer 3 connectivity (IP)
- MOBIKE feature provides quick reconnection -- great for mobile devices

# OpenVPN

- Open-source software and protocol
- Uses OpenSSL library to handle key eschange via SSL/TLS
- Creates a Layer 2 or Layer 3 connection
- Uses a custom security protocol based on TLS
- Uses TCP port 1194 by default, can be changed to other UDP/TCP ports
- Works well through NAT and proxies

# SSTP, WireGuard, and SoftEther

### SSTP
- Secure Socket Tunneling Protocol
- Creates a secure channel using SSL/TLS
- Uses TCP port 443
- Fairly wide support
- Creates a client-to-network connection

### WireGuard
- Software and protocol
- Out-of-band key exchange (keys are assigned to peers in configuration)
- Creates Layer 2 and Layer 3 connections over IP
- Packets are encrypted with the public key of the destination host
- Open source, with a goal of easy auditability
- Not considered finalized yet (Wireguard.com)

### SoftEther
- Software Ethernet
- Offers IPsec, SSTP, and other protocols, in addition to its own protocol
- Send traffic through HTTPS
- Offers Layer 2 and Layer 3 connections
- Open source
- Creates a virtualized Ethernet devices


# SSH

Secure Shell
- Create a connection to a SSH server for port forwarding
- Can forward a local port to a remote port (connect localhost:8080 to server:80)
- Some implementations can open a local port and act as a SOCKS proxy, sending traffic to the server
- SSH doesn't create network interfaces
- Very useful for certain cases
- Widespread and difficult to block