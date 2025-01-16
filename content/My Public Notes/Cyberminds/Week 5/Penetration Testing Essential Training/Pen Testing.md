## Cyber Defense Spectrum

**Vulnerability Scanning** (such as Nessus) + **Pen Testing** (such as zero-day vulnerabilities) + **Red Teaming** + **Cyber Hunter** (search for indicators of compromise)

## Cyber Kill Chain

- **Reconnaissance** (IP address, port scan, identify vectos for attacks, checking software versions)
- **Weaponization** (Customize a vulnerability to a target)
- **Delivery** (Email attachment, compromised website, log in to the target, flash drive, internet-exposed vulnerability)
- **Exploitation** (exploit a vulnerability, unauthrized use of credentials, unaware execution of malware)
- **Installation** (install payload into memory or disk, execute payload after system restart, provides ongoing access)
- **Command and Control** (connect to the commands and control server, receive commands, determine the command)
- **Action** 

## MITRE ATT&CK

The MITRE ATT&CK Model is a framework that describes the techniques and tactics used in cyberattacks. It plays a critical role in mitigating phishing attacks by identifying and preventing them at various attack stages. This model helps organizations identify and defend against cyberthreats by mapping attack methods and strategies.

### **Use case scenario**

Consider a scenario where a large corporate organization is targeted by a sophisticated phishing email designed to access sensitive employee data. The organization's security team, well-versed in the Cyber Kill Chain framework, is prepared to respond at each stage of the attack.

The following are the various attack stages:

1. **Reconnaissance:** The attacker gathers information about employees and scripts the phishing email to deceive a specific target like the human resource (HR) manager.
2. **Weaponization:** The attacker crafts an email containing a malicious attachment camouflaged as a legitimate document, like an updated employee benefits file.
3. **Delivery:** The HR manager receives the phishing email and unknowingly clicks the attachment, triggering the attack.
4. **Exploitation:** The attachment executes hidden malware that exploits a known vulnerability in the HR manager's email client, granting the attacker initial access to the system.
5. **Installation:** The malware installs additional components that create a backdoor, allowing the attacker persistent access to the system.
6. **Command and control (C2):** The attacker uses the installed backdoor to establish a communication channel, sending commands to extract sensitive data from the HR files.
7. **Actions on objectives:** The attacker downloads sensitive employee data for further exploitation.

The security team can intervene and respond at any stage in the attack. For instance, in the delivery phase, email filtering can block suspicious activities and phishing attempts before they reach the HR manager. If the email is delivered, the exploitation stage can be disrupted through endpoint detection and response (EDR) solutions, which monitor for unusual behavior after execution. By blocking or isolating the compromised system, the organization mitigates the risk of data theft and protects the integrity of sensitive data.

## Diamond Model of Intrusion Analysis

The Diamond Model of Intrusion Analysis examines cybersecurity incidents by analyzing the relationship between the four critical elements involved in an intrusion: adversary, infrastructure, capability, and victim. The model helps identify, investigate, and mitigate cyberthreats by understanding these interconnections. Organizations primarily use this model to understand how these elements influence the execution of attacks and better address cyber intrusions.

### **Use case scenario**

Consider a mid-sized financial services organization that becomes the target of a sophisticated ransomware attack. The security team uses the Diamond Model of Intrusion Analysis to understand and mitigate the threat.

Let's first discuss the four elements of the diamond model.

- **Adversary:** Threat actors are known cybercrime groups that target financial institutions for profit. They use advanced techniques and malware to break into networks, focusing on weaknesses through phishing emails and remote desktop protocol (RDP) vulnerabilities.
- **Infrastructure:** The attackers operate from compromised servers and a C2 system used in previous attacks. They conceal their location using virtual private networks (VPNs) and Tor networks, making it difficult to trace their activities. However, the security team can analyze network patterns to identify potential defense points.
- **Capability:** The attackers' ransomware features strong encryption, which can disable security systems. It tricks employees into downloading harmful attachments disguised as legitimate documents. To combat this, the organization enhances employee cybersecurity training and uses advanced tools to detect and block such threats.
- **Victim:** The targeted financial company has sensitive client data and proprietary information. However, vulnerabilities like outdated software and poor network segmentation have been identified. To improve defense against future attacks, the cybersecurity team will implement multifactor authentication (MFA), conduct regular software updates, and establish robust backup solutions.

### **Relationship between elements**

- **Adversary–Victim:** The cybercriminal group targets the financial firm for its valuable client data, aiming for ransom payouts. Understanding this helps the firm boost its defenses against potential attacks.
- **Adversary–Infrastructure:** The ransomware spreads through emails from a compromised but legitimate-seeming domain. The company can block harmful messages by monitoring incoming traffic and using advanced filters.
- **Victim–Infrastructure:** Attackers exploit weak remote desktop settings to access internal systems. Regularly auditing system configurations and monitoring for unusual access can significantly lower this risk.
- **Victim–Capability:** The company enhances cybersecurity using Security Information and Event Management (SIEM) systems for real-time analysis and alerts about the attackers' tactics. Knowing the ransomware's capabilities helps the firm strengthen defenses and reduce future attack impacts.

This case illustrates how applying the Diamond Model of Intrusion Analysis offers valuable insights, enabling the financial services organization to enhance its cybersecurity framework and better defend against ransomware threats.

## **Summary**

In this reading, you learned how the MITRE ATT&CK Model and the Diamond Model of Intrusion Analysis identify and mitigate cyberthreats.