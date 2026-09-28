<a id="top"></a>
<div align="center">

# 🌐 01 · Networking — Index
### Addressing, Switching, Routing, Services & Redundancy
**Track 01 of 3 — Cisco Networking Lab Portfolio**

![Addressing](https://img.shields.io/badge/Addressing-VLSM_%26_CIDR-005EB8?style=for-the-badge)
![Switching](https://img.shields.io/badge/Switching-VLANs_%26_Inter--VLAN-6f42c1?style=for-the-badge)
![Routing](https://img.shields.io/badge/Routing-Static_RIP_EIGRP_OSPF-117864?style=for-the-badge)
![Services](https://img.shields.io/badge/Services-DHCP_NAT_HSRP_Syslog-E95420?style=for-the-badge)
![Tool](https://img.shields.io/badge/Tool-Packet_Tracer-B9770E?style=for-the-badge)
![Status](https://img.shields.io/badge/Labs-11_of_11-brightgreen?style=for-the-badge)

**Quick guide to every lab in this track.**

### [📖 Open the full README](README.md)

</div>

---

<div align="center">

| 🧪 Labs | 🧩 Topic Groups | 🛠 Main Tool | 🔀 Routing Protocols Covered |
|:---:|:---:|:---:|:---:|
| **11** | **4** | **Cisco Packet Tracer** | **4** |

</div>

<p align="center">🧩 <b>Track:</b> Simulated Cisco 2911 routers and 2960 switches · each lab has its own README and screenshots</p>

---

## 📑 Lab Index

| # | Lab | Group | Key Topics | Folder |
|:---:|---|:---:|---|:---:|
| 1 | IP Addressing, VLSM & CIDR | 🔵 Addressing | `172.16.0.0/20` split into /22, /23, /24 subnets and three /30 WAN links | [📁 Lab](./01-Enterprise-ip-addressing-vlsm-cidr/) |
| 2 | DHCP Multi-VLAN Deployment | 🟣 Switching | Three VLANs, Router-on-a-Stick, per-VLAN DHCP pools | [📁 Lab](./02-DHCP-multi-vlan-deployment/) |
| 3 | Enterprise VLAN & Inter-VLAN Routing | 🟣 Switching | VTP, VLANs 10 / 20 / 99, inter-VLAN routing, SSH v2, port security, ACL | [📁 Lab](./03-Enterprise-network-vlan-intervlan-routing/) |
| 4 | VLAN & Inter-VLAN Troubleshooting | 🟣 Switching | Finding and fixing faults layer by layer | [📁 Lab](./04-Enterprise-network-troubleshooting-vlan-intervlan-routing/) |
| 5 | Routing Protocols | 🟠 Routing | Static, RIP, EIGRP and OSPF | [📁 Lab](./05-Routing-protocols-ospf-eigrp-rip-static/) |
| 6 | Enterprise OSPF Single-Area Routing | 🟠 Routing | Single-area OSPF across an enterprise network | [📁 Lab](./06-Enterprise-network-ospf-single-area-routing-lab/) |
| 7 | Multi-Area OSPF | 🟠 Routing | OSPF with more than one area | [📁 Lab](./07-Multi-area-ospf-lab/) |
| 8 | OSPF–EIGRP Redistribution | 🟠 Routing | Sharing routes between two protocols | [📁 Lab](./08-OSPF-eigrp-redistribution/) |
| 9 | NAT & PAT Address Translation | 🟢 Services | Address translation for private networks | [📁 Lab](./09-NAT-pat-address-translation/) |
| 10 | HSRP Redundancy & Failover | 🟢 Services | First-hop redundancy and gateway failover | [📁 Lab](./10-HSRP-redundancy-failover/) |
| 11 | Multi-Site Syslog Logging | 🟢 Services | Central logging across multiple sites | [📁 Lab](./11-Syslog-multisite-logging-enterprise/) |

---

## 🔵 Addressing — Lab 1 · 🟣 Switching & VLANs — Labs 2, 3, 4

| Lab | What It Proves |
|---|---|
| 01 · VLSM & CIDR | One address block turned into right-sized subnets, three routers connected with OSPF Area 0 |
| 02 · DHCP Multi-VLAN | Clients across three VLANs leasing addresses from the gateway router |
| 03 · VLAN & Inter-VLAN Routing | Departments segmented and routed, with an ACL blocking VLAN 20 → VLAN 10 only |
| 04 · VLAN Troubleshooting | VLAN and inter-VLAN faults found and fixed |

## 🟠 Routing — Labs 5, 6, 7, 8 · 🟢 Services & Redundancy — Labs 9, 10, 11

| Lab | What It Proves |
|---|---|
| 05 · Routing Protocols | Static, RIP, EIGRP and OSPF each routing traffic between networks |
| 06 · OSPF Single Area | An enterprise network routed with single-area OSPF |
| 07 · Multi-Area OSPF | OSPF working across more than one area |
| 08 · OSPF–EIGRP Redistribution | Routes exchanged between OSPF and EIGRP |
| 09 · NAT & PAT | Private hosts translated for outside access |
| 10 · HSRP | A gateway that fails over instead of being a single point of failure |
| 11 · Multi-Site Syslog | Logs collected centrally from several sites |

---

## 🔍 Lab Spotlights

The labs documented step by step here.

| Lab | Topology | Screenshots | Highlights |
|:---:|---|:---:|---|
| 01 · VLSM & CIDR | 3 buildings (HQ-R1 / R2 / R3), 2911 routers, 2960 switches | 13 | Building A /22, B /23, C /24, plus three /30 WAN links; PC-C's wrong mask was hidden by Proxy ARP, then corrected and re-verified |
| 02 · DHCP Multi-VLAN | Switch1 (2960), Router1 (2911), VLANs IT 10 / HR 20 / Sales 30 | 8 | Per-VLAN DHCP pools with excluded ranges; the first inter-VLAN ping timed out while ARP resolved, then succeeded on retry |
| 03 · VLAN & Inter-VLAN | 2 switches (2960) with VTP server / client, router 2911 | — | VLANs 10 Sales, 20 IT, 99 Management; per-VLAN DHCP, SSH v2, port security, BPDU guard, ACL blocking VLAN 20 → VLAN 10 |

---

## 🎯 Verification Checklist

| Check | Method | Lab | Status |
|:---:|---|:---:|:---:|
| End-to-end connectivity | Ping between PCs, `show ip route ospf` on all three routers | 01 | ✅ Confirmed |
| Correct subnet mask | Mask corrected to `255.255.255.0` and re-verified | 01 | ✅ Confirmed |
| Client leases per VLAN | `show ip dhcp binding`, `show ip interface brief`, inter-VLAN ping | 02 | ✅ Confirmed |
| Verification for labs 03–11 | See each lab's README | 03–11 | 📖 Per lab |

> [!NOTE]
> All labs are simulated in Cisco Packet Tracer. Screenshots and `.pkt` files are stored inside each lab's own folder.

---

<div align="center">

[⬆️ Back to top](#top) &nbsp;·&nbsp; [📖 Full README](README.md) &nbsp;·&nbsp; [⬅️ Portfolio Root](../README.md)

📶 **[What is DHCP](https://www.cloudflare.com/learning/network-layer/what-is-dhcp/)** · 🧮 **[What is a subnet](https://www.cloudflare.com/learning/network-layer/what-is-a-subnet/)** · 🔀 **[What is a LAN](https://www.cloudflare.com/learning/network-layer/what-is-a-lan/)**

</div>
