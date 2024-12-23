## Defintion

see [[Threats that target Human Side Security|Social Engineering]]

-> Exploits factor of human psychology: **Greed** and **Fear**

## Social Engineering Types


| Social Engineering Type | Description                                                                                                                                                                                                                                            |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Phising                 | Attacker mass distribute emails in order to steal credentials                                                                                                                                                                                          |
| Spear Phising           | Targeted version of phising. Personalized emails                                                                                                                                                                                                       |
| Whaling                 | Form of spear phising that targets CEOs or CFOs ("big fishes")                                                                                                                                                                                         |
| Vishing                 | Voice Phising uses phone calls instead of emails                                                                                                                                                                                                       |
| Tailgating              | Physical scurity breach. Attacker exploits a moment when a controlled entry point is opened by an authorized individual                                                                                                                                |
| Impersonation           | Attacker adopts false identity                                                                                                                                                                                                                         |
| Dumpster diving         | Involves searching through and individual's or company's discarded items for valuable data                                                                                                                                                             |
| Shoulder surfing        | Observing a person's private information (such as passwords) by peering over their shoulder                                                                                                                                                            |
| Hoax                    | Distribution of false alarms or misinformation to deceive, create panic or manipulate individuals. Incite users to install unnecessary software of perform certain actions                                                                             |
| Watering hole attack    | Lying in wait at locations frequently visited by the target. Attackers identify and compromise websites taht are popular with their victims. They potentially exploit vulnerabilities witin the site's security or infect it through indirect methods. |

## Variations

#### Credentials Attack

1. Gather information (intelligence) -> Google, Linkedin, Facebook...
	in order to do a **Spear Phising** attack (personalized)
2. Use information gathered to write a ''legitimate'' email where there is a link to put on their credentials
3. The user logs with their credentials -> ⚠ STOLEN

--> Use of **greed**

##### Solution
- Secure DNS (**QUAD9**)
	change DNS in the browser or IP stack to *9.9.9.9*
	will look in its blacklist for the website
- User education
- Critical Thinking
#### Control Attack

1. Gather information (intelligence) -> Google, Linkedin, Facebook...
	in order to do a **Hoax** attack (personalized)
2. Call the user and tells them there is malware on their computer and gives them instruction in order to download a ''sanitizer'' software
3. The user downloads the software -> ⚠ RAT (*Remote Acess Trojan*)
4. The attacker has complete access to the system

 --> Use of **fear**
##### Solution
- Secure DNS (**QUAD9**)
	change DNS in the browser or IP stack to *9.9.9.9*
	will look in its blacklist for the website
- User education
- Critical Thinking
- MFA

#### Intellectual Property Attack

1. Gather information (intelligence) -> Google, Linkedin, Facebook...
	in order to do a **Impersonation** attack (personalized)
2. Retrieves videos of conferences, presentation that the user had done and  gives it to a Deep Fake Generator
3. Deep Fake creates an audio with the user's voice. The attacker calls another person and when it goes to the voicemail (call afterhours, lunch or use specialized software), the audio generated is played
4. This audio (impersonating the user) urges the person to send sensitive information to the attacker's email

##### Solution
- User education
- Critical Thinking
- Call the person back
- Do not send sensitive information

