<div align="center">

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:00ff41&height=200&section=header&text=Haider%20Jamal&fontSize=45&fontColor=00ff41&fontAlignY=35&desc=Penetration%20Tester%20%7C%20CEH%20Certified&descAlignY=55&descColor=8b949e&animation=fadeIn)

```
[root@haider]─[~]$ whoami
> Certified Ethical Hacker | Offensive Security Focus
> Breaking things in isolated labs so I can explain exactly how — and how to fix it
```

</div>

<br>

## `~/about`

```yaml
role:          Penetration Tester / Red Team (Aspiring)
certification: CEH (Certified Ethical Hacker) — Corvit, NAVTTC — Completed
also_studying: CCNP, Huawei (GNS3 / eNSP)
focus:         Recon → Enumeration → Vulnerability Analysis → Exploitation → Post-Exploitation
philosophy:    Labs > theory. Evidence > claims. Every exploit gets a remediation.
```

<br>

## `~/lab-infrastructure`

Everything below runs in an isolated, host-only virtualized lab — Kali as the attack box, Windows/Metasploitable2 as intentionally vulnerable targets, never against anything I don't own or have authorization for.

| Layer | Stack |
|---|---|
| **Virtualization** | VMware Workstation, EVE-NG, GNS3, Cisco Packet Tracer |
| **Attack box** | Kali Linux |
| **Targets** | Metasploitable 2, Windows 7/10/11 VMs (XAMPP-simulated services), Cisco 3640 (GNS3) |
| **Networking gear (virtual)** | Cisco routers/switches (IOS), HSRP/VRRP/GLBP labs |

<br>

## `~/skills`

