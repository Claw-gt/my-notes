# Selecting your methodology

## Risk Assessments
### NIST
SP 800-30 Revision 1
*Guide for Conducting Risk Assessments*

### FAIR
Factor Analysis of Information Risk
Quantitive approach

## Security Control Assessments
### NIST
SP 800-53 Revision 5
*Security and Privacy Controls for Information Systems and Organizations*
### FAIR
ISO 27001:2022
Code of practice for information security controls

## Compliance Assessment
- Driven by data set
- Self-assess vs third party
- Frequency dictated by standard

#### PCI DSS
- Credit card data
- Accept, process, store and/or transmit
#### HIPAA
- Electronic protected health information (ePHI)
- Security Risk Assessment Tool (SRA Tool)

## Vulnerability Assessment

**Popular vulnerability scanners:**
- [Nessus](https://www.tenable.com/)
- [Qualys Cloud Platform](https://www.qualys.com/)
- [Nexpose](https://www.rapid7.com/)
- [OpenVAS](https://www.openvas.org/)

**Large Enterprise:**
- Veracode
- AppScan
- Sentinel
**Small Enterprise:**
- Acunetix
- Checkmarx
- Synopsys
**Free and Open Source:**
- Burp Suite
- OWASP ZAP

##### Authenticated vs. Unauthenticated scans
--> **Authenticated**
- Trusted insider
- Full visibility
- More likely to impact production
--> **Unauthorized**
- Unauthorized outsider
- Limited visibility
- Less likely to impact production

## Penetration Testing

**PTES**: Penetration Testing Execution Standard

**OSSTTM**: Open Source Security Testing Methodology Manual

##### Automated vs. Manual
--> **Automated**
--> **Manual**
- OWASP Testing project (web)
- CIS Benchmarks

---
# Basic assessment tools

#### Risk Assessment Tools
- Many manual processes
- Spreadsheets galore
- Tool: *SimpleRisk*
	Preconfigured machines
#### Security Control Assessment Tools
- Interviews with administrators
- Review of technical documentation
- Even more spreadsheet

For FISMA alignment --> *OpenFISMA*
For ISO2700 alignment --> *ISO27k Toolkit*

---
# Advanced Assessment Tools

#### Compliance Assessment
##### PCI
Self-Assessment Questionnaires (SAQs)
##### HIPAA
Security Risk Assessment Tool (SRA Tool)

*Note:* SecTools