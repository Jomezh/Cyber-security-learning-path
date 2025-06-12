# 🛜Networking Concepts

> ⚽Basic networking concepts

> 📅*Completed* on 11-06-2025

---

## 📳OSI Model
- ***Open Systems Interconnection (OSI)*** decribes how communication should occur in a computer
- It is comprised of seven layers
    1. **Physical Layer**: Refers to the physical connection between devices— ethernet cable, Wifi etc.
    2. **Data Link Layer**: It refers to how devices within a network communication with each other.
    3. **Network Layer**: It refers to how different networks communitcate and interact with each other
    4. **Transport Layer**: It refers how communication/data transfer occurs between networks— `TCP`, `UDP`
    5. **Session Layer**: Establishes connection and sychronizes between applications
    6. **Presentaion Layer**: Makes sure that the data is properly understood, —encoding, decoding, and encryption.
    7. **Application Layer**: End user applications

## 🪪TCP/IP Model
- The **TCP/IP** model has 4 layers
- Application layer, contains the layer 5,6, and 7 of the **OSI** model
- Transport layer, is same as layer 4 of **OSI** model
- Internet layer, same as the layer 3 of the **OSI** model
- Link layer, same as the layer 2 of the **OSI** model

## ➕IP Addresses and Subnets
- Identifier for the hosts to identify and communicate
- Diviied into 4 octect
- IPv4 is the most commonly used one
- Can use `ipconfig` command on windows, `ifconfig` and `ip a s` on linux and UNIX-based system to look up the IP address
- There are private and public IP addresses
- Private is for the devices to communicate within a network, and public is for communcation over the internet
- Routing: The router forwards the data packets over the interneto to the proper network. Usually it takes packets to pass through multiple routers before reaching its destination

## 🪢UDP and TCP
- There are two transport protocols
- **UDP**: ***User Datagram Protocol***, allows to reach specific process on this target host. Its based on layer 4. Its connection less, hence doesn't have methods to make sure if the data is recieved properly.
- **TCP**: ***Transport Control Protocol***, forms a connection between two hosts before transportation. The connection is based on a protocol called three-way handshake, sends out a request for connection `SYN`, recieves an acknowledge signal `SYN-ACK`, and then a packet acknowledging that the acknowledgement has been confirmed is send out `ACK`. Ensures proper data transfer.

## 💊Encapsulation
- Each layer— from application to datalink—adds its ouwn headers or trailers or both to the data being transferred by the process called encapsulation.
- Each layer adds relevent information by each layer protocol for the proper data transfer
- Application layer adds header based on the application protocol based on the transport layer
- Transport segment adds header creates a **TCP** *segment* or **UDP** *datagram* and is sent to the layer below called network layer
- Network layer adds an IP header and this IP packet is send to the layer below
- Data Link frame, ethernet or WiFi recieves the IP packet and adds proper header and trailer creating a frame

## 📞Telnet
- A practical session giving a hands-on practice on the telnet command, connecting to an IP and port.

---