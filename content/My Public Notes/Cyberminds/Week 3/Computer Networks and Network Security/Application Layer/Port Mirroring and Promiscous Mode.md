
# Port Mirroring

>[!info] Helps to analyze data and detect network errors

A switch helps to make a copy of traffic updates on ports and sends it to a designated monitoring port (*SPAN port*)
A Cisco switch is called a Switch Port Analyzer (SPAN)
Remote Switch Port Analyzer (RSPAN) allows remote (not on the same switch) destination ports

> [!warning] Attackers can use port mirroring to exploit networks
> IDS analyzes the mirrored traffic

## Intrusion Detection Systems (IDS)
Can be connected to the monitoring port
Help to:
- Analyze destination ports
- Monitor real-time traffic to detect anomalies
--> Sends out alerts when a threat is detected

>[!warning] IDS can analyze defects, but takes no action


# Promiscous Mode

The endpoint or server being fed the mirrored data must have a [[Computer Networks#^9bda1d|NIC]] (*Network Interface Card*) running **promiscuously** to read all the frames it receives. (see [[Packet Sniffing#^58f278|Promiscuous mode]])
These framse have all the **destination MAC addresses**
Wireshark helps put NIC in promiscuous mode

>[!info] NIC, not in promiscuous mode, would ignore the frames

>[!important] For an IDS or other network analysis tool to work, it must have a NIC configured in promiscuous mode to read all the frames sent to its incoming port

