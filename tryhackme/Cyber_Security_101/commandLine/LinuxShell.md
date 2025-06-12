# 🐧Linux Shells

> 🍟We all are used to the *Graphical User Interface* (*GUI*), which runs on top of the *OS*. But *Command Line Interface* (*CLI*), is a method to directly interact with the *OS*, hence making the interactions and performance much more resource efficient.

> 📅 Completed on 11-06-2025

---

## 🤏How TO Interact With Shell
- Most Linux distro uses ***Bash*** ***(Bourne Again Shell)*** as their default shell.
- `pwd` command can be used to identify the current working directory
- `cd` to change directory
- `ls` to list the contents
- `cat` to read the contents of the file
- `grep` to search for contents in the file

## 🦐Types of Linux Shells
- You can use `cat /etc/shells` to list all the *shells* within the system —`/etc/shells` contain the installed shells on a Linux system.
- To switch between the shells, just type the name of the shell in the command line and press enter. Eg; `bash`, `zsh`
- 🐚***Bourne Again Shell***
    - **Bash**: Default for most Linux distributions
    - Has scripting capabilities
    - Offers tab feature, autocomplete a command by pressing tab
    - It keeps history file and logs of all the commands and can be navigated through using `up` and `down` arrow keys. You can also type `history` on the command line and press enter to display the history as a list of commands
- 🍤***Friendly Interactive Shell***
    - **Fish**: Not default, and focuses on user-friendliness
    - Offers simple syntaxes that are user-friendly
    - It has auto-spell correct unlike bash
    - Customizable prompt with fish compatible themes
    - Syntax highlighting based on their roles
    - Also provides scripting, tab completion, and command history
- 🎼***Z shell***
    - **Zsh**: Not default, and is considered a modern shell
    - Provides advanced tab completion, and script writing
    - Also provides spell correction
    - Command histroy and several other features
    - Can extend tab completion feature using plugn-ins

## 📃Shell Scripting and Components
- It is a set of commands to be executed in a particular order.
- It is used to automate tasks
- The file must be saved with `.sh` extention
- Every script should start from ***shebang***— a combination of characters that are added at the beginning of a script— starting with `#!` followed by the name of the interpreter to use while executing the script. Eg; `#!/bin/bash`
- Variables store a set of value inside it. To use a complex value, be a *URL*, *file path*— several times in a script.
- `echo` command displays a string on screen
- `read` reads input from user
- `Ctrl+x` to save and exit
- `chmod +x <name of file>` to make file executable
- *Loops* to iterate tasks 
Eg:
    `for i in {1..10};`
    `do`
    `echo $i`
    `done`
- *Conditional Statements* to act on certain conditions
Eg:
    `echo "please enter your name: "`
    `read name`
    `if [ "$name" = "Stewart" ]; then`
    `   echo "Welcome Stewart! "`
    `else`
    `   echo "Sorry you are not authorized"`
    `fi`
- *Comments* to write texts that doesn't affect the code
Eg:
    `# Command starts here`

## 🔑The Locker Script
- A script that verifies user before giving access

## ⚒️Practical Exercise
- To demonstrate and further deepen the understanding on scripting

---