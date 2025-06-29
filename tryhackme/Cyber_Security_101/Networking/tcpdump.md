# 🎣Tcpdump: The Basics

> 🗣️Talks about command line argument ***tcpdump***

> 📅 *Completed on* 22-06-2025

---

## 📦Basic Packet Capture
- Can choose the network interface to listen to using `tcpdump -i <interface>`
- Interfaces on the devie can be obtained using `ip a s` command
- The packet captured can be saved to be accessed later using `-w <File_name>`
- The most commonly used extention is .pcap
- To read the captured file use command `-r <File_name>`
- Number of captured packet count can be limited using `-c <COUNT>`
- If count is not specified, it will keep capturing the packets till you stop it
- By default it will resolve the ip address to appropriate domain and port number to such as `80` to `http`. This can be avoided using `-n` and `-nn`
- The output can be made more verbose using `-v` command. The more verbose you need it to be, more the 'v' you need to add
- commands
    - `tcpdump -i Interface`
    - `tcpdump -w file`
    - `tcpdump -r file`
    - `tcpdump -c Count`
    - `tcpdump -n`
    - `tcpdump -nn`
    - `tcpdump -v`

## 🥅Filtering Expressions
- To filter packets of a particular host, you can use `host <IP>` or `host <HOSTNAME>` commands
- Also can filter between incoming and outgoing packets using `src host <HOSTNAME>` and `dst host <HOSTNAME>`
- To filter packets based on ports: `port <portNumber>`
- Source and destination can also be specified like host
- Protocols can also be filetered `ip`, `tcp`, `udp`, `icmp`, `ip6`
- Logical operators like `and`, `or` and `not` can be used to filter and combine filters

## ⚙️Advanced filtering
- Can be filtered based on their length: `greater <Length>` and `lesser <Length>`, greater than or equal and less than or equal respectively
- Header bytes and filtering based on header bytes
- `proto [expr:size]`
    - `proto` refers to the protocol like `arp`, `ether`, `icmp`, `ip`, `ip6`, `tcp`, `udp`
    - `expr` refers to the offset, as in 0 being first byte
    - `size` number of bytes that we want to look at, one by default
- You can use `tcp[tcpflag]` to compare with tcp falgs
    - `tcp-syn`: synchronize
    - `tcp-ack`: acknowledge
    - `tcp-fin`: finish
    - `tcp-rst`: reset
    - `tcp-push`: push

## 📺Displaying Packets
- There are different ways to display packets
- `-q`: Quick output; print brief packet information
- `-e`: Print the link-level header
- `-A`: Show packet data in ASCII
- `-xx`: Show packet data in hexadecimal format, referred to as hex
- `-X`: Show packet headers and data in hex and ASCII

---
