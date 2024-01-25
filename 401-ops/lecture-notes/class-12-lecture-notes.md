# Class 12 - Log Analysis with Splunk

## Outline

- APT Groups
- Website defacement
- **Cyber Kill Chain**
- Web Vulnerability Scanners
- OSINT
- Brute Force Attack
- Dynamic DNS (DDNS)
- Splunk commands

## Advanced Persistent Threats (APT)

- **Advanced Persistent Threat (APT)**
  - Employ advanced and sophisticated hacking techniques, tools, and tactics
  - Attackers maintain unauthorized access for extended periods of time.
  - Operate steathily, making detection challenging by disguising their activities.
  - Highly targeted, focusing on specific organizations, industries, or individuals
  - Many APTs are believed to have connections to nation-states, providing them with significant resources and sophistication.

Two organizations have developed naming conventions for APTs. However, these are clearly devised from a US or Western perspective.
  - Crowdstrike  https://www.crowdstrike.com/adversaries/
  - Mandiant https://www.mandiant.com/resources/insights/apt-groups


## Website Defacement

- Typically a form of activism.
- The attac

## CYBER KILL CHAIN

The **Cyber Kill Chain** is _CRITICAL KNOWLEDGE_, much like the **CIA Triad**.

- The **Cyber Kill Chain** is a security model outlining the sequential phases of a cyber attack, in order to make it harder for the attacker to be success. This is accomplished by knowing all the steps necessary for an attack to be successful and so that defenders can try and break that chain to prevent the success of the attack.
- Originally developed by Lockheed Martin.

![kill chain](https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-12/slides/assets/12_06.png)

### Overview

1. Reconnaissance
2. Weaponization
3. Delivery
4. Exploitation
5. Installation
6. Command and Control
7. Actions on Objectives

### Stages of the Lockheed Martin Cyber Kill Chain

1. **Reconnaissance**
    - Attackers try to gain as much information about your target as possible to identify weaknesses.
    - Cost-benefit analysis
    - Gathering information
      - Active information gathering.
        - Port scanning, etc.
        - Phishing
        - Social Engineering.
        - Anything that interacts with the target.
      - Passive information gathering.
        - OSINT
2. **Weaponization**
    - Threat actor develops malware payload designed to target newly-discovered vulnerabilities.
      - Leverages information discovered during _reconnaissance_.
    - Tools customized to target network
      - "What will work?"
      - "How will I develop it?"
      - "Can I source the weapon from the dark web? Or open source security research?"
      - "Can I tailor it to the target?"
3. **Delivery**
    - Malware payload delivered to target network or system
      - Ex: Spear phishing attack.
      - Targeted email with a malicious attachment
      - Tainted USB
      - Often utilizes some form of social engineering to facilitate delivery.
    - Exploit mismanaged or misconfigured servers.
4. **Exploitation**
    - Malware executed.
    - Discovered vulnerabilities exploited
    - Superuser access grated / privileges escalated to threat actor.
5. **Installation**
    - Malware embeds itself into the system.
    - Additional malware components are downloaded.
6. **Command and Control (C2)**
    - Management and communication established from attack to malware infection and compromised host.
    - Facilitates greater movement within target network.
7. **Actions on Objectives (End Goal)**
    - Mission-specific actions are finally taken to achieve original objectives.
      - Employ Ransomware, steal database, etc.

## Web Vulnerability Scanners

- Automated tools that scan web applications looking for security vulnerabilities
  - Cross-site scripting (XSS)
  - SQL injection
  - Cross-site request forgery (CSRF)

These tools are useful for defenders to test and find their own vulnerabilities but it can also be used by attackers to find your vulnerabilities.

- Example Products:
  - Burp Suite (by Portswigger)

Similar to nmap's "scanme.nmap.org", which invites people to test their port scanners, there exists Web Applications for testing Web Vulnerability Scanners such as ([OWASP's Juice Shop](https://owasp.org/www-project-juice-shop/))