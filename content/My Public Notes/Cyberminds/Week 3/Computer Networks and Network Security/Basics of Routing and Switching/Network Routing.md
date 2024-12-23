A packet contains voth layer 2 (burned into each NIC by the manufacturer) and layer 3 (assigned by network administrator) addresses

| Layer 2                          | Layer 3                            |
| -------------------------------- | ---------------------------------- |
| MAC addresses                    | IP addresses                       |
| **Physical** identifiers in NICs | **Logical** addressing and routing |
## Address Resolution Protocol (ARP)

- Sends data to IP address
- Ensures correct device
- Resolves IP to MAC
- Enables proper printing

`ip neigh show` in Linux to show ARP table
`arp -a` in Windows to show ARP table

`ip route show` in Linux to show gateway and IP of router
`route print` or `netstat -rn` in Windows

`tracepath` and `ip addr show` in Linux
## Routers and Routing tables

Routing tables determine the path for data packets

### Routes

#### Default routes
Sends data to a destination not listed in the routing table --> **Default gateway**
#### Direct/Connected routes

#### Dynamic and static route
##### Static
Manually set by a network administrator
##### Dynamic
Routes are updated through dynamic routing protocols


---

## Layer 2 and Layer 3 Addressing

### Network interface card (NIC) connections
[[Computer Networks#^9bda1d|NICs]]

- Connect internal networks to public networks
- Exist as a chip or separate device
- Support wired or wireless conntections
- Contain burned-in physical address (the [[Network Attacks#^a38c33|MAC address]])

---

>[!info] Broadcast domains can also be called VLANs

