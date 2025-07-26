# NSTU Campus Area Network Design

This project presents a complete simulation of the *Campus Area Network (CAN)* for *Noakhali Science and Technology University (NSTU)* using Cisco Packet Tracer. 
The network connects multiple departments, halls, library, and administrative buildings, implementing key routing protocols and access control mechanisms.

## 📌 Project Goals

- Design a scalable and structured network for NSTU
- Implement proper routing and segmentation
- Ensure secure communication using ACLs and VLANs
- Simulate realistic university infrastructure

## 🛠 Technologies Used

- *Cisco Packet Tracer*
- *OSPF (Open Shortest Path First)*
- *EIGRP (Enhanced Interior Gateway Routing Protocol)*
- *BGP (Border Gateway Protocol)*
- *ACL (Access Control List) –  Extended*
- *VLAN (Virtual LAN)*
  
## 🔐 Security Implementation

- * Extended ACLs* to filter network traffic(all departments can communicate with server but they cannot communicate with each other)
- VLAN segmentation for isolation between different buildings/departments
- Controlled Internet access simulation

## 🗂 File Included

- Campus Area Network.pkt – The main Packet Tracer project file

## 🖥 How to Use

1. Open Campus Area Network.pkt with *Cisco Packet Tracer*.
2. Explore the network topology: routers, switches, PCs, and servers.
3. View and modify routing tables, VLANs, and ACL configurations.
4. Use the simulation tab to test connectivity and packet flows.

## 🧾 Sample Configuration Snippets

### OSPF on Core Router
router ospf 1

network 192.168.160.24 0.0.0.3 area 0


##EIGRP
router eigrp 100

network 192.168.1.0 0.0.0.255

no auto-summary

##BGP

router bgp 10

neighbor 192.168.233.8 remote-as 100
