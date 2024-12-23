Distribute work among servers

DNS Entry points to the Virtual IP address (load balancer address)
--> One Single Point of Failure
### Autoscaling
Automatically adds or removes servers

## Benefits
- SSl certificate management
- URL filtering
- Other web application security tasks

## Round-Robin Scheduling
Each server gets an equal number of requests
--> not always efficient

## Session Persistence
Routes and individual user's requests to the same server


**Avoid OSPoF**
### Active-Active
Two or more load balancers actively handle network traffic and continue to function with diminished capacity if one device fails
### Active-Passive
One load balancer handles all traffic while a second monitors activity and assumes responsibility if the primary load balancer fails

