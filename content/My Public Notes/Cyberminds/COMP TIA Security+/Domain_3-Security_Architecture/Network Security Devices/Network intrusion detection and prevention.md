
IDS and IPS

# Intrusion Detection Systems (IDS)

Monitor network traffic for signs of malicious activity
Alert administrator of suspicious activity
👎Require someone to monitor and take appropriate action
# Intrusion Prevention Systems (IPS)

Block malicious activity **automatically**

**Deployment modes**:
- Inline (active) deployment: sits in the path of network communciations, block suspicious traffic from entering the network. It can disrupt all network communication since inline IPS is a single point of failure
- Out-of-band (passive) deployment : connects to SPAN or TAP port on switch, which allows to receive copies of all traffic sent through the netwrok to scan. It cannot disrupt the flow of traffic. Can react **after** suspicious traffic enters the network
## False Positive Error
IDS/IPS triggers an alert when an attack did not actually take place
## False Negative Error
IDS/IPS failts to trigger an alert when an actual attack occurs

---
# Technologies used by IDS and IPS
## Signature Detection Systems

- Contain databases with rules describing malicious activity
- Alert admins to traffic matching signatures
- Fail to detect brand new attacks

## Anomaly Detection Systems

- Deviation from "normal" activity trends
- Detect previously unknow attacks
- Increased false positive rates
- aka **Heuristic detection** and **behaviour-based detection**

