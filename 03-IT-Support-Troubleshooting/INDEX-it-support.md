<a id="top"></a>
<div align="center">

# 🖥️ 03 · IT Support & Troubleshooting — Index
### Accounts, Network, Services & Windows Systems
**Track 03 of 3 — Cisco Networking Lab Portfolio**

![Identity](https://img.shields.io/badge/Identity-Active_Directory-6f42c1?style=for-the-badge)
![Network](https://img.shields.io/badge/Network-DNS_IP_LAN_Wi--Fi-005EB8?style=for-the-badge)
![Services](https://img.shields.io/badge/Services-Email_%26_Printing-E95420?style=for-the-badge)
![Windows](https://img.shields.io/badge/Windows-RDP_VPN_Updates-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Status](https://img.shields.io/badge/Labs-9_of_9-brightgreen?style=for-the-badge)

**Quick guide to every lab in this track.**

### [📖 Open the full README](README.md)

</div>

---

<div align="center">

| 🧪 Labs | 🧩 Topic Groups | 🔧 RDP Faults Fixed (Lab 07) | 🩺 Fault Categories Diagnosed (Lab 08) |
|:---:|:---:|:---:|:---:|
| **9** | **4** | **6** | **5** |

</div>

<p align="center">🧩 <b>Track:</b> Real-world IT support scenarios · each lab has its own README and screenshots</p>

---

## 📑 Lab Index

| # | Lab | Group | Key Topics | Folder |
|:---:|---|:---:|---|:---:|
| 1 | Active Directory & User Account Issues | 🟣 Identity | Samba4 AD, domain provisioning, create / disable / enable users | [📁 Lab](./01-Active-Directory-User-Account-Issues/) |
| 2 | DNS Troubleshooting & Resolution | 🔵 Network | `nslookup`, `dig`, forward and reverse lookup, DNS flush | [📁 Lab](./02-DNS_Troubleshooting_Resolution/) |
| 3 | Email Troubleshooting | 🟠 Services | SMTP, IMAP, POP3, DNS MX records, port testing | [📁 Lab](./03-Email-Troubleshooting/) |
| 4 | Gateway & IP Conflict Resolution | 🔵 Network | APIPA, duplicate IPs, default gateway misconfiguration | [📁 Lab](./04-Gateway_IP_Conflict_Resolution/) |
| 5 | LAN & Wi-Fi Connectivity Diagnostics | 🔵 Network | `ipconfig`, `arp`, SSID issues, channel interference | [📁 Lab](./05-LAN-WiFi-Connectivity-Diagnostics/) |
| 6 | Printer & Network Print Troubleshooting | 🟠 Services | Print spooler, driver issues, network printers across subnets | [📁 Lab](./06-Printer_Network_Print_Troubleshooting/) |
| 7 | Remote Desktop & VPN Troubleshooting | 🟢 Windows | Six RDP faults, CMD, PowerShell, Registry, Group Policy, Event Viewer | [📁 Lab](./07-Remote_Desktop_VPN_Troubleshooting/) |
| 8 | System Diagnostics & Desktop Support | 🟢 Windows | CPU/RAM, drivers, app crashes, BSOD, corrupted files, WinDbg | [📁 Lab](./08-System_Diagnostics_Desktop_Support/) |
| 9 | Windows Update & Patch Management | 🟢 Windows | Update services, cache reset, DISM, SFC, policy audit | [📁 Lab](./09-Windows_Update_Patch_Management/) |

---

## 🟣 Identity — Lab 1 · 🔵 Network — Labs 2, 4, 5

| Lab | What It Proves |
|---|---|
| 01 · Active Directory | A domain provisioned and user accounts managed |
| 02 · DNS | Name resolution faults found and fixed |
| 04 · Gateway & IP Conflict | Addressing and gateway faults resolved |
| 05 · LAN & Wi-Fi | Link and wireless problems diagnosed |

## 🟠 Services — Labs 3 and 6

| Lab | What It Proves |
|---|---|
| 03 · Email | Mail delivery problems traced to DNS, ports and protocols |
| 06 · Printer | Print failures fixed at spooler, driver and network level |

---

## 🟢 Windows Systems — Labs 7, 8 and 9

| Lab | Modules | Screenshots | Environment | Highlights |
|:---:|:---:|:---:|---|---|
| 07 · Remote Desktop & VPN | 20 | 20 | One Windows 10 Pro machine | Console-session error, wrong-IP error, firewall block, stopped `TermService`, `fDenyTSConnections`, Group Policy restriction |
| 08 · System Diagnostics | 20 | 21 | Windows 10/11 | Five fault categories diagnosed from real machine state; no faults artificially staged |
| 09 · Windows Update | 17 | 17 | Windows 10 Pro 22H2 | `wuauserv` / `bits` / `cryptsvc` cycled, caches cleared, DISM and SFC run, execution-policy block fixed |

---

## 🎯 Verification Checklist

| Check | Method | Lab | Status |
|:---:|---|:---:|:---:|
| Six RDP faults each diagnosed and fixed | CMD, PowerShell, Registry, Group Policy, Event Viewer | 07 | ✅ Documented |
| Real machine faults diagnosed from evidence | Event Viewer, Reliability Monitor, minidump analysis | 08 | ✅ Documented |
| Update pipeline repaired step by step | Services, cache, DISM, SFC, policy audit | 09 | ✅ Documented |
| Verification for labs 01–06 | See each lab's README | 01–06 | 📖 Per lab |

> [!NOTE]
> Labs 07, 08 and 09 used built-in Windows tools only. Screenshots are stored inside each lab's own folder.

---

<div align="center">

[⬆️ Back to top](#top) &nbsp;·&nbsp; [📖 Full README](README.md) &nbsp;·&nbsp; [⬅️ Portfolio Root](../README.md)

🌐 **[What is DNS](https://www.cloudflare.com/learning/dns/what-is-dns/)** · 📶 **[What is DHCP](https://www.cloudflare.com/learning/network-layer/what-is-dhcp/)** · 🪟 **[Windows Commands](https://learn.microsoft.com/windows-server/administration/windows-commands/windows-commands)**

</div>
