## Firewall Log Details
- Details of attempted connections
- Timestamp
- Relevant firewall rule
- Useful in security incident investigation
- Network issue troubleshooting
- Anomalous activity detection
=> Full packet capture require large storage capacity. Therefore, the alternative is **Network Flow Data**
## Network Flow Data

^55a736

a.k.a NetFlow data
=> captures connection details, a summary
- Source and destination systems
- Source and destination ports
- Timestamps
- Amount of data transferred
Does not capture *what* was communicated but does identify *who, when, and how much*
## SIEM
Network security systems that automate the collection and analysis of logs from many different systems for security purposes

- Automates logs analysis
- Rapid analysis

**SIEM Log Sources**:
- Firewalls
- Network devices
- Servers
- Applications