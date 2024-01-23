# Class 11

## SOC Concepts

- **Security Operations Center (SOC)**

  - A central team that monitors security infrastructure
  - The SOC team is responsible for monitoring, detecting ,responding to, and mitigating security threats and incidents.

- A **security incident** is an event or series of events that compromise the confidentiality, integrity, or availability, of an organization's informaton, systems, or network.
- **Incident Response (IR)** is the process by which an organization handles a data breach, cyber attack, or leak. Includes remediation and post-event action.

- **Threat hunters**, however, do not perform the full IR lifecycle and instead focus on identification and detection.

<center><img src="https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-11/slides/assets/11_06.png"/></center>

## SOC Tools

- SIEM - Security Information and Event Management
- EDR
- XDR
- IDS
- IPS
- Firewalls
- Vulnerability Scanners
- Investigation Tools
- Vulnerability Feeds and DB
- Ticketing Solutions

- SIEMs are about **log aggregation**
  - Security Information and Event Management (SIEM) is software that aggegates and analyzes activity from many different resources in your IT infrastructure
    - Examples:
      - Splunk (commercial)
      - Elastic/ELK Stack (open source)
    - Performs:
      - Event and log collection
      - Normalization
      - Correlation
      - Adaptability (scalable)
      - Reporting and alerting
      - Log management
      - Layered centric views

## Splunk Concepts

- **What is Splunk?**

  - A widely used software designed for searching, analyzing, and visualizing machine-generated data in real-time.
  - Primarily used for log and event data management and is especially valuable for monitoring the security of IT systems.

- Splink uses a **Search Processing Language** (SPL), similar to **SQL**.
  - Designed specifically for querying and analyzing data and filter large volumes of data.
  - Syntax orginally based on the Unix pipeline and SQL.
- **SPL scope:**
  - Data searching
  - Filtering
  - Modification
  - Manipulation
  - Insertion

<center><img src="https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-11/slides/assets/11_07.png"/ width=500px></center>

### Stages of SIEM Data Pipeline in Splunk

- **Stage 1: Data Input**
  - Data accessed from the source and turned into 64k blocks.
- **Stage 2: Data Storage**
  - Parsing Phase
    - Splunk examines, analyzes, and transforms the data.
  - Indexing Phase
    - Splunk writes parsed events to the index queue.
    - Individual indexes are created as objects in Splunk, and you define what scope of data gets monitored and goes into each index.
- **Stage 3: Data Searching**
  - How data is accessed, used, and viewed is controlled.

<center><img src="https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-11/slides/assets/11_09.png" style="background-color: white;" width=800px></center>

### Splunk Architecture

Splunk indexes are repository for data.

- Indexes reside in flat files on the indexer, which transforms raw data into searchable vents.

- Class 11's Lab VM comes preloaded with three indexes that are data-populated:
  - default
  - botsv1
  - mordor
