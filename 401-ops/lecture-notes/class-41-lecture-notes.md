# Class 41 Lecture Notes: Penetration Testing

## Security Testing

Security Testing is **_NOT_** a penetration test. It is testing on software behaviour for security problems. Usually done by blue team defenders.

- Can involve bringing outdated systems up to date.
- Software security testing during Software Dev Life Cycle (SDLC)
- Maintaining of packages and systems.

## Vulnerability Testing 
Vulnerability testing is also not a penetration test. It's about finding and documentating vulnerabilities in a system or software and not about exploiting them. 
  - Vulnerability testers may find an exploit, see how far it can be used as an exploit, and document it. 

## Pentest Stages (Imperva Version)

Similar to the Lockheed Cyber Kill Chain.

### Phase 1: Planning & Reconnaissance

- Define scope and goals of tests.
- Gathering intelligence on target.

Pentesters perform recon against their target in order to gain more informatio about what their about to attack.

Types of recon:
  - Passive: 
    - OSINT, observing, sniffing, information gathering.
    - OSINT consists of publicly available information on the target.
    - Not interacting with the target.
  - Active: 
    - Interacting with the target and probing for weaknesses.

### Phase 2: Scanning

- How will a target application respond?
  - Static analysis
    - Examine the code and look for possible entry points.
  - Dynamic analysis
    - Interact with the application to see if we can get the network to act in ways it's not suppose to.
- Enumeration

### Phase 3: Gaining Access
  - Social Engineering
    - Phishing, etc.
  - Web App attacks
    - Public facing APIs / Applications / etc.

### Phase 4: Maintaining Access
  - Achieving persistence = APT
    - More work and requires cleanup. 
    - May also cost more.

### Phase 5: Analysis
  - Compile results of testing into reports
    - Vulnerabilities discovered and exploited
    - Sensitive data/systems accessed.
