# 🦈Wireshark: The Basics

> ⌨️Basics about wireshark

> 📅*Completed on* 16-06-2025

---

## ⛏️Tool Overview
- Use cases
    - Detecting and troubleshooting network
    - Detecting security anomalies
    - Investigating and learning protocol details
- Capable of loading PCAP files
- Capable of colouring packets based on their conditions
- Traffic sniffing capabilities
-  Can merge PCAP files
- Can view the File details

## 💉Packet Dissection
- Also called protocol dissesction, investigates packet details by decoding available protocols and fields
- Packet details: accessed by clicking on a packet, contains layers (5 to 7) based on *OSI* model
- Details of each layer can be accessed

## 🗺️Packet Navigation
- Wireshark assigns a unique packet number for each packets
- Can directly search for packet using packet numbers— `Go to Packet`
- Can also find packets by packet content using `Find packet`
- Packets can be marked
- Packet comments: comments can be helpful for analyst
- Packets can be exported
- Object files can also be exported—`DICOM`, `HTTP`, `IMF`, `SMB`, and `TFTP`

## 🥅Packet Filtering
- Two types of filters ***capture filters*** and ***display filters***
- ***Capture filters*** only capture packets for valid filter
- ***Display filters*** for viewing packets of valid filters
- Apply as Filter: Most basic way of filtering traffic. *Right Click menu* -> *Analyse* -> *Apply as filter*
- Conversation Filter: Filters based on IP address and Port numbers. *Right Click menu* -> *Analyse* -> *Conversation Filter*
- Colourise Conversation: Highligth linked packages without applying display filter. *View* -> *Colourise Conversation*
- Prepare as Filter: Created display filter like *Apply Filter*, but doesn't filter immediately and waits for an execution command or another filter to be added
- Apply as Column: Use information in packet details pane to create a column in packet list pane

--- 