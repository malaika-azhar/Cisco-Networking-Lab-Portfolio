<div align="center">

# 🌐 Cisco Networking Lab Portfolio

A hands-on collection of Cisco Packet Tracer and Windows troubleshooting labs, organized into three tracks — core networking, network security, and IT support/troubleshooting. Every lab documents the topology, the configuration, the verification, and the gaps, not just the happy path.

<sub>by <a href="https://github.com/malaika-azhar">@malaika-azhar</a></sub>

<br>

![Labs](https://img.shields.io/badge/26_Labs-2ea44f?style=flat-square)
![Tool](https://img.shields.io/badge/Packet_Tracer-E95420?style=flat-square)
![Windows](https://img.shields.io/badge/Windows_10-0078D6?style=flat-square)
![Status](https://img.shields.io/badge/In_Progress-B9770E?style=flat-square)

</div>

---

## 📑 Table of Contents

1. [At a Glance](#at-a-glance)
2. [Portfolio Architecture](#architecture)
3. [The Method](#method)
4. [Tools & Technologies](#tools)
5. [01 — Networking](#01-networking)
6. [02 — Network Security](#02-security)
7. [03 — IT Support & Troubleshooting](#03-support)
8. [Skills Demonstrated](#skills)
9. [Repo Structure](#repo-structure)

---

<a id="at-a-glance"></a>
## 📊 At a Glance

<div align="center">

| 🌐 Networking | 🔒 Network Security | 🖥️ IT Support | 📁 Total Labs |
|:---:|:---:|:---:|:---:|
| **11 Labs** | **6 Labs** | **9 Labs** | **26** |

</div>

---

<a id="architecture"></a>
## 🏗️ Portfolio Architecture

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '14px'}, 'flowchart': {'nodeSpacing': 24, 'rankSpacing': 42, 'curve': 'linear'}}}%%
flowchart TB
    Root(["🌐 Cisco Networking<br/>Lab Portfolio"]):::root

    Root --> N["01 · Networking<br/><sub>11 labs</sub>"]:::net
    Root --> S["02 · Network Security<br/><sub>6 labs</sub>"]:::sec
    Root --> I["03 · IT Support<br/><sub>9 labs</sub>"]:::sup

    N --> N1["Addressing · VLANs · DHCP<br/>OSPF · EIGRP · NAT · HSRP"]:::netleaf
    S --> S1["AAA · ACLs · VPN<br/>Port Security · SSH"]:::secleaf
    I --> I1["AD · DNS · Email · LAN/Wi-Fi<br/>Print · RDP/VPN · Updates"]:::supleaf

    classDef root fill:#1B2A4A,stroke:#0B1730,stroke-width:2px,color:#FFFFFF,font-weight:bold
    classDef net fill:#1BA0D7,stroke:#0B4D66,stroke-width:2px,color:#FFFFFF,font-weight:bold
    classDef sec fill:#943126,stroke:#571C16,stroke-width:2px,color:#FFFFFF,font-weight:bold
    classDef sup fill:#0078D6,stroke:#003D6B,stroke-width:2px,color:#FFFFFF,font-weight:bold
    classDef netleaf fill:#EAF6FC,stroke:#1BA0D7,stroke-width:1px,color:#0B4D66
    classDef secleaf fill:#FBEAE9,stroke:#943126,stroke-width:1px,color:#571C16
    classDef supleaf fill:#E9F2FB,stroke:#0078D6,stroke-width:1px,color:#003D6B
    linkStyle default stroke:#8896A6,stroke-width:1.5px
```

---

<a id="method"></a>
## 🧭 The Method

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '14px'}, 'flowchart': {'nodeSpacing': 20, 'rankSpacing': 36, 'curve': 'linear'}}}%%
flowchart LR
    A(["Design"]):::a --> B(["Configure"]):::b --> C(["Break"]):::c --> D(["Diagnose"]):::d --> E(["Fix"]):::e --> F(["Verify"]):::f --> G(["Document"]):::g

    classDef a fill:#2C3E70,stroke:#131B3A,stroke-width:2px,color:#FFFFFF
    classDef b fill:#1A5276,stroke:#0B2E43,stroke-width:2px,color:#FFFFFF
    classDef c fill:#943126,stroke:#571C16,stroke-width:2px,color:#FFFFFF
    classDef d fill:#B9770E,stroke:#6E4409,stroke-width:2px,color:#FFFFFF
    classDef e fill:#76448A,stroke:#432752,stroke-width:2px,color:#FFFFFF
    classDef f fill:#117864,stroke:#083D33,stroke-width:2px,color:#FFFFFF
    classDef g fill:#1E8449,stroke:#0E4A28,stroke-width:2px,color:#FFFFFF
    linkStyle default stroke:#8896A6,stroke-width:1.5px
```

---

<a id="tools"></a>
## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Simulation | Cisco Packet Tracer |
| Hardware modeled | Router 2911, Switch 2960 |
| OS | Windows 10/11 Pro |
| Command-line | CMD, PowerShell |
| System internals | Registry Editor, Group Policy Editor, Event Viewer, WinDbg |
| Switching | VLANs, 802.1Q trunking, VTP, port security, STP loop prevention |
| Routing | OSPF (single & multi-area), EIGRP, RIP, static, redistribution, NAT/PAT, HSRP |
| Security | AAA, standard & extended ACLs, SSH hardening, IPsec site-to-site VPN |
| IT Support | Active Directory, DNS, DHCP, email, RDP/VPN, print services, SFC/DISM, minidump analysis |

---

<a id="01-networking"></a>
## 🌐 01 — Networking

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '13px'}, 'flowchart': {'nodeSpacing': 14, 'rankSpacing': 30}}}%%
flowchart LR
    A["Addressing<br/>VLSM/CIDR"]:::n --> B["VLANs<br/>& DHCP"]:::n --> C["Inter-VLAN<br/>Routing"]:::n --> D["Routing Protocols<br/>OSPF·EIGRP·RIP"]:::n --> E["NAT/PAT<br/>& HSRP"]:::n --> F["Syslog<br/>Logging"]:::n
    classDef n fill:#1BA0D7,stroke:#0B4D66,stroke-width:1.5px,color:#FFFFFF
    linkStyle default stroke:#8896A6,stroke-width:1.5px
```

| # | Lab | Focus | Status |
|:---:|---|---|:---:|
| 01 | [Enterprise IP Addressing, VLSM & CIDR](./01-Networking/01-Enterprise-ip-addressing-vlsm-cidr) | 172.16.0.0/20 split via VLSM across 3 buildings + 3 WAN links, OSPF Area 0 | ✅ |
| 02 | [DHCP Multi-VLAN Deployment](./01-Networking/02-DHCP-multi-vlan-deployment) | 3 VLANs, Router-on-a-Stick, per-VLAN DHCP pools | ✅ |
| 03 | [VLAN & Inter-VLAN Routing](./01-Networking/03-Enterprise-network-vlan-intervlan-routing) | VTP sync, InterVLAN routing, SSH, port security, ACL | 🔄 |
| 04 | [VLAN/InterVLAN Troubleshooting](./01-Networking/04-Enterprise-network-troubleshooting-vlan-intervlan-routing) | Diagnosing VLAN/InterVLAN routing faults | ⏳ |
| 05 | [OSPF, EIGRP, RIP, Static Routing](./01-Networking/05-Routing-protocols-ospf-eigrp-rip-static) | Multi-protocol routing comparison | ⏳ |
| 06 | [OSPF Single-Area Routing](./01-Networking/06-Enterprise-network-ospf-single-area-routing-lab) | Single-area OSPF deployment | ⏳ |
| 07 | [Multi-Area OSPF](./01-Networking/07-Multi-area-ospf-lab) | Multi-area OSPF design and summarization | ⏳ |
| 08 | [OSPF/EIGRP Redistribution](./01-Networking/08-OSPF-eigrp-redistribution) | Redistributing routes between OSPF and EIGRP | ⏳ |
| 09 | [NAT/PAT Translation](./01-Networking/09-NAT-pat-address-translation) | NAT and PAT configuration | ⏳ |
| 10 | [HSRP Redundancy & Failover](./01-Networking/10-HSRP-redundancy-failover) | First-hop redundancy | ⏳ |
| 11 | [Syslog Multisite Logging](./01-Networking/11-Syslog-multisite-logging-enterprise) | Centralized logging across an enterprise topology | ⏳ |

---

<a id="02-security"></a>
## 🔒 02 — Network Security

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '13px'}, 'flowchart': {'nodeSpacing': 14, 'rankSpacing': 30}}}%%
flowchart LR
    A["AAA<br/>Authentication"]:::s --> B["ACLs<br/>Standard/Extended"]:::s --> C["Port Security<br/>& STP"]:::s --> D["SSH<br/>Hardening"]:::s --> E["IPsec VPN<br/>Site-to-Site"]:::s
    classDef s fill:#943126,stroke:#571C16,stroke-width:1.5px,color:#FFFFFF
    linkStyle default stroke:#8896A6,stroke-width:1.5px
```

| # | Lab | Focus | Status |
|:---:|---|---|:---:|
| 01 | [AAA Local Authentication](./02-Network-Security/01-AAA_Local_Authentication) | Local AAA authentication | ⏳ |
| 02 | [Extended ACL — Telnet/Ping](./02-Network-Security/02-Extended_ACL_Telnet_Ping_Control) | Extended ACLs controlling Telnet and ICMP | ⏳ |
| 03 | [IPsec VPN Site-to-Site](./02-Network-Security/03-IPsec_VPN_Site_to_Site) | Site-to-site IPsec VPN tunnel | ⏳ |
| 04 | [Port Security & STP Loop Prevention](./02-Network-Security/04-Port_Security_STP_Loop_Prevention) | Port security plus STP loop prevention | ⏳ |
| 05 | [SSH Hardening](./02-Network-Security/05-SSH_Hardening_Telnet_Replacement) | Replacing Telnet with SSH v2 | ⏳ |
| 06 | [Standard ACL Implementation](./02-Network-Security/06-Standard_ACL_Implementation) | Numbered → named ACL, host-based deny/permit | ✅ |

---

<a id="03-support"></a>
## 🖥️ 03 — IT Support & Troubleshooting

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '13px'}, 'flowchart': {'nodeSpacing': 20, 'rankSpacing': 32}}}%%
flowchart TB
    SYMPTOM(("🗣️ User-reported<br/>symptom")):::top
    SYMPTOM --> LOGIN["🔑 Login/AD issue"]:::branch
    SYMPTOM --> NET["🌐 No connectivity"]:::branch
    SYMPTOM --> APP["📧 App/print/email issue"]:::branch
    SYMPTOM --> SLOW["🐢 Slow / crashing / BSOD"]:::branch

    LOGIN --> T1["Active Directory<br/>Lab 01"]:::tool
    NET --> T2["DNS · Gateway · LAN/Wi-Fi<br/>Labs 02, 04, 05"]:::tool
    APP --> T3["Email · Print · RDP/VPN<br/>Labs 03, 06, 07"]:::tool
    SLOW --> T4["System Diagnostics · Updates<br/>Labs 08, 09"]:::tool

    T1 & T2 & T3 & T4 --> ROOT(("🎯 Root cause<br/>identified")):::bottom

    classDef top fill:#2C3E50,stroke:#16202A,stroke-width:2px,color:#FFFFFF
    classDef branch fill:#B9770E,stroke:#6E4409,stroke-width:2px,color:#FFFFFF
    classDef tool fill:#0078D6,stroke:#003D6B,stroke-width:2px,color:#FFFFFF
    classDef bottom fill:#117864,stroke:#083D33,stroke-width:2px,color:#FFFFFF
    linkStyle default stroke:#8896A6,stroke-width:1.5px
```

| # | Lab | Focus | Status |
|:---:|---|---|:---:|
| 01 | [AD User Account Issues](./03-IT-Support-Troubleshooting/01-Active-Directory-User-Account-Issues) | Diagnosing AD account/login problems | ⏳ |
| 02 | [DNS Troubleshooting](./03-IT-Support-Troubleshooting/02-DNS_Troubleshooting_Resolution) | DNS resolution failure diagnosis | ⏳ |
| 03 | [Email Troubleshooting](./03-IT-Support-Troubleshooting/03-Email-Troubleshooting) | Email client/server issue diagnosis | ⏳ |
| 04 | [Gateway IP Conflict Resolution](./03-IT-Support-Troubleshooting/04-Gateway_IP_Conflict_Resolution) | Resolving duplicate gateway IPs | ⏳ |
| 05 | [LAN/Wi-Fi Diagnostics](./03-IT-Support-Troubleshooting/05-LAN-WiFi-Connectivity-Diagnostics) | Wired and wireless connectivity troubleshooting | ⏳ |
| 06 | [Printer & Network Print Troubleshooting](./03-IT-Support-Troubleshooting/06-Printer_Network_Print_Troubleshooting) | Network print failure diagnosis | ⏳ |
| 07 | [Remote Desktop & VPN Troubleshooting](./03-IT-Support-Troubleshooting/07-Remote_Desktop_VPN_Troubleshooting) | 6 RDP faults staged/fixed — firewall, service, registry, GPO | ✅ |
| 08 | [System Diagnostics & Desktop Support](./03-IT-Support-Troubleshooting/08-System_Diagnostics_Desktop_Support) | High CPU/RAM, driver faults, app crashes, BSOD, SFC/DISM | ✅ |
| 09 | [Windows Update & Patch Management](./03-IT-Support-Troubleshooting/09-Windows_Update_Patch_Management) | Service repair, DISM/SFC, PSWindowsUpdate fix | ✅ |

---

<a id="skills"></a>
## 🧠 Skills Demonstrated

VLSM/CIDR addressing · VLANs & trunking · Inter-VLAN routing · OSPF/EIGRP/RIP · NAT/PAT · HSRP · AAA & ACLs · SSH hardening · Site-to-site IPsec VPN · Active Directory & DNS troubleshooting · Windows service/registry/GPO repair · SFC/DISM image repair · BSOD & minidump analysis · CMD & PowerShell verification

---

<a id="repo-structure"></a>
## 📁 Repo Structure

```
Cisco-Networking-Lab-Portfolio/
├── 01-Networking/                   (11 labs)
├── 02-Network-Security/             (6 labs)
└── 03-IT-Support-Troubleshooting/   (9 labs)
```
