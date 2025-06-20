# 🛜Network Securing Protocols

> 🥅Discusses protcols that manage network security

> 📅**Completed on** 15-06-2025

---

## 🔐TLS
- In normal networking protocols there was the vulnerability of packet-capturing by with an attacker can intercept and access data
- To prevent this initially Secure Socket Layer (SSL) was developed
- Later on Transport Layer Security (TLS) was developed as an upgrade to SSL 3.0
- It is a cryptographic protocol at the transport layer of the OSI model
- Allows for secure communication over an insecure network

## #️⃣HTTPS
- HTTP uses TCP port 80
- It was sent over clear text and anyone could intercept
- HTTPS stands for Hypertext Transfer Protocol Secure—HTTP over TLS
- Normal HTTP
    - Establishes TCP three-way handshake
    - Communicate using HTTP protocol
- HTTPS
    - Establishes TCP three-way handshake
    - Establishes TLS connection
    - Communicates using HTTP 
- All the packets gets encrypted, thus it requires key to access the contents of the packets

## ⌨️SMTPS, POP3S, and IMAPS
- Its no different that HTTPS
- S is added for Secure for the security added by TLS
- Ports used by non-secure protocol
    - HTTP : `80`
    - SMTP : `25`
    - POP3 :`110`
    - IMAP :`143`
- Ports used by secure protocol
    - HTTPS : `443`
    - SMTPS :`465` and `587`
    - POP3S : `995`
    - IMAPS : `993`

## 🐢SSH
- ***Secure Shell***
- To administer remote system
- Port `22`
- It offers 
    - Secure authentication: password auth, public key, two factor auth
    - Confidentiality: provide end-to-end encryption
    - Integrity: protects integrity of traffic
    - Tunneling: creates a secure tunnel, similar to a VPN
    - X11 forwarding: connecting to a UNIX-like system with graphical interface allows use of graphical application over the network

## 🗃️SFTP and FTPS
- ***SSH File Transfer Protocol*** and ***File Transfer Protocol Secured***
- SFTP shares same port as SSH
- SFTP commands are UNIX-like and differ from FTP
- FTP uses port `20` while FTPS uses `990`

## 🔑VPN
- ***Virtual Private Network***
- The VPN client will entcrypt the data and pass it through the VPN server via the VPN tunnel.
- Once a VPN tunnel is established all the internet traffic will be routed over the VPN connection

---