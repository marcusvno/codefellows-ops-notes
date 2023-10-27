# Class 05 Reading Assignment

## Microsoft Command Line Tools (CompTIA A+) ([link](https://www.professormesser.com/professor-messer-archives/220-1002/microsoft-command-line-tools/))

1. **How can you list the files in the current directory using the command prompt?**
	- `dir` command shows the contents of all the directory you are currently (like the `ls` command in Linux).
2. **How might the "sfc" command and "gpupdate" command help in troubleshooting on Windows?**
	- `sfc` is the System File Checker, utility used to scan all the critical operating system files and locate any that may be damaged and repair those if need be. It can be used to scan individual files and verify those files. It can also do offline repairs. 
	- Windows system in a job environment are likely managed at the group level. Group policy is often updated a logins but there are times you want to force a policy update prior login and that is when `gpupdate` comes in. `gpuupdate` is used to force a **g**roup **p**olicy **update** to a computer.
3. **What advantages does the "robocopy" command offer over the "xcopy" command, and why is it useful for the file transfers in certain situations?**
	- `xcopy` can be used to copy multiple files and directories in a single command. It can ignore folders that are have been created but are empty. `robocopy` (stands for robust copy) looks and acts similar to `xcopy` but with added features. One of the primary ones is the ability to resume a file transfer if it happens to be interrupted. This is particulary useful for transfering files over networks with intermittent connectivity. The information that `robocopy` provides during a transfer is also more descriptive and detailed than that offered by the `xcopy` command, allowing you to see the time it took for a copy to happen, the speed at which is happened (useful metric to judge connectivity), and the date. With automation, this would provide a useful log for later.
4. **Think about any real-life scenarios from your cultural context where the use of command line tools could be beneficial. Describe one such scenario and explain how a specific command line tool would help address the situation. **
	- `robocopy` would be a dream to have when dealing with massive folders of graphic design assets. Graphic designers accumulate a lot of art files so to not replicate effort (similar to IT knowledge bases used to allow future techs to solve problems faster), these assest folders can rapidly grow in size and may require often reorganization. `xcopy` and `robocopy` would have been great tools to use for creating back ups and for when I needed to provide large parts of my assets libraries to a team or a client. 

Additional Resource: [A+ Certification Cheat Sheet](https://gcit.enschool.org/ourpages/auto/2017/8/2/56105037/220%20901%20Cheat%20Sheet%202017.pdf)

## Things I Want to Know More About
With PowerShell becoming the default command line automation tool for Windows, does it utilize the same command line tools as the CMD does? Or does it have newer and different versions available as cmd-lets?
