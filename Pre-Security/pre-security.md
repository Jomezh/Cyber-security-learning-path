# 🛡️ TryHackMe Pre-Security Path – Progress Log

> ✅ Completed Path  
> 📅 Date: 02 June 2025 
> 🎯 Focus: Foundational knowledge of Cybersecurity, Networking, and Career Tracks

---

## Room 1: Offensive Security Introduction
- Overview of **offensive security** and its objectives
- Basic simulation to demonstrate offensive actions
- Introduction to careers in offensive roles (e.g., Pen Tester, Red Teamer)

## Room 2: Defensive Security Introduction
- Understanding **defensive security**: detection, response, and prevention
- Hands-on simulation showcasing defensive workflows
- Overview of defensive roles in the industry

## Room 3: Careers in Cybersecurity
- Exploration of various cybersecurity roles:
  - Security Analyst, Security Engineer, Incident Responder
  - Digital Forensics Examiner, Malware Analyst
  - Penetration Tester, Red Teamer
- Included a personality quiz  
  > 🧠 **Result**: Security Analyst  
  > 🚩 Recommended Paths: Pre-Security, SOC Level 1, Junior Penetration Tester

## Room 4: What is Networking?
- Introduction to computer networking and the internet
- Identifying devices in a network
- Basic use of **ping** and **ICMP** protocols  
- Interactive lab: Simulating real-world network discovery

## Room 5: Introduction to LAN
- LAN topologies (Star, Mesh, Bus, etc.)
- Basics of **subnetting**
- Overview of **ARP** and **DHCP**
- Understanding how devices receive dynamic IPs
- DHCP server concepts explained

## Room 6: OSI Model
- Introduction to the **7 layers** of the OSI Model:
  1. Physical  
  2. Data Link  
  3. Network  
  4. Transport  
  5. Session  
  6. Presentation  
  7. Application  
- Interactive lab: OSI-layer packet walkthrough

## Room 7: Packets and Frames
- Explanation of **packets**, **frames**, and data transmission
- TCP/IP stack and **Three-Way Handshake**
- **UDP/IP** for low-latency comms (without integrity checks)
- Introduction to ports and basic networking protocols

## Room 8: Extending Your Network
- Basics of **port forwarding** and **firewalls**
- Hands-on firewall lab (packet filtering)
- Intro to **VPN technology**
- Overview of networking hardware
- Simulation lab using a network simulator

## Room 9: DNS in Detail
- Breakdown of **Domain Name System**
- Hierarchy: Root → TLD → SLD → Subdomain
- Key DNS records:  
  - `A`, `AAAA`, `CNAME`, `MX`, `TXT`
- Step-by-step DNS resolution process
- Interactive DNS request lab

## Room 10: HTTP in Detail
- An overview of what **HTTP(s)** is
  - Talking about requests and responses— overview of **URL** and its components
    - `Host`, `User`, `Host`, `Port`, `Path`, `Query String`, `Fragment`
  - How a request is made
  - Its response
- Different HTTP methods— `Get`, `Put`, `Post`, `Delete`
- Different HTTP status codes
- HTTP headers—**Request Header** and **Response Header**
- What are **Cookies**, and a related interactive lab
- A practical lab to deepen the understanding of making HTTP(s) requests

## Room 11: How Websites Work
- Overview on basic workings of websites—`Front End (client-side)` and `Back End(Server-side)`
- Basics on **HTML** and an associated interactive lab
- Basics on **JavaScript** and an associated interactive lab
- A section about **Sensitive Data Exposure**
- Overview of **HTML Injection** and and associated interactive lab

## Room 12: Putting it all together
- How all the components of network— `Browser`, `DNS`, `Webserver`, `Website`— work together provide the system that we experience
- Certain components that help improve the efficiency of the system—`Load Balancers`, `CDN(Content Delivery Network)`, `Databases`, `WAF (Web  Application Firewall)`
- Working of webservers

## Room 13: Linux Fundamentals Part 1
- Introduction to what **LINUX** is
- Gives a breifing on **Linux**— its uses, Flavours.
- Introduction to interacting with **Linux** machine (in-browser)
- Basic commands like `echo`, `whoami`
- Commands that are used for interacting with FileSystem
  -  `ls`, `cd`, `cat`, `pwd`
- Searching for files using commands — `find`, `grep`
- Shell operators — `&`, `&&`, `>`,`>>`

## Room 14: Linux Fundamentals Part 2
- Accesing **Linux** machines using **SSH**
- Introduction to flags and switches (eg; `-a`). Using `man` command to open the manual.
- Further on *Filesystem* interaction.
  - `touch`, `mkdir`, `cp`, `mv`, `rm`, `file`
- A section regarding all the basics of *Permissions*. Covers **Users** and **Groups**— switching between **Users** `su`.
- Common directories; `/etc`, `/var`, `/var`, `/tmp`

## Room 15: Linux Fundamentals Part 3
- Terminal Text Editors; use of `nano` and `VIM`
- General utilities— Downloading files `Wget`, Transferssing file from Host `SCP(SSH)`, Serving files from Host `WEB`
- Overview on **Processes**— `ps`, `ps aux`, `top`, `kill`, `SIGTERM`, `SIGKILL`, `SIGSTOP`, `systemcl` *(start, stop, enable, disable)*
- Automation using *cron*  `crontab`, `crontab -e`
- Packages and repos
- System logs `access log`, `error log`

## Room 16: Windows Fundamentals 1
- Introduction to windows and its editions
- Desktop/GUI
- Filesystem; **NTFS** `Permissions`, `ADS`.
- **System32**
- User Accounts, Profiles and Permissions
- User Accounts controls
- Settings and Control Panel
- Task manager

## Room 17: Windows Fundamentals 2
- System configuration `msconfig`
- User Account Controls **UAC**
- Computer management `compmgmt`
- System Information `msinfo32`
- Resource monitor `resmon`
- Command Prompt `cmd`
- Registry Editior `regedit`

## Room 18: Windows Fundamentals 3
- Windows Updates `control/name Microsoft.WindowsUpdate.`
- Windows Security 
- Virus & threat protection
- Firewall & network protection `WF.msc`
- App & browser control
- Device security *core isolation*, *TPM*
- **BitLocker**
- Volume shadow copy service **VSS**