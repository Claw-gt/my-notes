# Documentation Review

Security Documentation Flow
```mermaid
flowchart TD
Mobile_Policy --> Standard_iOS
Mobile_Policy --> Standard_Android
Standard_iOS -.-> Guidelines_iOS
Standard_Android -.-> Guidelines_Android
Guidelines_iOS -.-> Procedure_iPad
Standard_iOS --> Procedure_iPad
Standard_iOS --> Procedure_iPhone
Guidelines_Android -.-> Procedure_Phone
Guidelines_Android -.-> Procedure_Tablet
Standard_Android --> Procedure_Phone
Standard_Android --> Procedure_Tablet
```

# Log Management Tools

**Commercial tools:**
- Splunk
- QRadar
- LogRhythm
- AlienVault

**Free and open-source tools:**
- Syslog
- Syslog-ng
- Graylog
- Elasticsearch

Logging Cheat Sheet --> [*Critical Log review Checklist for Security Incidents*](https://zeltser.com/security-incident-log-review-checklist/)

# Ruleset Review

Test firewall rules by using `nmap` to scan por open network ports --> messy

--> Tool: *Nipper*

# System Configuration Review

- Lynis
- CIS-CAT

# File Integrity Checking

- Tripwire
- OSSEC