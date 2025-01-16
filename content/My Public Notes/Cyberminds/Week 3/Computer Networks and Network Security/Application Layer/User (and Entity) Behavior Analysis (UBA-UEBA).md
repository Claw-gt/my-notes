# User Behaviour Analysis

--> Adds an extra layer of security
--> Focuses on internal activities
--> Detects suspicious behaviour early
--> Mitigates threats proactively

#### Baselining normal behavior

- Establish normal behavior patterns
- Monitor typical activities
- Flag deviations

#### Anomaly detection

- Identifies deviations from the baseline
- Detects potential threats
- Triggers alerts

#### Contextual awareness

- Analyzing user roles and activities
- Consider activity context
- Accurately interpret behavior

### Techniques and tools

#### Machine learning algorithms
- Learning and updating behavior patterns
- Enhancing anomaly detection accuracy
- Predicting potential threats based on historical data

#### Statistical analysis
- Quantify deviations from normal bahavior
- Techniques: 
	- **Standard deviation**
	- **Correlation analysis**
	- **Regression models**

#### Log analysis
- Analyze access logs, application logs, network logs
- Aggregating and correlating data to identify patterns and anomalies


----

**Integrating UBA with SIEM systems** --> Centralized view of security events

# User and Entity Behaviour Analysis

### **User and entity behavior analytics**

User and entity behavior analytics (UEBA) is a security software solution that uses behavioral analysis, machine learning (ML), and automation to detect unusual and potentially dangerous actions from users and devices. The main difference between UEBA and UBA lies in their focus: UBA only monitors the behavior patterns of end users, whereas UEBA extends its monitoring to include non-user entities like servers, routers, and Internet of Things (IoT) devices, detecting any unusual behavior or suspicious activity that could signal a security threat. UEBA solutions collect and analyze large amounts of data from various sources to understand the expected behavior of privileged users and entities.

Over time, as the system learns from this data, it requires fewer examples of typical behavior to maintain accuracy, thereby enhancing UEBA's security insights and supporting zero-trust security strategies. Once normal behavior is established, UEBA uses advanced analytics and ML to monitor current activities and identify unusual actions in real time.

### **Enhancing the effectiveness of UEBA**

UEBA's effectiveness increases by examining data from a wide range of sources, including:

- Network hardware like firewalls, routers, virtual private networks (VPNs), and Identity Access Management (IAM) systems
- Security tools like antivirus programs, Endpoint Detection and Response (EDR) systems, and Security Information and Event Management (SIEM) solutions
- Authentication repositories like Active Directory (AD) that store vital information about user accounts and network activities
- Threat intelligence sources and frameworks like MITRE ATT&CK that provide insights into common cyber threats, such as malware and security vulnerabilities
- Enterprise resource planning (ERP) and human resources (HR) systems that monitor potential security risks, such as former employees and disgruntled staff

### **UEBA scoring system**

UEBA uses the insights from analyzing user behaviors to detect unusual activities and assign risk scores. For example, multiple failed login attempts in a short time may signal a low-risk alert for a potential insider threat. In contrast, if a user connects several USB drives and downloads unusual amounts of data, it could indicate data theft, leading to a higher risk score. This scoring system helps security teams focus on the most significant threats while filtering out false alarms. Additionally, it allows for tracking lower-level alerts over time, which may indicate a severe, developing threat.

### **UEBA use cases**

UEBA enhances organizational security through various tactical and strategic applications. The tactical applications focus on immediate, operational security measures organizations can implement to detect and respond to threats. These applications leverage real-time data analysis to identify anomalies that may indicate a security breach or insider threat.

In contrast, the strategic applications focus on long-term security posture and organizational resilience. They leverage historical data trends and comprehensive behavioral analysis to inform broader security strategies.

Let's explore a few tactical and strategic use cases.

### **Tactical use cases**

- **Malicious insiders:** Individuals with privileged access can pose significant threats through cyberattacks. Traditional methods, such as log analysis, may overlook these threats. However, UEBA analyzes user behavior rather than just IP addresses, enabling better detection of those violating security rules.
- **Compromised insiders:** Attackers can obtain legitimate user credentials through phishing or brute-force methods, blending in with normal operations. UEBA helps identify unusual behaviors as these attackers navigate the network, enabling quick responses to potential breaches.
- **Compromised entities:** Several industries, particularly manufacturing and healthcare, use Internet of Things (IoT) devices that may not be well-secured, making them attractive targets for hackers. UEBA helps detect irregular activities that suggest a device may be compromised, enabling prompt action to mitigate potential threats.
- **Data exfiltration:** Insider threats and external attackers primarily target sensitive data. UEBA allows security teams to monitor and identify unusual patterns in data access or downloads in real time, enabling immediate action against potential data breaches.

### **Strategic use cases**

- **Implementing zero-trust security:** This approach requires continuous verification of all users and entities, regardless of their location. UEBA plays a crucial role by providing comprehensive visibility into user activity, ensuring that authentication and authorization processes are strictly followed.
- **General Data Protection Regulation (GDPR) compliance:** GDPR mandates strict control over personal data access and use. UEBA solutions help organizations track user interactions with sensitive data. They facilitate compliance by ensuring adherence to necessary data handling practices as required by the regulation.