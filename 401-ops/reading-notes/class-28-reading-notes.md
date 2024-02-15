# Class 28 Reading Assignment

## Log Clearing

Ethical Hacking: Log Tampering 101 - ([article](https://resources.infosecinstitute.com/topics/hacking/ethical-hacking-log-tampering-101/))

## Questions

1. **Explain some specifics of why a hacker might want to clear log files to a family member. Do not use the example from the article.**
   - Every spy, crime, or detective movie has someone wipe a doorknob of a door to remove their fingerprints. Clearing logs is the hacker digital equivalent of wiping the doorknob on the way out.
2. **What are three methods by which you can clear logs in a Windows system?**
    - Clearlogs.exe
    - Meterpreter
    - Windows Event Viewer
3. **What are the four steps in the process of covering your tracks.**
   - _Disable auditing_
     - Disabling auditing means that there are no logs to erase.
     - On Windows systems, **Auditpol** command line tool can allow hackers to see the set logging level and then only act in ways that won't be tracked or disable logging level that would detect them but not others. For instance, if they would only get noticed by "Information" logs, they would leave all upper log levels enabled. This makes it more difficult to detect them.
   - _Clearing logs_
     - This is the "wiping the fingerprints away."
     - **How to Clear Logs in Windows:**
       - **Clearlogs.exe -**
         - Needs to be installed.
         - Run the command : `clearlogs.exe -sec`
         - Clearlogs.exe clears the security logs of the target system, which can be verified by opening the Event Viewer.
     - Beginner mistake is to not remove the clearlogs.exe and leaves hard evidence that log tampering occurred.
       - On a Windows 10 system or Windows Server 2016, the Event ID `1102(S)` will be displayed.
   - _Meterpreter_
    - An advanced payload is a sort of shell that can help clear all logs in a Windows system after compromising the system with Metasploit.
      - Command: `clearev`

   - _Windows Event Viewer_
     - Even if auditing has been disabled, it is still smart to clear logs in **Windows Event Viewer** because disabling auditing will display as an event.
     - To do this:
       - Open Event Viewer
       - Open Windows Log
       - Right click on logs and select `Clear All Events`
   - _Linux systems_
     - To clear Linux logs, you want to use the `shred` tool.
       - `Shred -vfzu auth.log`
         - **auth.log** tracks logins and permissions (like sudo) escalation.
   - _Modifying logs_
     - Know where the logs are located.
     - A text editor may be required to modify logs.
   - _Erasing command history_
     - Bash (Linux) retains a history of bash commands.
       - They can be found in `~/.bash_history`
       - Like deleting `clearlogs.exe` file on Windows, be sure to erase the `Shred -vfzu auth.log` command from the bash history.

## Additional Resources

Guide to Data-Centric System Thread Modeling ([article](https://csrc.nist.gov/pubs/sp/800/154/ipd#pubs-abstract-header))
