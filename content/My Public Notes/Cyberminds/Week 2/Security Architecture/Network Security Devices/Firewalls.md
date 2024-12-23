Security guards at the perimeter of a network

see [[Cyberminds Academy/Week 1/Cybersecurity Architecture/Module 3/Network Security/Firewalls|Firewalls]]

## [[Stateless Inspection|Stateless Firewall]]
Evaluates each connection independently

## [[Stateful Inspection|Stateful Firewall]]
Tracks open connections

a.k.a **Layer 4 Firewall** --> works at the Transport Layer

---

## Rule Conents

- Source system address
- Destination system address
- Destination port and protocol
- Action (allow or deny)

### Implicit Deny or Default Deny

If the firewall receives traffic not explicitly allowed by a firewall rule, the that traffic must be blocked

#### Network Firewall
Hardware devices that regulate connections between two networks
#### Host Firewall
Sofware component of an operating system that limit connections to a server
## Next Generation Firewalls (NGFWs)

Layer 7 firewalls 
They incorporate decision-making

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

**Hardware WAF**
**Software WAF**
**Cloud WAF** --> effective againt DoS
**XML Firewall** --> filters access to REST APIs

	

