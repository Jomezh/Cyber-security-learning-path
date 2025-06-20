# 🚦Networking Protocols

> 📦Talks about networking protocols

> 📅Completed on 14-06-2025

---

## 📛DNS
- Domain Name System
- Four types of naming
    - A record for IPv4
    - AAAA record for IPv6 
    - CNAME record for domain names referring to other domain
    - MX record for mail exchange

## ❓WHOIS
- It tracks registration and manages domain name registration
- Can use commands like `whois` on linux to pull up information on a domain name and details of their registration

## 🥅HTTP(S)
- HTTP commands are `GET`, `PUT`, `POST`, `DELETE`
- HTTP use port 80 and HTTPS use port 443

## 📁FTP
- Commands are `USER`, `PASS`, `RETR`, `STOR`
- `ftp` command is used to connect to the remote server
- After logging in, `ls` is used to list the files, `type ascii` is used to text mode when retrieving text files, `get <filename>` is used to get the file

## 📨SMTP
- ***Simple Mail Transfer Protocol***
- Commands are `HELO` or `EHLO`, `MAIL FROM`, `RCPT TO`, `DATA`, `.`(end of mail)
- `HELO` iniates mail transfer by connecting to the main domain
- Port ***`25`***

## 📮POP3
- ***Post Office Protocol version 3***
- Email is send relying on *SMTP* and is retrieved based on *POP3*
- Commands are `USER <username>`, `PASS <password>`, `STAT`, `LIST`, `RETR <message_number>`, `DELE <message_number>`, `QUIT`
- Port ***`110`***

## 📧IMAP
- ***Internet Message Accessing Protocol***
- Helps with accessing mail from multiple devices
- Allows for message synchronization
- Commands are `LOGIN <username> <password>`, `SELECT <mailbox>`, `FETCH <mail_number> <data_item_name>`, `MOVE <sequence_set> <mailbox>`, `COPY <sequence_set> <data_item_name>`, `LOGOUT`
- Port ***`143`***

---
