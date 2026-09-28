<a id="top"></a>
<div align="center">

# 🔐 02 · Network Security — Index
### Access Control, Hardening, Authentication & Secure Connectivity
**Track 02 of 3 — Cisco Networking Lab Portfolio**

![ACLs](https://img.shields.io/badge/Access_Control-ACLs-943126?style=for-the-badge)
![SSH](https://img.shields.io/badge/Hardening-SSH_%26_Port_Security-6f42c1?style=for-the-badge)
![AAA](https://img.shields.io/badge/Authentication-AAA-005EB8?style=for-the-badge)
![VPN](https://img.shields.io/badge/VPN-IPsec-117864?style=for-the-badge)
![Tool](https://img.shields.io/badge/Tool-Packet_Tracer-B9770E?style=for-the-badge)
![Status](https://img.shields.io/badge/Labs-6_of_6-brightgreen?style=for-the-badge)

**Quick guide to every lab in this track.**

### [📖 Open the full README](README.md)

</div>

---

<div align="center">

| 🧪 Labs | 🧩 Topic Groups | 🛠 Main Tool | 📋 Standard ACL Lab Modules |
|:---:|:---:|:---:|:---:|
| **6** | **4** | **Cisco Packet Tracer** | **17** |

</div>

<p align="center">🧩 <b>Track:</b> Simulated Cisco routers and switches · each lab has its own README and screenshots</p>

---

## 📑 Lab Index

| # | Lab | Group | Key Topics | Folder |
|:---:|---|:---:|---|:---:|
| 1 | AAA — Local Authentication | 🔵 Authentication | Usernames, passwords, privilege levels, local AAA | [📁 Lab](./01-AAA_Local_Authentication/) |
| 2 | Extended ACL — Telnet & Ping Control | 🔴 Access Control | Port-based filtering, traffic direction, named ACLs | [📁 Lab](./02-Extended_ACL_Telnet_Ping_Control/) |
| 3 | IPsec VPN Site-to-Site | 🟢 Connectivity | IKE phase 1 and 2, transform sets, crypto maps | [📁 Lab](./03-IPsec_VPN_Site_to_Site/) |
| 4 | Port Security & STP Loop Prevention | 🟣 Hardening | MAC filtering, sticky MAC, BPDU guard, PortFast | [📁 Lab](./04-Port_Security_STP_Loop_Prevention/) |
| 5 | SSH Hardening & Telnet Replacement | 🟣 Hardening | RSA keys, SSH v2, VTY line hardening | [📁 Lab](./05-SSH_Hardening_Telnet_Replacement/) |
| 6 | Standard ACL Implementation | 🔴 Access Control | Host-based deny, numbered to named ACL migration | [📁 Lab](./06-Standard_ACL_Implementation/) |

---

## 🔴 Access Control — Labs 2 and 6

| Lab | What It Proves |
|---|---|
| 02 · Extended ACL — Telnet & Ping Control | Traffic controlled by port and direction with named ACLs |
| 06 · Standard ACL Implementation | One host blocked by IP while another stays permitted |

## 🟣 Device Hardening — Labs 4 and 5

| Lab | What It Proves |
|---|---|
| 04 · Port Security & STP Loop Prevention | Switch ports limited by MAC address and protected from loops |
| 05 · SSH Hardening & Telnet Replacement | Encrypted remote management in place of Telnet |

## 🔵 Authentication — Lab 1

| Lab | What It Proves |
|---|---|
| 01 · AAA — Local Authentication | Device logins tied to accounts and privilege levels |

## 🟢 Secure Connectivity — Lab 3

| Lab | What It Proves |
|---|---|
| 03 · IPsec VPN Site-to-Site | An encrypted tunnel between two sites |

---

## 🔍 Lab 06 Spotlight — Standard ACL Implementation

The one lab in this track documented step by step here.

| Step | What Was Done |
|:---:|---|
| 1 | Built a 3-router, 2-switch, 5-host topology: Branch-R1, Core-R2, HQ-R3 |
| 2 | Wrote a standard ACL on Core-R2 denying Branch-PC1 by host IP and permitting Branch-PC0 (numbered ACL 10) |
| 3 | Migrated the rule to a named ACL, `BLOCK_PC1` |
| 4 | Removed the old numbered ACL |
| 5 | Re-verified the result after the migration |

---

## 🎯 Verification Checklist

| Check | Method | Lab | Status |
|:---:|---|:---:|:---:|
| Target host blocked | Standard ACL on Core-R2 | 06 | ✅ Confirmed |
| Other host still permitted | Standard ACL on Core-R2 | 06 | ✅ Confirmed |
| Old numbered ACL removed, result re-verified | Migration to `BLOCK_PC1` | 06 | ✅ Confirmed |
| Verification for labs 01–05 | See each lab's README | 01–05 | 📖 Per lab |

> [!NOTE]
> All labs are simulated in Cisco Packet Tracer. Screenshots are stored inside each lab's own folder.

---

<div align="center">

[⬆️ Back to top](#top) &nbsp;·&nbsp; [📖 Full README](README.md) &nbsp;·&nbsp; [⬅️ Portfolio Root](../README.md)

🔐 **[What is an ACL](https://www.cloudflare.com/learning/access-management/what-is-an-access-control-list/)** · 🔑 **[What is SSH](https://www.cloudflare.com/learning/access-management/what-is-ssh/)** · 🌐 **[What is a VPN](https://www.cloudflare.com/learning/access-management/what-is-a-vpn/)**

</div>
