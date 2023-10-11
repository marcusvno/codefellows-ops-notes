# Class 01 Reading Assignment
## The Big Hack - How China Used a Tiny Chip to Infiltrate America's Top Companies
## Why It Matters
Coupled with our instruction on the component parts of a PC, this story demonstrates that the security vulnerabilities we, as future cybersecurity professionals, will face are not only software based but can also be hardware based. Making sure to not discount any possibility out of hand, like the **Apple** engineers did with the odd network activity and firmware issues on their servers, is what will allow us to be successful in detecting and countering hardware attacks.
### Discovery
In 2015, **Amazon** started evaluating a startup called **Elemental Technologies** for an acquisition in preparation of a massive expansion of their own streaming video service (Amazon Prime). **Elemental Technologies** specialized in software for video compression and had multiple national security contracts (such as with the CIA) which fit well with **Amazon's** highly secure cloud services (AWS) that **Amazon** also offered to the US Government. 

A third party security company was hired to examine *Elemental Technologies* servers (used for video compression) and there they found a tiny microchip that was not part of the boards' orginal design. The servers were assembled by **Super Micro Computer Inc.** (Supermicro), one of the world's largest suppliers of sever motherboards. At the same time, **Apple** had detected some firmware problems and odd network activity and similarly reached out to the US Authorities, however, **Apple** was vague and unwilling to provide access to the compromised hardware which left the investigation unsure of how to proceed until **Amazon** reported what it had found.

The subsequent report by **Amazon** to the US authorities raised alarm bells everywhere: **Supermicro** assembled **Elemental** servers were utilitized in highly sensitive locations: Department of Defense centers, CIA, Navy warships. Investigators found that chips were inserted during the manufacturing of the boards by subcontractors in China, noting it as an incredibly devastating supply chain attack ever conceived; something state-level actors like the NSA would be willing to invest multiple years and millions of dollars achieving.

Unlike interdiction hardware attacks, which happen during transit of the manufactured devices, China opted for changing the boards at the very inception of their construction, something they are highly advantaged to doing as they are estimated to build 75% of the world's mobiles and 90% of its computers.

**The investigators estimated that the hack affected almost *30 companies*, including banks, government contractors, and Apple.**

### Denial & Outcome
Despite multiple companies (**Amazon, Apple, Supermicro**) denying such a security exploit was discovered and US authorities declining to comment, several current and former senior national security officials have comfirmed the discovery of the chips and the subsequent investigation. The full ramification of the attack is still unknown, although the Trump administration has added computer hardware to part of its trade sanctions against China and the Biden administration passed the CHIPS bill to move manufacturing of computer chips back to the United States. 

### Questions:

1. **How is a hardware hack different than a software hack?**
   - Unlike software hacks, which target security holes in the software of a machine and can be patched, hardware hacks are decidedly more nefarious and dangerous as they are significantly more difficult to detect, can give backdoor access to the compromised machine, and cannot be patched in the same ways a software hack can be patched.
   - However, hardware hacks leave a real-world trail. Components aren't cheap and they leave a paper trail as they are shipped and sent all over the world. 
2. **What are the two ways for a spy to alter a computer's hardware?**
   -  *Interdiction*, favored by US intelligence agencies, intercepts the hardware in transit between manufacturer and consumer (or contractor like **Supermicro**). The alternative is to build the hack into the device during the manufacturing process as seen in this hack.
3. **Explain how the hack worked.**
   - Incredibly small, the chips were designed to by as inconspicuous as possible, easily mistakeable for signal conditioning couplers rather than microchips. Officials familiar with the investigation say the chips were made to create backdoors for other attackers to gain access to the compromised computers. They accomplished this by manipulating the operating instructions of the server that dictates what to do as data moves across the motherboard. As the computer's operating system (stored in the temporary memory) was en route to the CPU, the chip intercepted the data and could inject its own code or alter the instructions to the CPU. 
   - Due to the devices' small size, the code it could store and inject was also small but it was enough to allow it to tell the PC to contact computers on the internet with more complex code and able to prepare the computer's operating system to accept the more complex code. This was possible because the chip was connected to the *baseboard management controller*, a chip commonly used by sysadmins to remote log into servers. 
   - This could allow attackers to alter how the server functioned in an almost completely undetectable manner.
4. **How were investigators able to trace the chips back to the source?**
   - Investigators traced the **Supermicro** supply chain backwards towards the three primary manufacturers constructing its motherboards. US intelligence agencies used communication intercepts, informants, and even mobile phone tracking to discover which subcontractors were utilized and which had been compromised by Chinese agents.

## Things I Want to Know More About
Hardware hacking in general and the process in which these hacks can be detected in software activity, if possible.
