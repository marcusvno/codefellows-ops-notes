# Class 03 Reading Assignment
## What is BIOS ([link](https://www.learncomputerscienceonline.com/bios/))
## Why It Matters
An understanding of the BIOS allows us to troubleshoot potential problems, understand the similarities between the real machine operates and a virtual machine will operate, and (as shown by the Prowler video) is another possible vector of attack which we must be mindful of.

## Questions
1. **What is the BIOS?**
- The Basic Input Output System (BIOS) is firmware (code that lives in ROM on the motherboard) that checks the hardware components and boots the operating system when a computer is turned on.
2. **Use analogies from your previous background to explain what happens during the booting process?**
- From my background as a chef, the booting process is similar to checking your mise en place prior to service and ensuring you have all your ingredients ready and prepared, your knives are ready, and your stove and oven are on and at temp. If something is missing, you have to fix it prior to service.
3. **What is the “Power On Self Test”?**
- The Power On Self Test (POST) is a self-check performed by the BIOS when the computer is turned on to check if the necessarily hardware components (CPU, RAM, fans, storage devices, graphics card, etc) are functioning properly. 
4. **What is the CMOS?**
- The CMOS is the Complementary Metal Oxide Semiconductor chip that is used to store the code necessary to the booting process. 
5. **What is the CMOS battery?**
- The CMOS battery is maintains the CMOS/BIOS ROM with power which allows to settings to persist during times that the computer is turned off. This allows for several settings like boot order, peripheral port enabling/disabling, and more, to persist between shutdowns and prevents security loopholes to get around these settings.

## Prowler Boot Virus
A MS-DOS virus that would infect any executable file and lived in the boot partition. It activated itself on the 13th on the month and showed a message and animation of a Lemming (love that game!) marching across the screen before booting the computer like normal. While the payload was seemingly innocuous -- it increased the size of every file it infected and at the time storage space was severely lmited which could cause problems if sufficient files were infected -- the implications and its ability to infect each and every executable was much more terrifting. Awesome stuff! 

## Things I'd Like to Know More About
The reading mentioned UEFI as a modern alternative to the BIOS. As our lab PC is set to Legacy mode would changing it to UEFI change that interface? Would that affect the bootloader in any way or is it like switching between Browsers, with each offering different experiences but the same fundamental functionalities?
