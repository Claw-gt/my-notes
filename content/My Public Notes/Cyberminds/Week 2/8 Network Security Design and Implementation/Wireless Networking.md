# Wi-Fi

It is a standard
- Wi-Fi devices replace network cables with radio transmitters and receivers
- Chip with antenna
- They are radio transmissions --> Wi-Fi signals travel over open airwaves and are subject to undetectable interception

> [!info] Wi-Fi standard
> 802.11 (1997) allows 2 Mbps communciation
> 802.11b (1999) allows 11 Mbps communciation
> 802.11g (2003) allows 22 Mbps communciation
> 802.11n (2009) allows 600 Mbps communciation
> 802.11ac (2014) allows 1 Gbps+ communciation
# WAPs
**Wireless Access Points**
- Connect wireless networks to wired networks and the Internet
- Connected with a cable to a trdaitional wired network
- Wireless devices in the area can communicate with the access point to connect to other networks

---

# Wireless Encryption

## Wired Equivalent Privacy (WEP)

Original wireless encryption standard
Security vulnerabilities
No longer secure

## Wi-Fi Protected Access (WPA)

Replaced WEP in 2003
Uses the Temporal Key Integrity Protocol (TKIP) to rapidly rotate encryption keys
Contains vulnerabilities
No longer secure

## Wi-Fi Protected Access v2 (WPA2)

Released in 2004 as upgrade to WPA
Encrypts packets using AES encryption
Uses the CCM protocol
Potential security issues
It is considered secure

## Wi-Fi Protected Access v3 (WPA3)

Required on new Wi-Fi devices from 2020 onward
Support CCMP
Uses Simultaneous Authentication of Equals (SAE) for key exchange --> Based on Diffie-Hellman


| Standard | Status   |
| -------- | -------- |
| WEP      | Insecure |
| WPA      | Insecure |
| WPA2     | Secure   |
| WPA3     | Secure   |

# Wireless authentication

## Pre-shared keys:
- Simplest form
- Home network

#### Limitations
- Burden to change the encryption key
- Impossible to identify users and revoking individual user access

### Hexadecimal String
64-hexadecimal characters that encode a 256-bit encryption key
### Password
8-13 ASCII characters that are converted to a 256-bit encryption key using PBKDF2


## Enterprise Authentication
Individual credentials

### Lightweight EAP (LEAP)
Insecure protocol that relies upon MS-CHAP

### EAP
Broad framework with many variants, some secure, some not
#### EAP-TLS -- Secure
#### EAP-TTLS -- Secure

#### EAP-FAST -- Secure

#### EAP-MD5 -- Not Secure

### Protected EAP (PEAP)
Tunnels EAP iside an encrypted TLS session

## Captive Portals
Redirect users to an authorization page

---
# Wireless signal propagation

Use a **Site survey** to place effciently the antennas:
- Heat map
## Omnidirectional antennas
Send a signal in all directions

## Directional antennas
Direct all power from an access point in a single direction

## Beamforming Technology
802.11 ac
Virtual directional antenna that shifts as needes based on device's location

*Note:  manipulating power levels modifies wireless signal range*

----
# Wireless equipment

### Fat Access Points
Contain HW +SW needed to operate a wireless network

### Thin Access Point
Rely upon wireless controllers for configuration and to serve as the 'brains' of the wireless networks

## Wi-Fi Analyzers
Search for rogue networks and test wireless security
*Aircrack-ng* -> wireless security testing tool ^b1d3bb
