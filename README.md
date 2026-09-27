<div align="center">

# 🌐 Cisco Networking Lab Portfolio

**malaika-azhar**

A hands-on collection of Cisco Packet Tracer and Windows troubleshooting labs, organized into three tracks — core networking, network security, and IT support/troubleshooting. Every lab documents the topology, the configuration, the verification, and the gaps, not just the happy path.

![Networking](https://img.shields.io/badge/Track-Networking-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white)
![Security](https://img.shields.io/badge/Track-Network_Security-943126?style=for-the-badge&logo=shieldsdotio&logoColor=white)
![IT Support](https://img.shields.io/badge/Track-IT_Support-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Tool](https://img.shields.io/badge/Tool-Packet_Tracer_%2F_Windows_10-E95420?style=for-the-badge&logo=cisco&logoColor=white)
![Labs](https://img.shields.io/badge/Labs-26_Total-2ea44f?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In_Progress-B9770E?style=for-the-badge)

<br>

### [📂 Jump to the Labs ↓](#01-networking)

</div>

<br>

---

## 📑 Table of Contents

<table>
<tr>
<td valign="top" width="33%">

**Overview**
1. [At a Glance](#at-a-glance)
2. [About This Portfolio](#about)
3. [The Method](#method)

</td>
<td valign="top" width="33%">

**Tools & Labs**
4. [Tools & Technologies](#tools-technologies)
5. [01 — Networking](#01-networking)
6. [02 — Network Security](#02-network-security)
7. [03 — IT Support](#03-it-support)

</td>
<td valign="top" width="33%">

**Reference**
8. [Lab README Standard](#documentation-standard)
9. [Skills Demonstrated](#skills-demonstrated)
10. [Repo Structure](#repo-structure)

</td>
</tr>
</table>

---

<a id="at-a-glance"></a>
## 📊 At a Glance

<div align="center">

<table>
<tr>
<th>🌐 Networking</th>
<th>🔒 Network Security</th>
<th>🖥️ IT Support</th>
<th>📁 Total Labs</th>
</tr>
<tr align="center">
<td><h3>11</h3></td>
<td><h3>6</h3></td>
<td><h3>9</h3></td>
<td><h3>26</h3></td>
</tr>
</table>

</div>

---

<a id="about"></a>
## 📖 About This Portfolio

This repo is split into three tracks that build on each other:

<table>
<tr>
<td width="6%" align="center">🌐</td>
<td width="24%"><b>01 — Networking</b></td>
<td>Core routing, switching, and enterprise addressing fundamentals</td>
</tr>
<tr>
<td align="center">🔒</td>
<td><b>02 — Network Security</b></td>
<td>Hardening those same networks — ACLs, AAA, VPNs, port security</td>
</tr>
<tr>
<td align="center">🖥️</td>
<td><b>03 — IT Support &amp; Troubleshooting</b></td>
<td>Windows-side helpdesk scenarios — diagnosing and fixing real fault conditions</td>
</tr>
</table>

Each completed lab has its own folder and its own full README (see [Lab README Standard](#documentation-standard)) — this page is just the map.

---

<a id="method"></a>
## 🧭 The Method

```mermaid
%%{init: {'theme': 'base', 'themeVariables': {'fontSize': '15px'}, 'flowchart': {'nodeSpacing': 22, 'rankSpacing': 40, 'curve': 'linear'}}}%%
flowchart LR
    A["🎯<br/><b>Design</b>"]:::a --> B["⚙️<br/><b>Configure</b>"]:::b --> C["🐛<br/><b>Break</b>"]:::c --> D["🔎<br/><b>Diagnose</b>"]:::d --> E["🩹<br/><b>Fix</b>"]:::e --> F["✅<br/><b>Verify</b>"]:::f --> G["📝<br/><b>Document</b>"]:::g

    classDef a fill:#2C3E70,stroke:#131B3A,stroke-width:2px,color:#FFFFFF
    classDef b fill:#1A5276,stroke:#0B2E43,stroke-width:2px,color:#FFFFFF
    classDef c fill:#943126,stroke:#571C16,stroke-width:2px,color:#FFFFFF
    classDef d fill:#B9770E,stroke:#6E4409,stroke-width:2px,color:#FFFFFF
    classDef e fill:#76448A,stroke:#432752,stroke-width:2px,color:#FFFFFF
    classDef f fill:#117864,stroke:#083D33,stroke-width:2px,color:#FFFFFF
    classDef g fill:#1E8449,stroke:#0E4A28,stroke-width:2px,color:#FFFFFF
    linkStyle default stroke:#5D6D7E,stroke-width:2px
```
<p align="center"><em>Every lab — networking, security, or IT support — follows this same loop, so the evidence trail is consistent no matter the topic.</em></p>

---

<a id="tools-technologies"></a>
## 🛠️ Tools & Technologies

<table>
<tr><th align="left">Category</th><th align="left">Tools</th></tr>
<tr><td>🖥️ Simulation</td><td>Cisco Packet Tracer</td></tr>
<tr><td>🚪 Hardware modeled</td><td>Router 2911, Switch 2960</td></tr>
<tr><td>🪟 OS</td><td>Windows 10 Pro (22H2)</td></tr>
<tr><td>⌨️ Command-line</td><td>CMD, PowerShell</td></tr>
<tr><td>🗝️ System internals</td><td>Registry Editor, Group Policy Editor, Event Viewer</td></tr>
<tr><td>🔀 Switching</td><td>VLANs, 802.1Q trunking, VTP, port security, STP loop prevention</td></tr>
<tr><td>🔵 Routing</td><td>OSPF (single &amp; multi-area), EIGRP, RIP, static, redistribution, NAT/PAT, HSRP</td></tr>
<tr><td>🔒 Security</td><td>AAA, standard &amp; extended ACLs, SSH hardening, IPsec site-to-site VPN</td></tr>
<tr><td>🖧 IT Support</td><td>Active Directory, DNS, DHCP, email, RDP/VPN, print services, Windows Update/DISM/SFC</td></tr>
</table>

---

<a id="01-networking"></a>
## 🌐 01 — Networking

<img src="https://img.shields.io/badge/11_Labs-1BA0D7?style=flat-square&logo=cisco&logoColor=white" alt="11 labs">

| # | Lab | Focus | Status |
|:---:|---|---|:---:|
| 01 | [Enterprise IP Addressing, VLSM & CIDR](./01-Networking/01-Enterprise-ip-addressing-vlsm-cidr) | 172.16.0.0/20 right-sized via VLSM across 3 buildings + 3 WAN links, OSPF Area 0 | ![Complete](https://img.shields.io/badge/-Complete-2ea44f?style=flat-square) |
| 02 | [DHCP Multi-VLAN Deployment](./01-Networking/02-DHCP-multi-vlan-deployment) | 3 VLANs (IT/HR/Sales), Router-on-a-Stick, per-VLAN DHCP pools | ![Complete](https://img.shields.io/badge/-Complete-2ea44f?style=flat-square) |
| 03 | [VLAN & Inter-VLAN Routing](./01-Networking/03-Enterprise-network-vlan-intervlan-routing) | VTP sync, 3 VLANs, InterVLAN routing, SSH, port security, ACL | ![In Progress](https://img.shields.io/badge/-In_Progress-B9770E?style=flat-square) |
| 04 | [VLAN/InterVLAN Troubleshooting](./01-Networking/04-Enterprise-network-troubleshooting-vlan-intervlan-routing) | Diagnosing VLAN/InterVLAN routing faults | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 05 | [OSPF, EIGRP, RIP, Static Routing](./01-Networking/05-Routing-protocols-ospf-eigrp-rip-static) | Multi-protocol routing comparison | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 06 | [OSPF Single-Area Routing Lab](./01-Networking/06-Enterprise-network-ospf-single-area-routing-lab) | Single-area OSPF deployment | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 07 | [Multi-Area OSPF Lab](./01-Networking/07-Multi-area-ospf-lab) | Multi-area OSPF design and route summarization | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 08 | [OSPF/EIGRP Redistribution](./01-Networking/08-OSPF-eigrp-redistribution) | Redistributing routes between OSPF and EIGRP | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 09 | [NAT/PAT Address Translation](./01-Networking/09-NAT-pat-address-translation) | NAT and PAT configuration | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 10 | [HSRP Redundancy & Failover](./01-Networking/10-HSRP-redundancy-failover) | First-hop redundancy with HSRP | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 11 | [Syslog Multisite Logging](./01-Networking/11-Syslog-multisite-logging-enterprise) | Centralized logging across an enterprise topology | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |

---

<a id="02-network-security"></a>
## 🔒 02 — Network Security

<img src="https://img.shields.io/badge/6_Labs-943126?style=flat-square" alt="6 labs">

| # | Lab | Focus | Status |
|:---:|---|---|:---:|
| 01 | [AAA Local Authentication](./02-Network-Security/01-AAA_Local_Authentication) | Local AAA authentication configuration | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 02 | [Extended ACL — Telnet/Ping Control](./02-Network-Security/02-Extended_ACL_Telnet_Ping_Control) | Extended ACLs controlling Telnet and ICMP | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 03 | [IPsec VPN Site-to-Site](./02-Network-Security/03-IPsec_VPN_Site_to_Site) | Site-to-site IPsec VPN tunnel | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 04 | [Port Security & STP Loop Prevention](./02-Network-Security/04-Port_Security_STP_Loop_Prevention) | Port security plus STP loop prevention | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 05 | [SSH Hardening — Telnet Replacement](./02-Network-Security/05-SSH_Hardening_Telnet_Replacement) | Replacing Telnet with SSH v2 | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 06 | [Standard ACL Implementation](./02-Network-Security/06-Standard_ACL_Implementation) | Numbered → named standard ACL, host-based deny/permit, migration verified | ![Complete](https://img.shields.io/badge/-Complete-2ea44f?style=flat-square) |

---

<a id="03-it-support"></a>
## 🖥️ 03 — IT Support & Troubleshooting

<img src="https://img.shields.io/badge/9_Labs-0078D6?style=flat-square&logo=windows&logoColor=white" alt="9 labs">

| # | Lab | Focus | Status |
|:---:|---|---|:---:|
| 01 | [Active Directory User Account Issues](./03-IT-Support-Troubleshooting/01-Active-Directory-User-Account-Issues) | Diagnosing AD account/login problems | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 02 | [DNS Troubleshooting & Resolution](./03-IT-Support-Troubleshooting/02-DNS_Troubleshooting_Resolution) | DNS resolution failure diagnosis | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 03 | [Email Troubleshooting](./03-IT-Support-Troubleshooting/03-Email-Troubleshooting) | Email client/server issue diagnosis | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 04 | [Gateway IP Conflict Resolution](./03-IT-Support-Troubleshooting/04-Gateway_IP_Conflict_Resolution) | Resolving duplicate/conflicting gateway IPs | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 05 | [LAN/Wi-Fi Connectivity Diagnostics](./03-IT-Support-Troubleshooting/05-LAN-WiFi-Connectivity-Diagnostics) | Wired and wireless connectivity troubleshooting | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 06 | [Printer & Network Print Troubleshooting](./03-IT-Support-Troubleshooting/06-Printer_Network_Print_Troubleshooting) | Network print failure diagnosis | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 07 | [Remote Desktop & VPN Troubleshooting](./03-IT-Support-Troubleshooting/07-Remote_Desktop_VPN_Troubleshooting) | 6 RDP faults staged/fixed across firewall, service, registry, GPO, connection layers — 20 modules, 20 screenshots | ![Complete](https://img.shields.io/badge/-Complete-2ea44f?style=flat-square) |
| 08 | [System Diagnostics & Desktop Support](./03-IT-Support-Troubleshooting/08-System_Diagnostics_Desktop_Support) | General desktop diagnostics | ![Planned](https://img.shields.io/badge/-Planned-8E8E8E?style=flat-square) |
| 09 | [Windows Update & Patch Management](./03-IT-Support-Troubleshooting/09-Windows_Update_Patch_Management) | Service cycling, DISM/SFC repair, PSWindowsUpdate execution-policy fix — 17 modules, 17 screenshots | ![Complete](https://img.shields.io/badge/-Complete-2ea44f?style=flat-square) |

---

<a id="documentation-standard"></a>
## 📐 Lab README Standard

Every completed lab README follows the same layout, so any lab can be read the same way:

<table>
<tr><td align="center">📊</td><td><b>At a Glance</b></td><td>Key numbers for the lab in one row</td></tr>
<tr><td align="center">🗺️</td><td><b>Topology / Access Path</b></td><td>A diagram of the network or fault path</td></tr>
<tr><td align="center">⚙️</td><td><b>Module Walkthrough</b></td><td>Numbered steps, each with a command block and a screenshot exhibit</td></tr>
<tr><td align="center">🌟</td><td><b>Coverage Snapshot</b></td><td>A table mapping every claim to the exhibit that proves it</td></tr>
<tr><td align="center">📟</td><td><b>Command Cheat Sheet</b></td><td>Every command used, with its purpose</td></tr>
<tr><td align="center">⚠️</td><td><b>Challenges & Fixes</b></td><td>What went wrong and how it was resolved</td></tr>
<tr><td align="center">🚧</td><td><b>Scope & Limitations</b></td><td>What the lab does <b>not</b> claim to prove</td></tr>
<tr><td align="center">🧠</td><td><b>What I Learned</b></td><td>Takeaways in plain language</td></tr>
<tr><td align="center">🛠️</td><td><b>Skills Demonstrated</b></td><td>A bullet list mapped to the work shown</td></tr>
<tr><td align="center">🖼️</td><td><b>Screenshot Index</b></td><td>Every exhibit, numbered and described</td></tr>
</table>

---

<a id="skills-demonstrated"></a>
## 🧠 Skills Demonstrated Across the Portfolio

<div align="center">

![](https://img.shields.io/badge/VLSM_%2F_CIDR-1BA0D7?style=flat-square)
![](https://img.shields.io/badge/VLANs_%26_Trunking-1BA0D7?style=flat-square)
![](https://img.shields.io/badge/Inter--VLAN_Routing-1BA0D7?style=flat-square)
![](https://img.shields.io/badge/OSPF_%2F_EIGRP_%2F_RIP-1BA0D7?style=flat-square)
![](https://img.shields.io/badge/NAT_%2F_PAT-1BA0D7?style=flat-square)
![](https://img.shields.io/badge/HSRP-1BA0D7?style=flat-square)
<br>
![](https://img.shields.io/badge/AAA_%26_ACLs-943126?style=flat-square)
![](https://img.shields.io/badge/SSH_Hardening-943126?style=flat-square)
![](https://img.shields.io/badge/Site--to--Site_IPsec_VPN-943126?style=flat-square)
![](https://img.shields.io/badge/Port_Security-943126?style=flat-square)
<br>
![](https://img.shields.io/badge/Registry_%2F_GPO_Repair-0078D6?style=flat-square)
![](https://img.shields.io/badge/Firewall_Management-0078D6?style=flat-square)
![](https://img.shields.io/badge/CMD_%26_PowerShell-0078D6?style=flat-square)
![](https://img.shields.io/badge/Exhibit--Based_Documentation-0078D6?style=flat-square)

</div>

---

<a id="repo-structure"></a>
## 📁 Repo Structure

```text
Cisco-Networking-Lab-Portfolio/
|-- README.md
|-- LICENSE
|-- 01-Networking/
|   |-- 01-Enterprise-ip-addressing-vlsm-cidr/
|   |-- 02-DHCP-multi-vlan-deployment/
|   |-- 03-Enterprise-network-vlan-intervlan-routing/
|   |-- 04-Enterprise-network-troubleshooting-vlan-intervlan-routing/
|   |-- 05-Routing-protocols-ospf-eigrp-rip-static/
|   |-- 06-Enterprise-network-ospf-single-area-routing-lab/
|   |-- 07-Multi-area-ospf-lab/
|   |-- 08-OSPF-eigrp-redistribution/
|   |-- 09-NAT-pat-address-translation/
|   |-- 10-HSRP-redundancy-failover/
|   `-- 11-Syslog-multisite-logging-enterprise/
|-- 02-Network-Security/
|   |-- 01-AAA_Local_Authentication/
|   |-- 02-Extended_ACL_Telnet_Ping_Control/
|   |-- 03-IPsec_VPN_Site_to_Site/
|   |-- 04-Port_Security_STP_Loop_Prevention/
|   |-- 05-SSH_Hardening_Telnet_Replacement/
|   `-- 06-Standard_ACL_Implementation/
`-- 03-IT-Support-Troubleshooting/
    |-- 01-Active-Directory-User-Account-Issues/
    |-- 02-DNS_Troubleshooting_Resolution/
    |-- 03-Email-Troubleshooting/
    |-- 04-Gateway_IP_Conflict_Resolution/
    |-- 05-LAN-WiFi-Connectivity-Diagnostics/
    |-- 06-Printer_Network_Print_Troubleshooting/
    |-- 07-Remote_Desktop_VPN_Troubleshooting/
    |-- 08-System_Diagnostics_Desktop_Support/
    `-- 09-Windows_Update_Patch_Management/
```

<div align="center">

📶 **[Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)** · 🪟 **[Windows Server Docs](https://learn.microsoft.com/en-us/windows-server/)** · 🔀 **[OSPF Overview](https://www.cloudflare.com/learning/network-layer/what-is-ospf/)**

</div>

</div>
