Distribute work among servers

DNS Entry points to the Virtual IP address (load balancer address)
=> One Single Point of Failure

![[Cyberminds Academy/COMP TIA Security+/Domain_3-Security_Architecture/Network Security Devices/attachments/image 2.png]]

### Autoscaling
Automatically adds or removes servers, as needed

## Benefits
- SSL certificate management
- URL filtering
- Other web application security tasks

## Round-Robin Scheduling
Each server gets an equal number of requests
Load Balancer simply rotate servers for each request, giving each server an equal share
=> not always efficient
⚠ Advanced scheduling algorithms choose servers based upon performance and available capacity
## Session Persistence
Routes an individual user's requests to the same server => **Affinity for a specific server**


## Avoid OSPoF
### Active-Active
Two or more load balancers actively handle network traffic and continue to function with diminished capacity if one device fails
### Active-Passive
One load balancer handles all traffic while a second monitors activity and assumes responsibility if the primary load balancer fails

