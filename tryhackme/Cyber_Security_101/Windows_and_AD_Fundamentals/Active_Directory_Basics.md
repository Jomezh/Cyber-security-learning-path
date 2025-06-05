# 🖲️ Active Directory Basics

> ‼️*Active Directory* is used to manage devices in windows based network domain in corporate levels. 

---

## Windows Domains
- **Centralised identity management**: all users can be configured from *Active Directory*
- **Managing security policies**: All security policies can be configured from *Active Directory*
- Such domains are used in corporate settings when large number of devices have to be managed under a network, providing user authentication. Found in settings like corporte network, university/school networks.

## Active Directory
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