--> Provides an extra layer os security
--> Uses traffic routing device as intermediary
--> For outbound data, NAT creates an external IP address that **masks the internal IP address**
--> For inbound data, NAT translates the public IP address to the private IP address

### Benefits
- IP address conservation
- Security against external threats
- Simplified network management

### Types of NAT

##### Static
Maps one private IP address to one public IP address

##### Dynamic
Maps multiple private IP addresses to a public IP address
Uses a pool of public addresses

##### Port Address Translation (PAT)
a.k.a **NAT overload**
Maps multiple private IP addresses to a single public IP address
Uses different port number for each session
The most common form of NAT used in home networks


### NAT in use

#### Internal networks and outbound devices

Devices in the home network share an IP address with different port assignments (PAT)

#### Outgoing network traffic

Uses a static public IP address

### Common problems

- Port forwarding problems
- IP address conflicts
- Performance overhead