- Cloud customers must build and manage virtual networks in the cloud
- Cloud networking is highly virtualized and customizable

```mermaid
flowchart TD
	Firewall --- Public_VLAN
	Firewall --- Database_VLAN
	Firewall --- Admin_VLAN
```
In a traditional data center, virtual LANs (VLANs) separate systems of differing security levels

```mermaid
flowchart TD
	Firewall --- Public_VPC
	Firewall --- Database_VPC
	Firewall --- Admin_VPC
```

Cloud providers use virtual private clouds (VPCs) and similar concepts for the same purpose

### VPC Endpoints
Provide secure VPC interconnection

### SDN
Software-defined networking

### SDV
Software-defined visibility