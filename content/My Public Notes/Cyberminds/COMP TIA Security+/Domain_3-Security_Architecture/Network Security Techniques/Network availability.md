Maintaing network availabiloty is a crucial security goal
## Flooding attacks
Overwhelm network devices

**SYN floods**
Fill connection state tables on firewalls with half-open connection entries

**MAC floods**
Fill switch's MAC address table with many entries, causing it to flood traffic on all ports

Solution => **Flood Guard Technology**
=> **Port security** is also effective against MAC flooding
## Routing Loops
Allow broadcast storms

Solution => **Spanning Tree Protocol (STP)** : prevents broadcast storms by implementing loop prevention, prevents logical connections
STP uses routing status messages called **BDPU (*Bridge Protocol Data Units*)**. To avoid BDPU spoofing and malicious STP protocol => BDPU Guard


