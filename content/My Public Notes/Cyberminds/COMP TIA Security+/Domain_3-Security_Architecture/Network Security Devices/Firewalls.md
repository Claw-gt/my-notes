Security guards at the perimeter of a network

see [[Cyberminds Academy/Week 1/Cybersecurity Architecture/Module 3/Network Security/Firewalls|Firewalls]]

## [[Stateless Inspection|Stateless Firewall]]
Evaluates each connection (packet) independently

## [[Stateful Inspection|Stateful Firewall]]
Tracks open connections
a.k.a **Layer 4 Firewall** => works at the Transport Layer

---

## Rule Conents

- Source system address
- Destination system address
- Destination port and protocol
- Action (allow or deny)

### Implicit Deny or Default Deny

If the firewall receives traffic not explicitly allowed by a firewall rule, then that traffic must be blocked

#### Network Firewall
Hardware devices that regulate connections between two networks

![[Cyberminds Academy/COMP TIA Security+/Domain_3-Security_Architecture/Network Security Devices/attachments/image.png]]
#### Host Firewall
Sofware applications or operating system components that limit connections to a server
## Next Generation Firewalls (NGFWs)

Layer 7 firewalls 
They incorporate contextual information into their decision-making process

## Firewall Roles

- NAT gateway
- Content/URL filtering
- Web application firewalls (**WAFs**) protects from
	SQL injection
	XSS
	Directory traversal
	Buffer overflows
	Privilege escalation
	Cookie-based attacks

## Firewall Deployment

- Network Hardware vs Host-based software
- Open source (SW firewall) vs. proprietary (SW firewall and HW firewall)
- Hardware appliance (built-in) vs. Virtual appliance (loaded directly into a virtualization platform)

# Web Application Firewall (WAF)
Screens web connections

- Hardware WAF: Physical device positioned between the network firewall and web server
- Software WAF: Software running on the web server that screens requests
- Cloud WAF: Third-party service that remotely filters malicious traffic => effective againt DDoS
- XML Firewall: Filters access to REST APIs

Component of **defense-in-depth**

![[Cyberminds Academy/COMP TIA Security+/Domain_3-Security_Architecture/Network Security Devices/attachments/image 1.png]]
