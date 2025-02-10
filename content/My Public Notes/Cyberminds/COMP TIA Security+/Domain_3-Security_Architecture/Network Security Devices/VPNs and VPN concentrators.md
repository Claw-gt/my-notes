## Site-to-Site VPNs
Connect remote offices to each other and headquarters

## Remote Access VPNs
Provide remote access to corporate networks for mobile users

---
![[Cyberminds Academy/COMP TIA Security+/Domain_3-Security_Architecture/Network Security Devices/attachments/image 3.png]]

Use encryption => Virtual tunnel

**VPN Endpoints**
- Firewalls
- Routers
- Servers
These previous devices can cause performance issues since they do not have crypto accelerator
- VPN concentrators (for high volume of VPN traffic)

They used the protocol **IPSec**

# IPSec

^5774fc
Set of protocols created to add security to TCP/IP
Unlike TLS, IP secures the entire packet payload

IPSec uses two protocols to encrypt informations:
1. *Encapsulating Security Payload (ESP)*: provides confidentiality and integrity protection for packet payloads
	- **Security Association (SA)**: identifies cryptographic algorithms. Most secure one is chosen. **IKE** creates SAs over port 500
2. *Authenticator Header (AH)*: provides integrity protection for packet headers and payloads
=> AH and ESP can be combined


- Works at the Network Layer (Layer 3)
- Supports Layer 2 Tunneling Protocol (L2TP)
- Provides secure transport
- Difficult to configure
- Less common for remote users VPN, more usual to static
*port 1701 UDP*
##### Site-to-Site VPNs
Encrypted tunnels connecting two networks together in a manner that is transparent to users
- **Tunnel mode**
##### End-User VPNs
Provide encrypted remote network access for individual systems
- **Transport mode**
# SSL/TLS VPNs

- Remote user VPNs now often rely upon SSL/TLS VPNs
- Work at the Application Layer over port 443
- OpenVPN: open source
- SSTP (Secure Socket Tunneling Protocol): proprietary of Windows *over port 443*
⚠ PPTP is deprecated
# HTML5 VPNs

- Work entirely within the web browser in  a proxying rule
---

## Full-Tunnel VPN

All network traffic leaving the connected device is routed through the VPN tunnel, regardless of the destination

## Split-Tunnel VPN

Only traffic destined for the corporate network is sent through the VPN tunnel. Other traffic is routed directly ove the Internet
Reduces the bandwisth
⚠ Provide users with a false sense of security

## Always On VPN

Connects automatically. Takes away control of the end user