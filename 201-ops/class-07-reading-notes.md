# Class 07 Reading Assignment

## Introduction to PowerShell
 - [Should you learn PowerShell?](https://www.techthoughts.info/ps1-should-you-learn-powershell/)
 - [Who needs Malware? IBM says most hackers just PowerShell through boxes now, leaving little in the way of footprints](https://www.theregister.com/2019/02/26/malware_ibm_powershell/)

 ## Questions

1. **What is the difference between Bash and PowerShell?**
    - Bash and PowerShell used to be the command line shells for the Linux and Windows, respectively. (Although, now, Bash and PowerShell are becoming more crossplatform.)
      - Bash works with strings and passes output/input as plain text. 
        - Strings allow for ease of sharing the data but requires a lot of string manipulation and parsing to get the information you are after.
      - PowerShell is not *just* a shell, it is a complete scripting environment and utilizes Objects instead of simply strings. This allows it to pass entire data objects and share complex data.
        - Because PowerShell operates with Objects, it can pass complex data around but these data objects are not universal and may not be accessible outside of PowerShell.
    - These two technologies aren't truly 1:1 equivalent. A Bash/Python mix would be closer to a proper comparison to PowerShell's capabilties while PowerShell can't achieve the same levels of capabilithes that Python has.
2. **In what scenarios or environments can you use PowerShell? Name some major platforms where PowerShell is supported.**
    - PowerShell has gone from being a Windows exclusive feature to cross-platform compatability, allowing it to be used in almost any environment and making it a very attractive command line scripting tool because of that. 
    - Some of the major platforms PowerShell can be used on are:
      - Windows
      - Linux
      - Hyper-V
      - VMWare
      - AWS
      - Azure
      - Oracle
3. **List at least three reasons why learning PowerShell could be beneficial for your career and environment.**
    - Cross-platform versatility
      - Learning a cross-platform tool means having it available no matter what working environment you find yourself in. It will always be useful everywhere.
    - Relevancy 
      - As its adoption continues to grow across the industry, learning PowerShell becomes less of a choice and more of a necessity to be competitive in the job market.
    - Automation 
      - Automation allows you to spend your time on more critical tasks.
4. **How can PowerShell’s automation capabilities improve efficiency and reduce manual errors?**
    - Doing repetitive tasks manually can lead to mistakes. PowerShell can test outcomes and ensure accuracy. It can even catch and correct some errors.
5. **Think about a situation where you might use PowerShell in your everyday life or job. How could PowerShell help you accomplish a specific task or solve a problem?**
    - PowerShell's automation could be useful to maintaining system updates and drivers without having to do it manually. In a Linux environment, we could use cronjobs to launch Windows VMs through the command line and have PowerShell automate any driver and updates installations before shutting the VMs off. Therefore, saving us time from having to manually launch every VM and update them ourselves.

## Additional Resources:
- [What is a PowerShell attack?](https://www.youtube.com/watch?v=fe5Mbszdu9M) (Video)
- [Microsoft Docs: What is PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/overview?view=powershell-7)
- [Microsoft Docs: Getting Started with PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/learn/ps101/01-getting-started?view=powershell-7)
- [Quick Reference - PowerShell Variables and Operators](https://ss64.com/ps/syntax-variables.html)


## Things I Want to Know More About
I'd love to see usage examples that demonstrate the power, pun intended, of PowerShell while still being understandable for a beginner user.
