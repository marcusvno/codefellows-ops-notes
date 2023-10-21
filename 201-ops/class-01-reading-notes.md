# Class 01 Reading Assignment

## How to Use System Restore in Windows - ([link](https://www.lifewire.com/how-to-use-system-restore-in-windows-2626131))

1. What is the purpose of the Windows System Restore tool?
   - The Windows System Restore tool is to revert the system to a previous established *restore point* which holds the saved software, registry, and driver configuration of when the *restore point* was created. It is similar to the *snapshot* function of VirtualBox. Once activated, the System Restore tool will undo all changes since the *restore point* was created. 
2. How long does it usually take to use the System Restore tool in Windows?
   - Using the System Restore Tool revert to a previous point takes anywhere from 10 to 30 minutes. 
3. How do you start a System Restore from the command prompt?
Run the **rstrui.exe** command in the Command Prompt. 
4. What options are available if System Restore did not fix the problem?
If the System Restore doesn't fix the problem, then you can restore to an even earlier restore point, repeating the process until you find a configuration where the problem was not occuring. You may also need to try restoring in Windows Safe Mode in case there is malicious software loading with the normal Windows start.

## Things I Want to Know More About
Are there other situations where you might have to boot only into the command prompt to fix an issue on a Windows system?
