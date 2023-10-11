# Class 05 Reading Assignment
## Linux Command Line for Beginners ([link](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview))
## Why It Matters
The command line is one of the most important tools in cybersecurity (and server management) and understanding how to utilize it is a critical skill to develop.

## Questions
1. **Explain the terms “shell”, “terminal”, “cli”, and “command prompt”. Why are these still used today, when we have graphical interfaces?**
   - While, shell, terminal, command line interface (CLI), and command prompt are often used as interchangable jargon for a text-based interfaces for computers they are not the same although they are almost always used in conjunction with one another.
   - **shell** - The shell is command line interpreter that takes commands and allows users to run scripts in the command line. (Bash and Zsh are two popular modern shells)
   - **terminal** 
      - Originally, terminals were basic computers that allowed a connection to a mainframe computer and not able to run their own programs, instead simply sending input to the server and display results (similarly to remote SSHing into a server nowadays). 
      - Today, terminal emulators are programs used to access the command line and shell. 
   - **CLI** - The command line interface is the text interface that terminal emulators use to interact with the computer.
   - **command prompt** - The command prompt where you are prompted to enter commands and usually can be configured to display information is specific ways. Example: `mark@linux-desktop: ~$` (A popular prompt is [Starship](https://starship.rs/)) 
   - Compared to graphics interface, text interfaces are very light on system resources and commands are short amd capable of being combined, allowing for speed and efficient that is difficult to match with a graphical interface. As text is also small in size, it allows for fast interaction over networks even despite slow connections.
2. **What are the commands to change directories, list the file’s contents and rename/move files?**
   - `cd` (change directory) change directories.
     - Syntax: `cd <Directory Name>` 
     - Example: `cd Documents`
     - It is also possible to move to the parent directory be using `..` . Example: `cd ..` while in `~/Documents/notes` will take you to `~/Documents/`
     - Like all of Linux, capitals matters and due to this the `Documents` folder would be different than the `documents` folder. 
   - `ls` (list) shows a directory's contents.
     - Syntax: `ls` 
     - Additional arguments may display more information, example: `ls -a`
   - `mv` (move) is used to move files. To move a file you must indicate the file you wish to move and the location you wish to move it to.
       -  Syntax: `mv <file_name> <Destination_path>`
       -  Move example: `mv text.txt ~/Documents/`
    - `mv` is also used to rename files. To do so you indicate the file and what it will be renamed to. It is possible to note that you can move and rename a file in the same command.
       -  Syntax: `mv <file_name> <new_file_name>`
       -  Rename example: `mv example.txt old_example.txt` 
       - Rename & move example: `mv example.txt ~/Documents/old_example.txt`
3. **What are relative and absolute paths? What is special about starting with a ~ (tilde) or a ‘/’ character in the path?**
   - A *relative path* depends on what your working directory is and is relative to that position. An *absolute path* is the fixed location of a file or directory and can be used regardless of where in the file system you are located. A good analogy is determining the location of something based on where you -- for instance, whether you turn left on street depends on the direction you, the driver, is coming from -- versus it's coordinates on a map, which never change regardless of where you are coming from. 
        - Relative path example: `mv example.txt ../class-02/` 
           - This command would move the `example.txt` from this directory to the `class-02` directory in the parent directory of the directory we are currently in.
        - Local absolute path example: `mv example.txt ~/Documents/class-02/` 
           - This command would move the `example.txt` file from our working directory (current location) to the `class-02` directory in `~/Documents/` 
        - Total absolute path example: `mv ~/Downloads/ubuntu.iso ~/Documents/Codefellows/Linux-ISOs/` 
           - This command would move the `ubuntu.iso` file to the `~/Documents/Codefellows/Linux-ISOs/` directory regardless of our working directory.
    - The `/` path is your *root directory* and is the absolute base of the entire filesystem.
    - The `~` path is your user's *home directory*. (The absolute path of the home directory is `/home/<username>`)
4. **Explain what Linux is, using anything except English.**
   - Linux é uma marca de sistemas operacionais que utiliza o kernel Linux criado por Linus Torvalds.


## Things I Want to Know More About
More CLI commands! I've heard that https://overthewire.org/wargames/ is a good way to practice.
