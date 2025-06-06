# 🖲️ Active Directory Basics

> ‼️*Active Directory* is used to manage devices in windows based network domain in corporate levels. 

---

## 🏛️Windows Domains
- **Centralised identity management**: all users can be configured from *Active Directory*
- **Managing security policies**: All security policies can be configured from *Active Directory*
- Such domains are used in corporate settings when large number of devices have to be managed under a network, providing user authentication. Found in settings like corporte network, university/school networks.

## 🎯Active Directory
- Core of windows domain is **Active Directory Domain Service *(AD DS)*** 
- Holds the information of all the objects that are in the network
    - *AD* objects are, `users`, `groups`, `machines`, `printers`, `shares`
- ### Users
    - Most common obejct types 
    - They are known as **security principals**; can be authenticated by the domain and assigned resources like printers and files.
    - **Users** can represent two types of entities—`People`, `Services`
    - *People* : Persons in organization that access the network
    - *Services* : Services need users to run. They will only have privilleges needed to run their specific services
- ### Machines
    - Represent every computer that join the domain
    - They are also considered **Security principals**
    - They are local administrators within the computer itself
    - The machine accounts can be identified easily; if the device is named `DC01` then the machine account will be `$DC01`
- ### Security Groups
    - You can define *User Groups* to assign privelleges to a group of users.
    - Improves managebility and better organization
    - Default security groups are:
        - `Domain admins`, `Server Operators`, `Backup Operators`, `Account Operators`, `Domain Users`, `Domain Computers`, `Domain Controllers`
- Objects can be grouped into **Organizational Units (OU)**. They object containers that classify users and machines.
- **OU** is for applying polices to multiple objects, whereas **Security Groups** are to grant permission over resources to multiple users.

## 👤Managing Users in AD
- Deleting extra *OU*s and users
- **Deletgation**: Controls given to specific users over *OU*s

## 💻Managing Computers in AD
- By default all the machines that join a domain — except for the *DC*s— will be put in the container called **"Computers"**
- Devices can be divided into `workstations`, `servers`, `domain controllers`

## 🚨Group Policies
- *Group Policies* can be assigned to *OU*s
- They are manged through **Group Policy Objects**
- *GPO* can be customized using **Group Policy Management** tool
- *GPO* are shared to the network via network share called `SYSVOL`. They sync the devices in the network periodically. But the changes can take upto 2 hours to reflect throughout the entire network

## 🔐Authentication Methods
- There are two main protocols `Kerberos`, and `NetNTLM`
- ### Kerberos Authentication
    - Default authentication protocol for recent versions  of windows.
    - The users who log in will be assigned tickets
    - Initially they will be granted **Ticket Granting Ticket**
- ### NetNTLM Authentication
    - Uses challenge response mechanism
    - Challenge is generated is given to the client upon request for authentication
    - Client combines the **NTLM** password has with the challenge and sent it to the server. The server then forwards the challenge and response to Domain Controller for verfication.
    - Domain Controller uses the challenge to recalculate the request and compare it with the requet. If it matches the client is authenticated.

## 🌲Trees, Forests, and Trusts
- ***Trees***: Two similar domains in different regions with variations in certain group policies and are managed under same organization. They share same namespace.   
- ***Forests***: Domains under different namespace.Union of different trees with different namespace
- ***Trust Relationships***: Users from one domain having access to resources from a different domain.
    - One-way trust relationship: Only users from one domain can access from the other domain
    - Two-way trust relationship: Users from both domains can access resources from both domains.

---