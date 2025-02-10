Protect **physical security** of switch
Unlike routers that centrally located in secure data centers or netwrok rooms, switches are spread all over the place

⚠ An attacker who gains physical access to your switch controls that portion of the network

**VLAN Security**: Disable automatic trunk negotiation to prevent VLAN hopping attacks
\**VLAN trunking*: technology that switches use to carry VLANs accross many switches
## VLAN Pruning
Implement **Least Privilege Rule**: only trunk VLAN if that VLAN is needes on that switch
Limit unnecessary exposure of VLANs by limiting the number of switches where they are trunked, especially for sensitive VLANs

## VLAN Trunk Negotiation
VLAN hoping attack by pretending to be a switch
**Deny automatic VLAN trunk negotiation** to limit the effectiveness of VLAN hopping attacks

## Port Security
Limit the devices that may connect to a network switchport by MAC address (avoid connection of rogue devices)
Effective against MAC flooding

- **Static Port Security**
Administrator *manually* configure valid MAC addresses for each port
- more secure

- **Dynamic Port Security**
Switches memorize the first MAC address they see on each port and limit access to that address
- faster but more risky
## DHCP Snooping
Block malicious DHCP traffic