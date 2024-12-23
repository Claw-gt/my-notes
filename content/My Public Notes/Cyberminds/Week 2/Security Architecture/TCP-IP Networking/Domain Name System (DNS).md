DNS provides address resolution on the Internet
- DNS operates over UDP port 53
### DNS Servers
Translate between domain names and IP addresses

### DNS Resolution

1. User types domain name into browser
2. Computer sends a DNS query to the local DNS server
3. DNS server responds with an IP address
4. Computer contacts the server at that IP address

### DNS is a Hierarchical System
Organizations designate DNS servers that are authoritative for their domains

If local DNS does not have the domain --> DNS server

#### TOOL: `dig`

⚠ Some content filters alter DNS query results


### DNSSEC
Adds digital signatures to DNS
- Allows users to verify the authenticity of the domain
--> Avoids *DNS poisoning attack* (registering a fake DNS in a DNS server)