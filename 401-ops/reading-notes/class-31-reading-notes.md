# Class 31 Reading Assignment

## Malware Detection with YARA Rules 

- What Are YARA Rules? ([article](https://archerint.com/what-are-yara-rules/))
- Threat Hunting using YARA ([article](https://www.geeksforgeeks.org/threat-hunting-using-yara/))

## Questions

1. **What is the main goal of Threat Hunting and how is it different from traditional threat monitoring?**
    - Threat hunting is a proactive approach to identifying and mitigating cyber threats that have already entered an organization’s network. While traditional threat monitoring may depend on automated tools, alerts, and rules -- such as YARA rules, firewalls, and antivirus -- threat hunters are actively engaged in seeing what those tools may have missed. 
2. **What are the four types of YARA rules and what does each one of them use to identify and classify malicious software?**
    - **String-based Rules:** These rules use _strings of text_, either as literal values or as regular expressions, to identify malware.
      - **Example:** A string-based rule to detect malware that contains a spceific string of character in its code.
    - **File metadata-based rules:** These rules use _metadata_ about the files being analyzed to identify malware.
      - **Example:** A metadata rule to detect a particular file type or to identify files that have been created or modified withing a specific time period.
    - **Hash-based rules:** These rules use _cryptographic hashes_ to identigy malware. A cryptographic hash is a unique representation of the contents of a file, and if any part the file changes, so too does the hash. Hash-based rules can be used to detect malware that was hbeen modified or disguised in an attempt to evade detection.
    - **Network-based rules:** These rules use _network traffic data_ such as IP addresses or prots to ID malware. 
      - **Example:** A network-based rule to detect malware taht is communicating to a specific IP address or port. Such as 4444 for Metasploit!
3. **How are YARA rules similar to how Anti-Virus programs detect malicious software?**
    - Anti-virus programs use malware definitions to compare files to and detect any malware on a system. Similarly, YARA rules compare files to rules in a form similar to anti-virus's definitions. Both try to detect malware through behaviour (such as communicating on a particular port) or signatures (such as hash, filetype, or strings)

## Additional Resources

- YARA Rules GitHub Project ([article](https://github.com/Yara-Rules/rules))
  - This project covers the need of a group of IT Security Researchers to have a single repository where different Yara signatures are compiled, classified and kept as up to date as possible, and began as an open source community for collecting Yara rules.

