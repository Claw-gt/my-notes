Process of visualizing a network's physical and logical connections, such as routers, switches, and servers.
- Manage the network's complexity
- Troubleshoot issues
- Detect anomalies
#### [[nmap]]

^3a13d2
see [[Network port scanning and service identification]]
Network mapping tool
- Identify devices
- Detect open ports
- Detect security risks
- Automate network
**CheatSheet**: [HighOn.Coffee • Security Research • Penetration Testing Blog](https://highon.coffee/)
#### Wireshark

^822a4b

Network protocol analyzer
- Provides network traffic visibility
- Maps network activity in real-time
- Dissect packets
- Examine protocol-level interaction
- Ensure accurate network communications


| Queries                              | Description                                      |
| ------------------------------------ | ------------------------------------------------ |
| `http.response.code == 200`          | Filter for http status code                      |
| `http.user_agent == "xxx"`           | Filter to HTTP User Agent                        |
| `ip.addr == x.x.x.x`                 | Set filter for specific IP (both as src and dst) |
| `tcp.dstport = xx`                   | Filter Port to TCP destination                   |
| `tcp.srcport == xx`                  | Filter Port to TCP source                        |
| `ip.dst == x.x.x.x`                  | Filter IP to destination                         |
| `ip.src == x.x.x.x`                  | Filter IP to target                              |
| `ip.proto == 1`                      | Filter ICMP                                      |
| `icmp.type != 0`                     | ICMP non valid responses                         |
| `http.request.uri == "/example.php"` | Filter for requests to URL                       |

##### Mapping attack
- **Identify**:
	- Unguarded entry points
	- Vulnerable systems
	- Defenses
- **Navigate** the network
- **Prioritize** target segments
- **Deduce** high-value assets

>[!important]
>With this tools, attacker can:
