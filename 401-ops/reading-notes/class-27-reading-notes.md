# Class 27 Reading Assignment

## Persistence  
PowerShell Empire No Longer Maintained - ([article](https://www.bleepingcomputer.com/news/security/powershell-empire-framework-is-no-longer-maintained/))

## Questions

1. **What is one of the major advantages of PowerShell Empire?**
    - Lightweight and extensible, allowing for modular development, perfectly dovetailing with the Weaponization (Phase 2) of the Cyber Kill Chain, where attackers find and customize their attack and payloads.
2. **What are some of the APT groups that have been known to use PS Empire and into which step of the Cyber Kill Chain does the use of PS Empire fall?**
    - APT group _Hades_ used Empire in it's "Olympic Destroyer" campaign during 2018 Winter Olymptics in South Korea.
    - Cybercrime group _FIN7_ also utilized it. 
    - Once deployed, _PowerShell Empire_ is used in the Phase 6 of the Kill Chain: Command and Control (C2)
3. **What are the four main components needed to pull off an attack using PS Empire?**
    - **Listener**: the listener is a process which listens for a connection from the machine that is being attacked. This helps Empire send the loot back to the attacker’s computer.
    - **Stager:** A stager is a snippet of code that allows malicious code to be run via the agent on the compromised host.
    - **Agent:** An agent is a program that maintains a connection between the attacker's computer and the compromised host.
    - **Module:** These are what execute malicious commands, which can harvest credentials and escalate privileges as mentioned above.


## Additional Resources
Hacking with Empire ([article](https://www.hackingarticles.in/hacking-with-empire-powershell-post-exploitation-agent/))

