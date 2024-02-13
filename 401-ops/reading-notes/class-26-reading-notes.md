# Class 26 Reading Assignment

## Readings: Remote Code Execution

- Cyber Threat Analyst: Key Job Skills and Expected Salary- ([article](https://www.spiceworks.com/it-security/vulnerability-management/articles/cyber-threat-analyst-key-jobs-and-salary/))
- Tracking, Detecting, and Thwarting PowerShell-based Malware and Attacks ([article](https://www.trendmicro.com/vinfo/us/security/news/cybercrime-and-digital-threats/tracking-detecting-and-thwarting-powershell-based-malware-and-attacks))

## Questions

1. **You just got a new job as a Cyber Threat Analyst, how would you explain your role to a family member?**
    - An analyst job is like a digital detective who tracks down threats, analyze weaknesses in the perimeter, monitor for security breaches, and help build defenses against outside threats.
2. **Explain what makes PowerShell such an effective attack vector.**
    - PowerShell interaction occurs through cmdlets, which are commands that enable actions on .NET objects, in turn allowing users direct access to the entire system. While we've developed defenses against delivery of malware through virus scans, blocking automated running of macros or downloading files from suspicious website without valid ceriticates, PowerShell remains an ideal way to circumvent all these safeguard by injecting payloads directly into running applications, or utilizing scripting,  due to it being a trusted application.
3. **What are two things you can do to mitigate attacks that leverage PowerShell?**
    - With the increase of living-off-the-land PowerShell attacks, sysadmins can utilize it's built-in logging tools to ensure that it isn't abused as an attack vecture.
      - PowerShell Log Inspection, for instance, can be used to decode when attackers use PowerShell encoding to obfuscate their commands.
    - Behavioral monitoring, specially by leveraging machine learning, can help us establish baseline patterns which can help detect when abnormal behavior even with normal and trusted tools like PowerShell. A user who never has use for PowerShell for a long time and suddenly starts utilizing it may be cause for concern. Couple this with other detection methods can determine when it an intruder may be trying to utilize PowerShell as a tool.