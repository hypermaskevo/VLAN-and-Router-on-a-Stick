# Lesson 2 – VLAN and Router-on-a-Stick

## 🧠 Goal

Design and configure a simple network with two VLANs (VLAN10 and VLAN20) that can communicate with each other using a Router-on-a-Stick setup.
![image](https://github.com/user-attachments/assets/d407695f-c017-4ddd-bd92-f457413feb5f)


## 🖥️ Topology

- 1 Router (any model with at least 1 FastEthernet or GigabitEthernet interface)
- 1 Switch (supports VLANs and trunking)
- 2 PCs (PC0 and PC1)

## 🔧 Requirements

- PC0:
  - VLAN10
  - IP: 192.168.10.2
  - Subnet: 255.255.255.0
  - Gateway: 192.168.10.1

- PC1:
  - VLAN20
  - IP: 192.168.20.2
  - Subnet: 255.255.255.0
  - Gateway: 192.168.20.1

- Trunk:
  - Switch port F0/24 is trunk to the router

- Router:
  - Subinterfaces for both VLANs with proper encapsulation and IP configuration

## ✅ Tasks

1. Create VLAN10 and VLAN20 on the switch
2. Assign switch ports to the correct VLANs
3. Configure trunking on the router-facing port
4. Configure router subinterfaces with the correct IPs
5. Test connectivity using `ping` between the PCs

## 📁 Files

- `lesson2-router-on-a-stick.pkt` – Packet Tracer file
- `README.md` – This file
- `screenshots/` – Optional: screenshots of configuration and testing

## 🚧 Troubleshooting Notes

- Make sure trunking is enabled and encapsulation is correct (e.g., dot1q)
- Ensure the PCs have correct default gateways
- Don't forget to turn on all interfaces (`no shutdown`)

## 📌 Objectives

By the end of this lab, you should understand:
- How VLAN segmentation works
- The basics of Router-on-a-Stick
- Inter-VLAN routing through a single physical router interface

