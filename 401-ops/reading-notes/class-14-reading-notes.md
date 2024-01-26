# Class 14 Reading Assignment

## Intrusion Detection and Prevention Systems (IDS/IPS)

- The Pros and Cons of Network Intrusion Detection Systems ([article](https://www.rapid7.com/blog/post/2017/01/11/the-pros-cons-of-intrusion-detection-systems/))

## Questions

1. **List 2 differences between firewalls and an IDS?**
    - A firewall is there to block and keep out malicious attacks, an IDS (Intrusion Detection System) identifies incidents and *potential* threats through notifying sysadmins about suspicious and nefarious behaviors. (Such as a threat actor doing reconnaissance with nmap)
    - Firewalls focus specific on inbound and outbound traffic but an IDS can detect a lot more:
      - Keyloggers
      - Spyware
      - Accidental information leakage
      - Security policy violations
      - Configuration errors
    - Due to the focus on *detection*, an IDS can help inform what a firewall needs to be configured against.

2. **Under what circumstances would you choose a network-based IDS over a host-based IDS?**
    - Host-based IDS need software loaded and managed at different hosts on a network while a network does not care about operating systems and can monitor more than just computers but also routers, switches, etc. Due to this they have lower cost of setup and maintenance. It can also pick up on attacks that HIDS miss as NIDS are able to read packet headers in real-time. A large network will almost certainly need a network-based IDS.

3. **Name 3 major drawbacks of a NIDS?**
    - They cannot prevent incidents by themselves. NIDS can only help detection, so a process needs to be in place for what to do when the alarm goes up and a well trained staff who know how to react appropriately.
    - Encrypted packets can be used to slip past IDS since an IDS can't look inside them. This leads an IDS to only detect threat actors when they are already on the network.
    - False positives are frequently an issue with IDS -- maybe more frequently than actual threats! -- so engineers are needed to tune the IDS and monitor the alerts to determien if an alarm is false or the genuine article.

## Additional Resources

Network Intrusion Detection and Prevention - CompTIA Security+ SY0-501 - 2.1 (Professor Messer) [video](https://www.youtube.com/watch?v=hEgWPWIuq_s&ab_channel=ProfessorMesser)
