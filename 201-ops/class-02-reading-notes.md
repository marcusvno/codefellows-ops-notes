# Class 02 Reading Assignment

## What is Bash? ([link](https://opensource.com/resources/what-bash))

1. **What is the primary function of a shell in a computer's operating system?**
   - A shell is an application that operates outside the kernel and allows users to interact with the computer, usually by running other applications (commands) through the shell to the OS.
2. **How does Bash locate and execute commands on a Linux or Unix system?**
   - On \*Nix systems, most commands are stored in system directories such as **/bin**, for system wide commands, and **/usr/bin**, for user-specific commands; much like how Windows programs can be installed in the `C:\Program Files\` for system wide access or `C:\Users\marcus\AppData\Local\` for user specific. When a command is entered into *Bash*, it searches these directories to see if such a command exists. If the command is found, *bash* executes it. 
3. **How can you determine if your system is running a Bash shell?**
   - `echo $SHELL` will display whatever shell is currently being run in that terminal.
4. **What makes Bash scripting powerful and why is it considered scriptable?**
   - Anything you can type into *bash*, due to it being a text-based interface, can be put into a text file (known as a *script*) and be run automatically by the computer. Since almost everything in Linux runs on top of *bash* then almost everything can be scripted through *bash*. This gives immense customizable automation options to *bash* users who can make bespoke workflows with their scripts.
5. **Bash scripting allows for customization, automation, and efficiency. Discuss methods or practices from your previous work experiences or cultural background that aim to achieve similar goals in daily tasks.**
   - A professional kitchen is all about trying to achieve maximum efficiency and, more importantly, consistency under any customer load, whether during a sudden rush or a slow afternoon between lunch and dinner rush. The way this commonly done is through a strict use of specialized roles, prepared ingredients, and precisely placed and measure *mise en place* 
       - *Mise en place* is French for "everything in its place".
   - The *mise en place* is the routine and procedure that determines almost everything else in the kitchen as it determines the specific amounts of ingredients necessary for the day and determines what the prep crew will have to replenish. It also accounts for where ingredients are stored, ovens and fryer temperatures, and even the location of pots, pans, plates, knives, and towels so that regardless of which line cook or chef walks into the kitchen they can find everything fast and easy as well as placing ingredients near one another as needed by the recipes being made. A prep cook can come in and take a look at the *mise en place* and immediately know what they need to make at a glance. 

## Things I Want to Know More About
Bash scripting and the useful things it can be used for, such as after setting up a new Linux distro and having a script download and customize the OS to my specifications and my favorite tools.
