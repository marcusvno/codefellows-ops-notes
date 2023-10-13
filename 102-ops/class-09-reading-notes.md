# Class 09 Reading Assignment
## Why It Matters
With Windows having the leading marketshare of desktops and servers, it is of vital important to understand how to utilize the command prompt in it for server management. 

## Command Prompt ([link](https://www.lifewire.com/command-prompt-2625840))
1. **What is the Command Prompt?**
   - The Command Prompt is Window's command line interpreter, similar to Linux's shell, and is used to execute text-based commands, scripts, and batch files. 
2. **How do I access the Command Prompt?**
   - You can use **cmd* via the Run function on the Start Menu, via the Command Prompt shortcut on the Start menu, or simply by pressing Windows Key and typing out `command`, which will search up the command prompt shortcut.
3. What are some the most commonly used commands? (Citations at bottom)
   - `chkdsk`
      - Short for "check disk", it is a command line utility used to check disks and repair or recover data. 
      - Example: `chkdsk c: /r`
         -  This command performes an check on the `C:`, locates bad sectors, and recovers any readable data from them. It is best used outside of Windows from a recovery media.
   - `copy`
      - Copies file and stores second version in a specificed location. Similar to the `mv` on Linux, it can rename a file as well.
      - Example: `copy C:\Users\marcus\Downloads\test.txt D:\temp\`
         - The above command copies the `test.txt` file from the `Downloads` folder on the `C:` drive to the `temp` folder on the `D:` drive.
   - `ftp`
     - Transfers files from one computer to another. Other computer must be set up as an ftp server.
     - Example: `ftp ftp.example.microsoft.com`
         - Logs into the ftp server through `ftp.example.microsoft.com`.
   - `del`
     - Deletes files. Particularly useful with wildcard syntaxes to delete only certain files and relieve the user from having to delete each file individually.
       - Example: `del C:\Users\marcus\Pictures\*.png`
         - Deletes every file with the extension `.png`.
   - `format`
      -  Format is the command to delete everything on a partition (usually on a drive like a hard drive, USB, etc) and setting up a file system. Common file system are exFAT, FAT32, and NTFS.
      - Example:  `format d: /q /fs:exFAT`
        - This quick formats the `D:` drive to the exFAT file system. 
   - `ping`
      - The ping command is used to test connectivity to another networked device. You can ping IP addresses or hostnames.
         - Example: `ping 192.168.0.1`
         - In this example, we could ping the TP-Link router that was in the Lab Kit. (If the Lab PC was connected to that router)
   - `attrib`
      - Displays or changes the file attributes of a file or folder. This can change whether a file is hidden, editable, or even executable.
         - Example: `attrib +r C:\users\marcus\Documents\taxes`
            - This would make the `taxes` folder `read-only`.
   - `net`
      - Manages newtork settings on Windows, including but not limited to: network users, shares, print jobs, computers, sessions, groups, etc. 
      - Example: `net view`
         - Displays all networked devices.
   - `dir`
      - The Windows cousin to \*nix systems `ls` command, `dir` displays a list of files and folders in the current working directory. By default, it will also show the date and time the item was last changed, its size (if it is not a folder), and the name and extension. Like `ls` it can take modifiers to list more such as hidden items.
         - Example: `dir /ah`
            - Shows only the hidden files in the current working folder.
   - `help`
      - The `help` command is used to find out more about another command. (Linux has the `man` command)
         - Example: `help dir`
            - Shows you the help entry for the `dir` command.
   - `shutdown`
      - Command to power off, restart, log off, or sleep a computer. Can be used to remotely on other computers you have access to over a network.
         - Example: `shutdown /r`
            - Shuts down a computer fully and restarts it.
   - Note that many of the above commands can take flags, switches, or modifiers to alter the manner in which they are executed.
4. **What is Windows PowerShell?**
   - The PowerShell is essentially a beefed up version of the Command Prompt, with added functionalities (particularly in scripting and automation) to allow Windows to compete with Linux robust command line tools and capabilities. PowerShell is particularly useful for performing adminstrative tasks on a Windows server.  (Citation: Techtree)
5. **What is Windows Terminal?**
   - Windows Terminal is a Terminal emulator like those found on Linux and has increased functionalities that improve on Windows PowerShell and Command Prompt as well as being able to access both of those command line interperters. 


## Citation:
**When to use the Windows Command Prompt vs. Powershell (Techtree)**
   - https://www.techtarget.com/searchitoperations/tip/When-to-use-the-Windows-command-prompt-vs-PowerShell

**Lifewire - CMD Prompt Commands**
   - `chkdsk` https://www.lifewire.com/chkdsk-command-2625838
   - `copy` https://www.lifewire.com/copy-command-2625842
   - `delete` https://www.lifewire.com/delete-command-2625859
   - `format` https://www.lifewire.com/format-command-2618091
   - `ping` https://www.lifewire.com/ping-command-2618099
   - `attrib` https://www.lifewire.com/attrib-command-2625802
   - `net` https://www.lifewire.com/net-command-2618094
   - `dir` https://www.lifewire.com/dir-command-4050018
   - `help` https://www.lifewire.com/help-command-2618092
   - `shutdown` https://www.lifewire.com/shutdown-command-2618100
   - `ftp` https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/ftp


## Things I Want To Know More About
Powershell is becoming more crossplatform but so are Linux-esque terminal emulators like Alacritty and cmder, which allow the usage of Linux syntax commands on Windows, should we learn both? Focus on one?
