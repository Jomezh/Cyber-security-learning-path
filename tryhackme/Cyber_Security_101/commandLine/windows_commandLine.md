# 🗨️Windows Command Line

> Command Line Interface *(**CLI**)* is a text based interface that uses little resources, helps with automation and remote management.

> 📅 completed on 06-06-2025

---

## ❗Basic System Information
- We can only issue commands in a given path, so check the path using `set`
- `ver` can be used to determine the version of the ***OS***
- `systeminfo` can be used to fetch much more details about the ***OS*** and the ***System***
- Longer outputs can be managed by piping it using more `<command>|more`
- `help` provides information on specific command
- `cls` clears the commmand prompt screen
- `Ctrl+c` to stop the execution of the program

## 🛜Network Troubleshooting
- Network Configuration: network information can be checked using `ipconfig`
- For more informatino you can use `ipconfig/all`
- Network Troubleshooting: To see if the server can access particular server on internet you can use `ping <address>`
- You can also use `tracert <address>` to trace the routers that the package has to travel through.
- `nslookup` looks up host or domain and returns its IP address
- `netstat` return current network connection and listening ports
    - `-a`: display all established connection and listening ports
    - `-b`: shows the program associated with each listening ports and connections
    - `-o`: reveals the process id ***PID***
    - `-n`: uses numerical form for addresses and ports

## 📁File and Disk Management
- `cd` to change directory
- `dir` to list directories; `/a` to display hidden files and system files, `/s` to display current directories and subdirectories
- `tree` to display directories and subdirectories visually
- `mkdir` to make directories
- `rmdir` to remove directories
- `type` to view the contents of the files; `|more` can be used to manage display of large information.
- `copy` command to copy files
- `move` command to move files
- `del` or `erase` to delete files
- `*` can be used to refer to multiples files; `copy *.md C:/markdown ` will copy all files from that location with the file type .md

## ⚒️Tasks and Process Management
- `tasklist` to see all the proccesses that are running
- You can also apply filtersp; `tasklist /FI "imagename eq sshd.exe"` this will display the tasks with image name sshd.exe, `taskkill /PID target_pid` this can be used to display a task with particular ***PID***

## 🌀Some other Commands
- `chkdsk`: To check filesystem and disk volumes for errors and bad sectors
- `driverquery`: display a list of installed device drivers
- `sfc/scannow`: scans system files for corruption adn repairs them if possible.

---