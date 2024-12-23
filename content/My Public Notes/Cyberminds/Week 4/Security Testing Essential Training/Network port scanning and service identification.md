#### nmap
Scans the 1000 most common ports by default

No Ping, assume the host is up (more accurate results):
`nmap -Pn <IP>`

Service and Version info
`nmap -A <target>`

Specific Ports
`nmap -p 80 <target>`
`nmap -p 1-65535 <target>`

#### Example

`nmap scanme.nmap.org`

For more details:
`nmap -v -A scanme.nmap.org`
