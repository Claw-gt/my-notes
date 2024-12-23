
#### Bastion
⚠ Not recommended

```mermaid
flowchart LR
Internet --> Server --Firewall -->Intra
```

#### Tri-Homed
Buffer that sits in between a Not-Trusted Environment (Internet) and More-Trusted Environment (Intra)

```mermaid
flowchart LR
Internet --> Server(DMZ) --> Intra
Intra --> Server(DMZ)
Intra --> Internet
```
**DMZ**: Demilitarized Zone (*Semi-Trusted*) ^54c2b3

👍Scalable
👍Cheap

👎One Single Point of Failure (SPOF)
#### Basic DMZ

```mermaid
flowchart LR
Internet --Firewall --> Server --Firewall -->Intra
```

👍Defense in Depth
👍Scalable

👎Cost
👎Complex


#### Multi-Tiered DMZ

```mermaid
flowchart LR
Internet --Firewall --> WebServer --Firewall -->AdServer --Firewall -->DataBase
```

👍Defense in Depth
👍Granularity

👎Cost
👎Complex