- Allow deep inspection of traffic
- Troubleshoot network issues
- Investigate security incidents
- Eavesdrop on confidential communications
## TOOL:

#### [[Mapping#^822a4b|Wireshark]]

#### `tcpdump`
Open-source command-line protocol analyzer
Displays singel network packet
`tcpdump -n -i eth0 'tcp port 22'`

- Same language as Wireshark => They are both built on the **libpcap** library
#### `tcpreplay`
Allows editing and replaying traffic