![Networking](https://img.shields.io/badge/Networking-Subnetting_|_VLANs_|_NAT_|_ACLs_|_OSPF/RIP/BGP-161b22?style=for-the-badge&logo=cisco&logoColor=00ff41&labelColor=161b22)
![OS](https://img.shields.io/badge/Systems-Linux(Kali/Debian/RHEL)_|_Windows_Server_|_AD-161b22?style=for-the-badge&logo=linux&logoColor=00ff41&labelColor=161b22)
![Offensive](https://img.shields.io/badge/Offensive-Recon_|_Enumeration_|_Exploitation_|_Post--Exploitation-161b22?style=for-the-badge&logo=hackthebox&logoColor=00ff41&labelColor=161b22)
![WebSec](https://img.shields.io/badge/Web_Security-OWASP_Top_10_|_DAST_|_Manual_Validation-161b22?style=for-the-badge&logo=owasp&logoColor=00ff41&labelColor=161b22)
![Net](https://img.shields.io/badge/Network_Attacks-ARP_Poisoning_|_MITM_|_Packet_Analysis-161b22?style=for-the-badge&logo=wireshark&logoColor=00ff41&labelColor=161b22)

**Tools:**

![Nmap](https://img.shields.io/badge/Nmap-161b22?style=flat-square&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMDBmZjQxIiBzdHJva2Utd2lkdGg9IjIuNSIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIj48Y2lyY2xlIGN4PSIxMSIgY3k9IjExIiByPSI3Ij48L2NpcmNsZT48bGluZSB4MT0iMjEiIHkxPSIyMSIgeDI9IjE2IiB5Mj0iMTYiPjwvbGluZT48L3N2Zz4K)
![Wireshark](https://img.shields.io/badge/Wireshark-161b22?style=flat-square&logo=wireshark&logoColor=00ff41)
![Metasploit](https://img.shields.io/badge/Metasploit-161b22?style=flat-square&logo=metasploit&logoColor=00ff41)
![Burp](https://img.shields.io/badge/Burp_Suite-161b22?style=flat-square&logo=burpsuite&logoColor=00ff41)
![Kali](https://img.shields.io/badge/Kali_Linux-161b22?style=flat-square&logo=kalilinux&logoColor=00ff41)
![Ettercap](https://img.shields.io/badge/Ettercap-161b22?style=flat-square&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMDBmZjQxIiBzdHJva2Utd2lkdGg9IjIuNSIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIj48cG9seWxpbmUgcG9pbnRzPSIyMiAxMiAxOCAxMiAxNSAyMSA5IDMgNiAxMiAyIDEyIj48L3BvbHlsaW5lPjwvc3ZnPgo=)

`Nmap · Gobuster · Shodan · SearchSploit · Metasploit/Meterpreter · John the Ripper · Hydra · Nessus · OpenVAS/Greenbone · OWASP ZAP · Burp Suite · Wireshark · Ettercap · Lynis · Aircrack-ng`

<br>

## `~/evidence-portfolio`

> Documented, reproducible offensive work — not just "I installed the tool."

```
[+] Metasploitable 2 — Nessus Vulnerability Assessment
    436 findings | 28 Critical · 99 High · 148 Medium · 20 Low · 141 Info
    Critical: Apache PHP-CGI RCE, Shellshock, bind-shell backdoor,
              phpMyAdmin SQLi exposure, UnrealIRCd backdoor, weak VNC creds

[+] Metasploitable 2 — Controlled Exploitation & Pentest Report
    - Bind shell backdoor (ingreslock/1524)  → root shell, validated via Nmap + netcat
    - UnrealIRCd 3.2.8.1 backdoor            → Meterpreter session, root access
    - VNC weak credential ("password")       → validated via Metasploit aux scanner
    - Apache PHP-CGI argument injection      → vuln confirmed, alt. exploit path documented
    Each finding paired with remediation guidance.

[+] OWASP ZAP — Web Application Assessment (v2.17.0)
    Target: Metasploitable2 (DVWA, Mutillidae II, TWiki, phpMyAdmin, WebDAV)
    23 findings | Highest: High (MD5-crypt hash disclosure)
    Medium: missing CSP, directory browsing, vulnerable JS library, no anti-clickjacking

[+] ARP Poisoning / MITM Lab — Ettercap + Wireshark
    Topology: Kali (attacker) · Windows 7 (victim 1) · Windows 10 (victim 2) — isolated host-only network

    Baseline:
    - Recorded IPv4 + MAC for both Windows hosts (ipconfig /all) and Kali's eth0 (ifconfig)
    - Verified clean ARP state on both victims (arp -a) — each held the other's true MAC, no Kali entry
    - Confirmed baseline reachability with ICMP between victims (no poisoning yet)

    Attack:
    - Launched Ettercap (GUI mode) on Kali, sniffing on eth0
    - Performed a host scan, identified both Windows machines from the host list
    - Assigned Win7 → Target 1, Win10 → Target 2
    - Enabled IP forwarding on Kali (net.ipv4.ip_forward = 1) so poisoned traffic would route
      through the attacker instead of black-holing
    - Launched MITM → ARP Poisoning attack

    Validation:
    - Re-checked arp -a on both victims — each host's ARP table now resolved the other's IP
      to Kali's MAC address, confirming successful cache poisoning
    - Started a live Wireshark capture on Kali's eth0
    - Generated ICMP traffic between the two Windows hosts and observed it transiting through
      the attacker, visible directly in the Wireshark capture

    Takeaway: demonstrates the core weakness ARP exploits — no authentication on ARP replies —
    and the practical mechanics of a Layer 2 MITM: poison → verify cache corruption → enable
    forwarding to stay transparent → intercept with a packet analyzer.

[+] Network Forensics — Malware Delivery + C2 Investigation (PCAP)
    Victim requested /update.exe x4 over HTTP:8000 → outbound TCP:4444 to C2 host
    ~566KB transferred in <1s post-handshake, ~67s sustained bidirectional session
    Pattern consistent with staged Meterpreter payload + interactive C2

[+] Nessus / Wireshark — Windows Network Scan Analysis
    15,621 packets / ~16 min capture | ~623 TCP ports probed via SYN scan
    SMB/RPC enumeration (LSA, SAMR, share enum) + default SNMP "public" string found
    Correctly distinguished recon/enum activity from actual exploitation

[+] Cisco 3640 — Nessus Vulnerability Assessment (GNS3)
    Network-device-focused scan with full severity breakdown

[+] Lynis — Linux Security Audit (Kali)
    269 tests | Hardening index: 60/100 | 1 warning, 49 suggestions
    Findings: inactive firewall/IDS, fail2ban gap, GRUB & PAM hardening opportunities

[+] OSINT & Recon Tooling
    Aliens Eye     — username OSINT scanner across 840+ platforms
    MailAccess     — email investigation/harvesting workflow (venv-based CLI tool)
    OSINT Recon    — subdomain/DNS enumeration (dnsenum, dnsrecon, dig, Subfinder) on a
                     real target, uncovered internal subdomains (sonarqube/vpn/UAT) behind
                     real origin IPs missed by standard footprinting

[+] AI-Assisted Offensive Tooling
    HexStrike AI & pentest-ai (ptai) — MCP-driven offensive tool orchestration (150+ modules,
    17 specialist agents), self-verifying scan/exploit findings, natural-language-driven
    recon and exploitation workflows — used strictly in authorized lab environments
```

<br>

## `~/cisco-networking`

Hands-on Cisco IOS labs, not just theory:

`IPv4/binary/subnetting` · `NAT (static + dynamic)` · `Standard & Extended ACLs` · `VLANs + inter-VLAN routing` · `RIP/OSPF/EIGRP/BGP concepts` · `HSRP/VRRP/GLBP failover labs` · `STP/BPDU & switching loops` · `DHCP` · `Wireless/WLC concepts`

<br>

## `~/currently`

```diff
+ CEH (Certified Ethical Hacker) — Completed, Corvit
+ Learning CCNP + Huawei configuration (GNS3 / eNSP)
+ Sharpening exploitation and post-exploitation workflows on new lab targets
+ Preparing for Penetration Tester / Red Team entry-level roles
```

<br>

<div align="center">

`Everything above was performed in isolated, authorized lab environments — Metasploitable2, self-hosted VMs, and virtual network topologies. No unauthorized targets.`

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:00ff41,100:0d1117&height=100&section=footer)

</div>
