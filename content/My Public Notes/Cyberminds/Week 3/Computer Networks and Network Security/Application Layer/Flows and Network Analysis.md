Network flows provide data and statistics on packets flowing through and traversing network interfaces
### Devices that provide flow data

- **Routers**
- **Switches**

### Data collected

**Usage**:
- Packet count
- Byte count
**Time of the day**:
- Start sysUpTime
- End sysUpTime
**Port utilization**:
- Input IfIndex
- Output IfIndex
**QoS (*Quality of Service*)**:
- Type of service
- TCP flags
- Protocol
**To/From**:
- Source IP address
- Destination IP address
**Application**:
- Source TCP/UDP Port
- Destination TCP/UDP Port
**Routing and peering**:
- Type of service
- TCP flags
- Protocol

## Protocols
#### NetFlow
Developed by Cisco
#### sFlow
From InMon
#### IPFIX

## Applications

#### DDoS Detection
--> Unusally high number of packets per second (PPS)

#### Data Exfiltration
--> Sending sensitive data to  external IPs

#### Internal threat Detection
--> Abnormal flow patterns