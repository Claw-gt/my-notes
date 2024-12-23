#### Kali Linux
#### [[Mapping#^3a13d2|nmap]]
#### [[Vulnerability Management|Nessus]]
Search vulnerabilities on a host
Scans based on known vulnerabilities
#### [[Mapping#^822a4b|Wireshark]]
#### Lynis
For security configuration assessments
-> Use Center Internet Security (CIS) for understanding Lynis output

Modifications: assign lynis folder to user 'root'
`sudo chown -R 0:0 ./*`
- `-R`: recursively
- `0:0`: root
- `./*`: everything in this directory

#### CIS-CAT Lite
Scans for security configurations weaknesses
#### [[Wireless Networking#^b1d3bb|Aircrack-ng]]
- Connect another wireless adapter (e.g. Alfa AWUS036NH)
- Realtek chipset
- Identify wireless encryption

```
Step 1: airmon-ng
## display wireless interfaces + chipsets
airmon-ng

## e.g., monitor interface wlan0 on channel 9
airmon-ng start wlan0 9

Step 2: airodump-ng
## capture wireless traffic
## channel 9 + AP MAC address + interface in monitor mode
airodump-ng -c 9 --bssid 00:11:33:33:77:00 -w psk mon0

Step 3:aireplay-ng
## deauthenticate wireless client
aireplay-ng -0 1 -a 00:14:6C:7E:40:80 -c 00:0F:B5:FD:FB:C2 mon0

## -0 means deauth
## 1 is the number of deauths to send
## -a is the MAC address of the wireless AP
## -c is the MAC address of the wireless client
```

#### Hashcat
"world's fastest password cracker"

```
## check the help file for specific parameters based on the algorithms used to generate the passwords you want to crack

hashcat -h
```

#### OWASP ZAP
Trial and error

- Zed Attack Proxy
- Free and open-source web application security scanner
*OWASP Juice Shop*
- Intentionally vulnerable web app
- Written in Node.js, Express, and Angular