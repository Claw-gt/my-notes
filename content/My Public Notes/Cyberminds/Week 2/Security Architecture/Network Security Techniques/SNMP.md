Automate routine network monitoring anad management tasks
**SNMPv3**
## Components

```mermaid
flowchart TD
subgraph normal
Administrator --GetRequest --> Agent
Agent --Response --> Administrator
Administrator --SetRequest--> Agent
end

```
Agent --SNMP Trap--> Administrator


Agent --SNMP Trap --> Administrator