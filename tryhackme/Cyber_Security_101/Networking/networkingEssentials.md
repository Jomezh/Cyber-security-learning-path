# 🪢Networking Essentials

> 🐾Essential concepts in networking

> 📅***Completed*** on 12-06-2025

---

## 🤝DHCP
- Dynamic Host Configuration Protocol
- Provides a network configuration—***IP***, ***Router***, ***DNS***
- Automated way to configure connected devices
- Four steps are
    - ***DHCP Discover***
    - ***DHCP Offer***
    - ***DHCP Request***
    - ***DHCP Acknowledge***
- Uses `0.0.0.0` as IP address to request for an IP from broadcast address`225.225.225.225`
- For link layer it sends to broadcast MAC `ff:ff:ff:ff:ff:ff`

## 📛ARP
- Devices communate using MAC address to create a proper data link header
- Devices only need MAC addresses while communicating.
- The device will know the IP addresses
- ARP request is sent to the IP address that you want to know the MAC address of

## 📦ICMP
- ***Internet Control Message Protocol***
- Used for network diagnostics
- `ping` is an ICMP command to test connectivity of target system and measure **Round Trip Time**
- `traceroute` is `traceroute` in linux and `tracert` in windows, diacover route from host to target

## 🚦Routing
- It delivers packets from one network to another
- It uses various routing protocols to deliver the packets effieciently
- Eg: `OSPF (Open Shortest Path First)`, `EIGRP (Enhanced Interior Gateway Routing Protocol)`, `BGP (Border Gateway Protocol)`, `RIP (Routing Information Protocol)`

## 🎯NAT
- ***Network Address Translation***
- Minimizes the number of IP address used
- Assigns single IP for a network and the resolves the device that requested the packet


---