# 🏦 Enterprise Banking Network

I designed and implemented an enterprise banking network simulated in **Cisco Packet Tracer**, designed for a single building with **4 floors**, each representing a department (HR, Accounts, Marketing, etc.). The project covers end-to-end network design — from physical topology and IP addressing to routing, security, and wireless access.

---

## Network Topology Design using Draw.io 👇🏻

https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=BankNetworkTopology.drawio&dark=auto#Uhttps%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1MsbMCMovGhrak4Cqg_Vpcw7eF8sVhjXi%26export%3Ddownload

---

## 📐 Network Topology Implementation in Cisco Packet Tracer

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

## ✅ TO DO

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

---

## ⚙️ Configuration Steps

| # | Step | Details |
|---|------|---------|
| 1 | **Basic Settings + SSH** | Hostname, passwords, banner, password encryption, SSH on all routers and L3 switches |
| 2 | **VLANs + Port Configuration** | VLAN assignment, trunk ports (Fa0/1-2), access ports (Fa0/3-24) on all switches |
| 3 | **Switchport Security** | MAC sticky, max 2 devices, violation shutdown on all 12 L2 switches |
| 4 | **Subnetting & IP Addressing** | /26 subnets for VLANs, /30 for backbone point-to-point links |
| 5 | **OSPF Routing** | Dynamic routing configured on all routers and L3 switches in Area 0 |
| 6 | **Static IPs — Server Room** | Fixed IP addresses for DHCP, DNS, and file servers |
| 7 | **DHCP Server** | Centralized DHCP with separate pools for each VLAN subnet |
| 8 | **Inter-VLAN Routing** | L3 switch SVIs with `ip helper-address` relay to DHCP server |
| 9 | **Wireless Network** | Access points configured at each branch |
| 10 | **Verification & Testing** | `show` commands + ping tests across all VLANs and branches |

---

## 🔐 Security Features

- **SSH** configured on all routers and L3 switches (Telnet disabled)
- **Port Security** — MAC sticky, max 2 devices, violation: shutdown
- **Password Encryption** — `service password-encryption` on all devices
- **MOTD Banner** — unauthorized access warning on all devices

---

## 🌐 Technologies Used

`Cisco Packet Tracer` `VLANs` `OSPF` `Inter-VLAN Routing` `DHCP` `SSH` `Subnetting` `Port Security` `Wireless Connection` `Static IP Addressing`

---
