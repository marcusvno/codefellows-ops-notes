# Class 13 - Threat Taxonomy

**Threat taxonomy** is a classification system used to categorize and organize various types of security threats, vulnerabilities, and risks.

- **Tactics, techniques, and procedures (TTP)s** are "patterns of activities or methods associated with a specific threat actor or group of threat actors"
  - Typically the Modus Operandi of these cyber threat actors.
  - From a defensive point of view, identifying the patterns makes it easier to stop them from being successful and anticipating their next actions.
    - This idea has some similarities with the _Cyber Kill Chain_.
  - One of the global repositories of known TTPs is maintained by **MITRE** and is known as the **MITRE ATT&CK Matrix** (or Framework).
    - A shared security knowledge base. Massive collection of data.

- The order of **Tactics, Techniques, Procedures** is important as the list is hierarchical.
  - Tactics - Category.
    - Techniques - Subcategory.
      - Procedures - Detailed items.

## MITRE Attack Framework

- A knowledge base of adversary behavior
  - Based on real-world observations
  - Free and open
  - Common language for security professionals
  - Community-driven
- Used for developing threat models and methodologies.

![mitre](https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-13/slides/assets/13_02.png)

### Tactics in a Cyberattack

The **MITRE Attack Framework** defines the following tactics used in a cyberattack:

- **TA0001:** Initial Access
- **TA0002:** Execution
- **TA0003:** Persistence
- **TA0004:** Privilege Escalation
- **TA0005:** Defense Evasion
- **TA0006:** Credential Access
- **TA0007:** Discovery
- **TA0008:** Lateral Movement
- **TA0009:** Collection
- **TA0010:** Exfiltration
- **TA0011:** Command and Control (C2)

(NOTE: "Tactics" are high level categories that contains _techniques_. "Techniques" can contain _sub-techniques._)

Example:

- **TA0001: Initial Access -** The adversary is trying to get into your network.
  - **T1566 Phishing -** Adversaries may send phishing messages to gain access to victim systems.
    - **.001: Spearphishing Attachments -** Adversaries may send spearphishing emails with a malicious attachment in an attempt to gain access to victim systems.
      - **TA0001:T1566.001**



