<div align="center">
  
# 🏥 Hospital Enterprise Network Design & Security Simulation

![Cisco](https://img.shields.io/badge/Cisco-Networking-blue?logo=cisco)
![Packet Tracer](https://img.shields.io/badge/Simulation-Packet%20Tracer-green)
![Security](https://img.shields.io/badge/Focus-Network%20Security-red)
![Architecture](https://img.shields.io/badge/Architecture-3--Tier-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

</div>

---

## 📌 Overview

This project presents a **secure and scalable enterprise network design** for a **multi-site hospital system**, implemented using Cisco Packet Tracer.

The system includes:
- 1 Main Site (Central Hub)
- 2 Branch Sites (DBP & BHTQ)

The design focuses on:
- Secure communication  
- Network segmentation  
- Centralized Internet control  
- Risk-aware architecture  

---

## 🎯 Objectives

- Design a **3-tier enterprise network architecture**
- Implement **VLAN segmentation & inter-VLAN routing**
- Deploy **secure WAN connectivity (MPLS / SD-WAN simulation)**
- Configure:
  - NAT (Internet access)
  - VPN (site-to-site & remote access)
- Apply **network security controls**:
  - ASA Firewall
  - ACLs
  - DMZ architecture

---

## 🧠 Network Architecture

### 🔷 3-Tier Design

- **Core Layer**  
  High-speed routing and WAN connectivity  

- **Distribution Layer**  
  Inter-VLAN routing (Layer 3 Switch), policy enforcement  

- **Access Layer**  
  End-user devices, wireless access  

---

### 🌐 Multi-Site Topology

- Main site acts as **central hub**
- Branch sites connect via **WAN tunnels**
- All Internet traffic is routed through **Main Site**

---

## 🧩 Key Features

### 1. Network Segmentation
- VLAN-based separation:
  - Staff  
  - Medical devices  
  - Administration  
  - Guest WiFi  

### 2. Inter-VLAN Routing
- Implemented using **Layer 3 Switch (SVI)**

### 3. NAT (Network Address Translation)
- PAT (Overload) configured at Main Site
- Enables internal users to access the Internet

### 4. VPN Connectivity
- Site-to-Site VPN between 3 sites  
- Remote-access VPN (teleworker)

### 5. Security Implementation
- Cisco ASA Firewall at each site  
- Access Control Lists (ACLs)  
- Traffic filtering between VLANs  
- Guest network isolation  

### 6. DMZ Design
- Public **Web Server** placed in DMZ  
- Isolated from internal network  

### 7. Wireless Network
- Separate Access Points:
  - Staff WiFi  
  - Guest WiFi (restricted access)

---

## 🔐 Security Architecture (Cyber Risk Focus)

This project applies **enterprise security principles**:

- Network segmentation limits lateral movement  
- DMZ protects internal systems from public exposure  
- Centralized Internet access improves monitoring  
- Firewall & ACL enforce strict access control  
- VPN ensures secure remote communication  

➡️ Designed based on **CIA Triad**:
- Confidentiality  
- Integrity  
- Availability  

---

## 🧪 Testing & Validation

### ✔ Verified Scenarios

- Intra-VLAN communication  
- Inter-VLAN routing  
- Cross-site connectivity  
- Internet access (via NAT)  
- DMZ server accessibility  
- Guest network isolation  

---

## 📊 Technologies Used

- **Networking**
  - VLAN (802.1Q)
  - Inter-VLAN Routing (SVI)
  - OSPF

- **Security**
  - Cisco ASA Firewall
  - ACLs
  - DMZ

- **WAN**
  - MPLS / SD-WAN (simulated)
  - VPN (Site-to-Site, Remote Access)

- **Other**
  - NAT (PAT)
  - Cisco Packet Tracer (Simulation)

---

## 📁 Project Structure
```
/docs
├── Specification.pdf
├── Final_Report.pdf
├── IP_VLAN_Plan.pdf

/simulation
├── hospital_network.pkt

/configs
├── core.txt
├── distribution.txt
├── access.txt
├── asa_firewall.txt
```
---

## 🚧 Limitations

- MPLS / SD-WAN simulated at conceptual level  
- No real IDS/IPS integration (Packet Tracer limitation)  
- Not implement a mechanism to automatically backup network device configuration
---

## 🔮 Future Improvements

- Integrate IDS/IPS systems  
- Apply Zero Trust Architecture  
- Add SIEM monitoring  
- Implement real SD-WAN controller  

---

## 👨‍💻 Author

**Ngo Giang**  
Aspiring Cybersecurity & Network Engineer  

---

## ⭐ Notes

This project is part of an academic assignment but has been extended and refined to reflect **real-world enterprise network security design practices**.
