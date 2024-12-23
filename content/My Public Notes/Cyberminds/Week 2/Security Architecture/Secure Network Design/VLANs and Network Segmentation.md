# VLAN

Virtual LANs separate systems on a network into logical groups based upon function, regardless of pysical location
Switches cary VLANs on a network

## Typical Network Diagram

```mermaid
flowchart LR
	Firewall --- Accounting
	Firewall --- Sales
	Firewall --- IT
```
## Network Border Firewall

```mermaid
flowchart LR
subgraph San Francisco
	User1 --- IT
	User2 --- HR
	User3 --- Sales
end
subgraph New York
	User4 --- User1
	User5 --- User2
	User6 --- User3
end
subgraph Networks
	IT --- User4
	HR --- User5
	Sales --- User6
end
```
--> VLANs extend the broadcast domain
--> *Users on the same VLAN will be able to contact each other as if they were connected to the same switch*

## Configuring VLANs

- Enable VLAN trunking
- Assign switch ports to VLANs
