# 🏦 Enterprise Banking Network

I designed and implemented an enterprise banking network simulated in **Cisco Packet Tracer**, designed for a single building with **4 floors**, each representing a department (HR, Accounts, Marketing, etc.). The project covers end-to-end network design — from physical topology and IP addressing to routing, security, and wireless access.

---

# Network Topology Design using Draw.io 👇🏻

https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=BankNetworkTopology.drawio&dark=auto#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1MsbMCMovGhrak4Cqg_Vpcw7eF8sVhjXi%26export%3Ddownload

## 📐 Network Topology

![Network Topology](/Screenshot%202026-03-21%20104106.png)

---

## 🏗️ Network Overview

| Detail | Description |
|---|---|
| **Building** | Single building — 4 floors |
| **Devices per Floor** | 1 Router, 1 L3 Switch, multiple L2 Switches |
| **VLANs** | 12 VLANs — one per department (HR, Accounts, Marketing, etc.) |
| **Routing Protocol** | OSPF — Area 0 |
| **IP Scheme** | 192.168.10.0 – 192.168.12.255 (/26 per VLAN) |
| **Backbone Links** | 10.10.10.0/8 — /30 point-to-point subnets |
| **Simulation Tool** | Cisco Packet Tracer |

---

## ⚙️ Configuration Steps

1. Basic settings on all devices + SSH on routers and L3 switches
2. VLAN assignment + trunk and access port configuration
3. Switchport security on all L2 switches
4. Subnetting and IP addressing
5. OSPF routing on routers and L3 switches
6. Static IP addressing for server room devices
7. DHCP server configuration
8. Inter-VLAN routing on L3 switches + ip helper-address (DHCP relay)
9. Wireless network configuration
10. Verification and testing

---

## 🔐 Security Features

- **SSH** configured on all routers and L3 switches (Telnet disabled)
- **Port Security** — MAC sticky, max 2 devices, violation: shutdown
- **Password Encryption** — `service password-encryption` on all devices
- **MOTD Banner** — unauthorized access warning on all devices

---

## 🌐 Technologies Used

`Cisco IOS` `VLANs (802.1Q)` `OSPF` `Inter-VLAN Routing` `DHCP` `SSH` `Subnetting` `Port Security` `Wireless (802.11)` `Static IP Addressing`

---

## 📁 Repository Structure

```
enterprise-banking-network/
├── README.md
├── packet-tracer/
│   └── enterprise-banking-network.pkt
└── screenshots/
    └── topology.png
```

---

## 🚀 How to Open

1. Install [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
2. Clone or download this repository
3. Open `packet-tracer/enterprise-banking-network.pkt`

---


**Shravani Dhandrut**  
[LinkedIn](https://linkedin.com/in/yourprofile) • [GitHub](https://github.com/yourusername)
