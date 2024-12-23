- Identify and removes SPOFs
- Redundancy addresses SPOFs

```mermaid
flowchart LR
WebServer_Cluster --Firewall--> Internet
WebServer_Cluster --Firewall--> Internet
```

- Bankruptcy
- Insufficient storage
- Perform succession planning for staff

---
# High Availability

Uses multiple systems to protect against service failure --> **Redundancy**

>[!warning] Not the same as load balancing
# Fault Tolerance

Makes a single system resilient against technical failure

**Techniques**:
- Power Supplies --> UPSs, PDUs
- Redundant Array of Inexpensive Disks (RAID) 

**Disk mirroring, RAID 1**, stores the same data on two different disks:

<img src="https://th.bing.com/th/id/OIP.usNRBc3niwIDW3JDCiegjgAAAA?rs=1&pid=ImgDetMain">

**Disk striping with parity, RAID 5**, uses three or more disks to store data and parity information

<img src="https://www.fusiondatarecovery.com/images/pages/RAID-5.PNG">

>[!warning] *not a backup strategy*

- Network Redundancy --> Multiple ISPs, NIC teaming, Multipath networking
- Platform Diversity --> Technologies, vendors, cryptography
- Multicloud --> adds resilience to operations
