#### nmap

`nmap -sn <IP range>`
-sn : ping requests

`nmap -PS <IP>`
-PS: TCP scan
nmap cancels the connection before the three way handshake is completed

`nmap -PS -P0 <IP>`
-P0: without

`sudo nmap -sU <IP>`
-sU: UDP scan

`nmap -p22 -sV <IP>`
-p22: specifies service
-sV: verson of the service

`sudo nmap -sSUV -p U:53,11,137,T:21-25,80,39,8080 <IP>`

`sudo nmap -O <IP>`
-O: fingerprint the OS

#### netcat

*On Kali:*
`myip`
-->10.0.2.15
`nc -lp 4545`
--> netcat is listening on port 4545

*On another machine:*
`nc64 10.0.2.15 4545`
`Hello Universe`
--> Connects to Kali

`nc64 -lp 4545 > incoming.txt`
--> Data sent is not received on stdout but on a file

---
*Connect to websites using netcat*
`nc -v google.com 80`
`GET index.html HTTP/1.1`


#### tcpdump

`tcpdump -D`

`sudo tcpdump -i any -c 10`
`sudo tcpdump -i eth0 -c 10 -nn`

`sudo tcpdump -i eth0 -c 10 -s0 -tX`
-t: readable form
-X: in hexadecimal
-s: size of data ('0' for full packet)

`sudo tcpdump -i eth0 -c 10 host <IP>`
`sudo tcpdump -i eth0 -c 10 udp`
`sudo tcpdump -i eth0 -c 10 net <IP>`
`sudo tcpdump -i eth0 -c 10 dst port 443` 
`sudo tcpdump -i eth0 -c 10 dst portrange 1-1023`
`sudo tcpdump -i eth0 -c 10 ip6 -w ip6.pcap`
`sudo tcpdump -i eth0 -c 10 'src <IP> and {dst port 80 or 443}'`

#### netstat, nbtstat, and arp

`netstat`
Shows TCP connections

`netstat -b`
`netstat -o`
`netstat -a`
`netstat -es`: statistics
`netstat -rn`: MAC addresses

---
`arp -a` : maps MAC addresses with IP addresses
`arp -s <IP> aa-bb-cc-dd-ee-f0`: adds to the table

#### Scripting with PowerShell

`Get-Verb`
(Get-Verb).count

`help pushd`

Windows PowerShell comes with ISE (instead of coding in notepad)

`echo` = `Write-Host`
`ls` = `dir`
`cat` = `type`

Add variables:
`$name = 'Malcolm`

If-Then commands:
`$>if ($nlist[1] -gt 0)`
`$>{`
`$>echo 'Positive'`
`$>}`
`Positive`

ForEach clause
`$> ForEach ($val in $nlist)`
`$> { echo "value is $val"`
`$> }`

#### PowerShell + Nishang
`Get-Passhashes`
`Invoke-PortScan -startaddress 10.0.0.21 -endaddress 10.0.2.8 -ScanPort`
`Invoke-BruteForce -startaddress 10.0.0.8 -service FTP -userlist users.txt -passwordlist passes.txt`
`Invoke-Prasdhak`: requires API key for [VirusTotal - Home](https://www.virustotal.com/gui/home/upload)

---

## Active Directory Domain Systems

##### Active Directory Hierarchy
```
Enterprise Realm
       |
     Forest
       |
	 Domain
	   |
	Subdomain
	   |
   Sub-Subdomain
```

#### Tool: dmitry
`dmitry yahoo.com`

##### Domain Controller View
```
    Domain
      |
    Site
      |
 Users,Devices
```

#### Tool: BloodHound

**BloodHound** is an open-source tool used for **Active Directory (AD) enumeration** and **privilege escalation**. It helps security professionals identify vulnerabilities in Active Directory environments that can lead to an attacker gaining elevated privileges, potentially compromising the entire domain.

---

Resources:
- [GitHub - swisskyrepo/PayloadsAllTheThings: A list of useful payloads and bypass for Web Application Security and Pentest/CTF](https://github.com/swisskyrepo/PayloadsAllTheThings)
- [What is cross-site scripting (XSS) and how to prevent it? | Web Security Academy](https://portswigger.net/web-security/cross-site-scripting)
- [What is CSRF (Cross-site request forgery)? Tutorial & Examples | Web Security Academy](https://portswigger.net/web-security/csrf#how-does-csrf-work)