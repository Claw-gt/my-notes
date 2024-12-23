
IDS and IPS

# Intrusion Detection Systems (IDS)

Alert administrator of suspicious activity
👎Require someone to monitor and take appropriate action
# Intrusion Prevention Systems (IPS)

Block malicious activity **automatically**

**Deployment modes**:
- Inline (active) deployment: sits in the path of network communciations, block suspicious traffic from enterignthe networkd
- Out-of-band (passive) deployment : connects to SPAN or TAP port on switch, can react **after**
## False Positive Error

## False Negative Error

---

# Signature Detection Systems

- Contains databases with rules describing malicious activity
- Alert admins to traffic matching signatures
- Fail to detect brand new attacks

# Anomaly Detection Systems

- Deviation form "normal" activity trends
- aka **Heuristic detection** and **behaviour detection**