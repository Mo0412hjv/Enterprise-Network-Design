# Cisco Enterprise Network Design

A multi-department enterprise network simulation built in **Cisco Packet Tracer**, covering subnetting, routing, wireless security, remote access, and NAT/PAT for internet connectivity.

## 🧩 Project Overview

This project simulates a small enterprise network connecting multiple departments (represented by color-coded VLANs/subnets) across two routers, with a dedicated internet edge and a wireless segment secured via WPA2 Enterprise.

**Departments / Networks:**

| Network | Segment | Subnet |
|---|---|---|
| 🟠 Orange | Router0 – Switch0 | `192.168.1.0/24` |
| 🔵 Cyan | Router0 – Switch1 | `192.168.2.192/26` |
| 🟣 Purple | Internet Edge | `200.100.50.0/24` |
| — | Router0 ↔ Router1 Link | `192.168.3.252/30` |
| 🟢 Green | Router1 – Switch7 | `192.168.4.248/29` |
| 🟡 Yellow | Wireless (WRT300N) | `192.168.0.0/24` |

## ⚙️ Key Features Implemented

- **VLSM Subnetting** — efficient IP allocation across departments of varying size
- **OSPF Routing** — dynamic routing between Router0 and Router1 (Area 0)
- **DHCP** — server-based address assignment per subnet, plus wireless DHCP via WRT300N
- **SSH & Telnet Access** — remote management with privilege levels and local authentication
- **WPA2 Enterprise Wireless Security** — RADIUS/AAA-based authentication for wireless clients
- **NAT/PAT** — PAT (overload) for general outbound traffic, Static NAT for the AAA server
- **Console Security** — hostname, enable secret, and line-level password protection

## 🛠️ Technologies & Protocols

`Cisco Packet Tracer` `OSPF` `DHCP` `SSH/Telnet` `WPA2-Enterprise` `RADIUS/AAA` `NAT/PAT` `VLSM`

## 📁 Repository Contents

| File | Description |
|---|---|
| [`network-topology.pkt`](./network-topology.pkt) | Full Packet Tracer simulation file |
| [`project.txt`](./project.txt) | Detailed configuration report (all CLI commands & setup steps) |

## 📖 Detailed Configuration

The full step-by-step configuration — including router CLI commands, DHCP/AAA server setup, and OSPF/NAT configuration — is documented in [`project.txt`](./project.txt).

## 🔧 How to Open

1. Download [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer) (free with a Cisco Networking Academy account)
2. Clone or download this repository
3. Open `network-topology.pkt` to explore the live simulation

---
*Built as part of hands-on networking practice — subnetting, routing, wireless security, and NAT design for a multi-department enterprise environment.*
