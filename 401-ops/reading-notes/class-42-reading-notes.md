# Class 42 Reading Assignment

## Pass the hash with Mimikatz  
- What is Mimikatz ([article](https://www.varonis.com/blog/what-is-mimikatz))

## Questions

1. **Name the six credential-gathering techniques which Mimikatz is able to perform and explain how two of them work.**
    - **Pass-the-Hash:** Attackers use Mimikatz to pass an exact hash string to log in to the target computer.
      - Windows used to store password data in an NTLM hash. Attackers use Mimikatz to pass that exact hash string to the target computer to log in. Attackers don’t even need to crack the password — they just need to use the hash string as-is. It’s the equivalent of finding the master key to a building on the lobby floor. You need just that one key to get into all the doors.
    - **Pass-the-Ticket:** Mimikatz provides functionality for a user to pass a Kerberos ticket to another computer and log in with that user's ticket.
      - Newer versions of Windows store password data in a construct called a ticket. Mimikatz provides functionality for a user to pass a Kerberos ticket to another computer and log in with that user’s ticket. It’s very similar to the pass-the-hash method.
    - **Overpass-the-hash:** Technique that passes a unique key obtained from a domain controller to impersonate a user.
    - **Kerberoast golden tickets:** A golden ticket gives you non-expiring domain admin credentials to any computer on the network.
      - This is a pass-the-ticket attack, but it’s a specific ticket for a hidden account called KRBTGT, which is the account that encrypts all of the other tickets. A golden ticket provides you with non-expiring domain admin credentials to any computer on the network.
    - **Kerberoast silver tickets:** Grants a user a TGS ticket that's used to log into any services on the network.
      - Another pass-the-ticket, but a silver ticket takes advantage of a feature in Windows that makes it easy for you to use services on the network. Kerberos grants a user a ticket-granting server (TGS) ticket, and a user can use that ticket to authentic to service accounts on the network. Microsoft doesn’t always check a TGS after it’s issued, so it’s easy to slip past any safeguards.
    - **Pass-the-cache:** Generally the same as a pass-the-ticket, but uses the saved and encrypted login data on a Mac/UNIX/Linux system.
1. **What are four ways we can defend against Mimikatz attacks. Explain how two of the mitigations can stop Mimikatz.**
    - **Restrict Admin privileges:** Limit admin privileges only to users that need them. If the attacker can't gain local admin privileges then they can't use Mimikatz to gain access to tickets or other files.
    - **Disable password-caching:** Windows caches password hashes that were recently used through their system registry. Mimikatz can then gain access to these cached passwords, which is why it’s important to change your default settings to cache zero recent passwords. 
      - This can be accessed through *Windows Settings > Local Policy > Security Options > Interactive Logon.*
    - **Turn off debugging privileges:** Windows default settings allow local admins to debug the system but Mimikatz can exploit this. Turning off debugging on machines is a best practice to safeguard your system and keeps Mimikatz for being able to exploit debugging privileges. 
    - **Increase local security authority:** 
      - Upgrading to Windows 10 can help mitigate the types of authentication attacks that Mimikatz enables. However, when this isn’t possible, [Microsoft has additional LSA configuration items](https://docs.microsoft.com/en-us/windows-server/security/credentials-protection-and-management/configuring-additional-lsa-protection) that help reduce the attack surface area. 