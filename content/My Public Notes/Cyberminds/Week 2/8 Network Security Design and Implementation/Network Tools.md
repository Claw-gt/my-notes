# ping and traceroute

see [[ping]] and [[ICMP#^58aa21|ping]]

see [[traceroute]] and [[ICMP#^b25427|traceroute]]

--> **Some systems don't respond to ping requests**: firewall rules

In Windows: ~~traceroute~~ `tracert`
## `hping`
Creates customized ping requests

## `pathping`
Combines ping + tracert in **Windows**

---
# DNS tools

## `dig`

In Windows: ~~dig~~ `nslookup`

## `whois`
**whois.domaintools.com**
Discovers ownership of the domain
--> Most use privacy tools

## `Reverse whois`
**viewdns.info**

---

# Ipconfig, ifconfig, and route

In Windows: ~~ifconfig~~ `ipconfig`
Displays MAC addresses (ether)
## `route`
Displays network traffic routing information

---
# netstat
All active network connection

In Linux: ~~netstat~~ `ss`

---
# netcat

## `nc`
see [[Bandit#^d7f944|Bandit CTF]] for a practical example with `nc`

Opens raw network connections on Mac and Linux
After connection, the user can type direct commands
No equivalent on Windows

---

# ARP
ARP translated between IP addresses used at the network layer and MAC addresses used at the Ethernet layer
- Works only on local networks
## `arp`
IP and MAC addresses

---
# curl
Retrieves data from the Internet
- Can be used to download files

---
# theHarvester
Mines the Internet for domain information

`python3 theHarvester.py -d <domain.com> -b all -l 200`

---
# cuckoo
Sandbox environment that allows you to test suspicious files to determine wheter they might display malicious activity

For **malware analysis**
Analyze:
- Executables
- Documents
- Email messages
- Websites

---
### Port Scanners
Probes for open network ports
### Vulnerability Scanners
Proves for known vulnerabilities
### Application Scanner
Test for application security flaws

# Port scanners

## `nmap`

## `scanless`
Pyhton script automating port scans

---
# Vulnerability Scanners
Scan probes open ports fro known vulnerabilities

## `Nessus`
Popular vulnerability scanner

## `Sn1per`
Automates penetration testing
