SW -> Bugs
% -> Vulns
SW -> Vulns

**Dev**eloping Phase
**Op**eration Phase -> Public Release

**TRADITIONAL APPROACH** --> *Linear*
```mermaid
flowchart LR
subgraph DEV
Plan --> Code --> Test
end
subgraph OPS
Test --> Release
end
```
👎Slow
👎Inflexible

**DevOps APPROACH** --> *Cyclical* ^0140b8

```mermaid
flowchart TD
subgraph DEV
Plan --> Code
Code --> Build
Build --> Test
end
subgraph OPS
Test --> Release
Release --> Deploy
Deploy --> Operate
Operate --> Monitor
Monitor --> Plan
end
```
👎Integrated
👎Agile

--> **DevSecOps**

- Security Built-In
- Security by Design
- Collaboration
- Automation