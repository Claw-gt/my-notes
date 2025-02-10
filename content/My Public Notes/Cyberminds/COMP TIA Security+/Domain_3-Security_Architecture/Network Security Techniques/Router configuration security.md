Performs Basic Filtering/Screening => **they reduce the load on firewalls** (they often sit in front of network firewalls)

## Router Access Control Lists
Restrict network traffic

=>Similar to firewall rules
### Standard ACLs
Based on the IP address
`access-list[number] [permit/deny][source][mask]`
### Extended ACLs
Based on more advanced criteria (source and destination, ports and protocols used for communication)

## Firewalls vs Routers

- Firewalls are purpose specific and efficient at complex filtering
- Firewalls have advanced rule capabilities
- Firewalls offer advanced security functionalities (threat intelligence, integrate with IDS)

>[!important] Placing ACLs on routers reduces the burden on firewalls
## Quality of Service (QoS)

Controls prioritize critical network traffic
Provide guaranteed bandwidth to high-priority applications