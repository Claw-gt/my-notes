# Network discovery

### Active Scanners
- Interact with target systems
- Generate network traffic
- Fingerprint the OS
- Identify available services
### Passive Scanners
- Do *not* interact with target systems
- Monitor network traffic
- Extract packet data for offline analysis

# OSINT

### DNS Zone Transfer

>[!info]
>Process of copying all the DNS records from one DNS server (usually the master or primary DNS server) to another DNS server (usually the secondary or slave DNS server). This ensures that both servers maintain identical information about domain names, IP addresses, and other DNS records in their respective zones


- Extract information from DNS servers
- Should be restricted
- Target internet-facing DNS servers

## Tools
- [Shodan Search Engine](https://www.shodan.io/)
- [Censys Search](https://search.censys.io/)
- [Hurricane Electric BGP Toolkit](https://bgp.he.net/)
- [DNS Server Scanner - Free AXFR test - Pentest-Tools.com](https://pentest-tools.com/network-vulnerability-scanning/dns-zone-transfer-check)