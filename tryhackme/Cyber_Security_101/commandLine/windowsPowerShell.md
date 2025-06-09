# 🐚Windows Power Shell

> ***PowerShell*** is a cross-platform task automation solution made up of a command-line shell, a scripting language, and a configuration management framework.

> 📅*Completed on 06-06-2025*

---

## 💪What is PowerShell
- Developed to overcome the limitations of existing commnand line
- Develped usijng the ***.NET*** framework
- To make tasks more effective by manipulating onjects, offering deeper integration with Windows systems
- A versatile tool to be used accross multipe ***OS***

## 🧱PowerShell Basics
- PowerShell can be launched by just searching on start menu or using `Win+Run` and then running `powershell`, searching `powershell` in file explorer search, using task manager.
- You can launch **PowerShell** by just typing PowerShell in the *Command Prompt* ***(cmd.exe)***
- PowerShell commands are knowl as ***comdlets***
- It follows `Verb-noun` strucutre: `Get-content`, `Set-location`
- Basic Cmdlets: 
    - `Get-command`; discovering commands that we can use. Can obtain informatino regarding the command using `CommandInfo` object. ` Get-command -CommandType "Function"` filters commands with command types funciton
    -  `Get-Help`: provides detailed information about he cmdlets. The `-examples` command displays example use cases of a given cmdlet
    - `Get-Alias`: shows the traditional windows command names for the cmdlets; that is their *alias*
    - `Find-Module`: to search for modules *(collection of cmdlets)*
    - `Install-Module`: to install the searched module
    
## 🗺️Navigating File System and Working with Files
- `Get-childitem` is similar to `dir` and `ls`. `-Path` can be used to specify the path of the directory to display the contents of.
- `Set-Location` is used to similarly to `cd` to change the directory
- `New-Item` is used to create both new directories and files. You need to spcify the new file path or directory path when creating it
- `Remove-Item` is used simlarly to `rmdir` and `del`
- `Copy-Item` is used to copy files and directories
- `Move-item` is used to move files and directories
- `Get-Content` command can be used similarly to `type` and `cat`

## 🪈Piping, Filtering, and Sorting Data
- ***Piping*** is used to allow the output of one command to be used as input for another.
- This creates sequence of operation where data flow from one command to the next
- It is represented by `|` in CLI
- ***PowerShell*** piping on the other hand is more powerful as it passes objects than just text. It carries data, properties, and methods
- Example; `Get-ChildItem | Where-Object -Property "Extension" -eq ".txt"`, this takes the contents of a given file-path and filters it based on the extention ".txt"
- Next filtering option is `Select-Object`, it selects based properties like name and length of the file.
- `Sort-Object` is usd to sort the objects in a directory based on a value like length

## 🛜System and Network Information
- `Get-ComputerInfo` retrieves information about the system; BIOS, hardware specifications, OS infor, and more
- `systeminfo`, the traditional counterpart on the other hand fetches less information compared to the `Get-ComputerInfo` command.
- `Get-LocalUser` lists all the local users in the system
- `Get-NetIPconfiguration` is similar to `ipconfig`. It provides info about network interface, DNS, IP addresses, gateway configuration etc.
- `Get-NetIPAddress` provides details about a specific IP address

## ⌛Real-Time System Analysis
- `Get-Process` provides detailed view of currently running processes
- `Get-Services` provides status of all the services in the machine
- `Get-NetTCPconnection` displays information on current TCP connections
- `Get-FileHash` along with the path variable will provide the file hash of that particular file-path


## 📜Scripting
- Writing and executing a series of commands contained in a text file.
- It is used to automate tasks
- Its a todo list for the computer to perform a set of tasks
- It is used in various cyber-security fields like red-team, blue-team, and system administrators.
- `Invoke-Command` is essential for invoking commands in a remote system.

---