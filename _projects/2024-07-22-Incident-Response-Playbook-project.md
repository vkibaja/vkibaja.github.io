---
title: 'Incident Response Playbook'
subtitle: 'A Project at Northeastern University'
date: 2024-07-22 00:00:00
description: This is a project where I acted as an Incident Response Manager and created Incident Response Playbook.
featured_image: '/images/demo/Incident-Response.jpg'
---

![](/images/demo/demo-landscape.jpg)

[Incident Response Playbook](assets/Incidence_Response_Playbook_VK.pdf)

### Incident Response Playbook Summary

As part of my role as the Incident Response Manager at "Viva la Vita Online," an online store specializing in vitamins and food supplements, I developed a comprehensive Incident Response Playbook to address various cybersecurity incident scenarios. This project was crucial for ensuring that our organization can systematically and effectively respond to potential security threats.

#### Background
The Incident Response Playbook for "Viva la Vita Online" outlines specific procedures to handle cyber incidents. It identifies the Cyber Incident Response Team (CIRT) members and their roles, detailing their responsibilities during an incident. The playbook includes detection, response, and recovery processes for various scenarios, ensuring the organization is well-prepared for potential threats.

#### Security Controls
Our security infrastructure includes several critical controls:
- **Network Controls:** Perimeter Firewalls, Intrusion Prevention Sensors, Email Gateway with Anti-malware and Anti-Spam Protection, and a Security Information and Event Management (SIEM) system.
- **Host Controls:** Anti-malware Endpoint Protection and Full Disk Encryption on employee laptops.
- **Other Controls:** A Vulnerability Patching program with a 30-day SLA.

#### CSIRT Composition
The CSIRT is composed of the following roles:
- **Incident Response Manager:** Directs the CSIRT team.
- **Security Analyst:** Supports the CSIRT Manager in coordination tasks.
- **CISO:** Maintains the company's information security vision.
- **CIO/CTO:** Maintains the company's information technology vision.
- **Technology and Operations Team Lead:** Has comprehensive knowledge of IT infrastructure and operations.
- **Senior Management:** Highest management level of the company.
- **Business Line Heads of Departments:** Direct and maintain business strategy.
- **Human Resources:** Manages the employee lifecycle.
- **Legal/General Counsel:** Provides legal advice.
- **Public Relations Officer:** Manages public relations.

#### General Incident Response Plan
The general incident response plan includes the following steps:
1. **Prepare:** Initial preparatory measures to ensure readiness.
2. **Detect:** Early detection methods to identify incidents promptly.
3. **Analyze:** Conduct investigations to understand the incident's scope and impact.
4. **Contain and Eradicate:** Contain the incident to prevent further damage and eradicate the threat.
5. **Recover:** Implement recovery plans to restore normal operations.
6. **Post-Incident Handling:** Review and update the incident response plan, applying lessons learned.

#### Incident Scenarios
For this project, I developed detailed playbooks for the following scenarios:

1. **Unauthorized Attempt to Access Payroll Records:**
   - **Detection and Notification:** SIEM logs detect unauthorized access attempts from the account "j.saw."
   - **Analysis:** Investigate account activity, identify the source of the social engineering attack, and assess any data accessed.
   - **Containment:** Change the password for the compromised account.
   - **Eradication:** Implement measures to prevent further social engineering attacks.
   - **Recovery:** Secure compromised accounts and reinforce access controls.

2. **SQL Injection Vulnerability:**
   - **Detection and Notification:** Regular database audit detects insecure code in SQL queries.
   - **Analysis:** Identify the developers of the code and assess whether the vulnerability has been exploited.
   - **Containment:** Deactivate vulnerable code immediately.
   - **Eradication:** Change the code to prevent SQL injection and enhance database security.
   - **Recovery:** Ensure proper backup and strengthen security measures.

3. **Blacklisted IP in VPN Connections:**
   - **Detection and Notification:** Intrusion prevention system flags an inbound connection from a blacklisted IP using the "j.saw" account.
   - **Analysis:** Investigate the IP address and account activity, assess the extent of access and damage.
   - **Containment:** Block the account and IP address immediately.
   - **Eradication:** Implement measures to prevent further unauthorized access.
   - **Recovery:** Restore affected files and verify system integrity.

This Incident Response Playbook ensures that "Viva la Vita Online" is prepared to respond effectively to various cybersecurity incidents, enhancing our overall security posture and resilience.

[Incident Response Playbook](assets/Incidence_Response_Playbook_VK.pdf)
 
Provided written guidance for detecting, responding, and recovering from each of the three incidents.

[Sample PDF](assets/Incidence_Response_Playbook_VK.pdf){:target="_blank"}

<a href="https://assets/Incidence_Response_Playbook_VK.pdf" target="_blank">Sample HTML PDF</a>


