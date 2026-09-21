<div align="center">

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:00ff41&height=200&section=header&text=Haider%20Jamal&fontSize=45&fontColor=00ff41&fontAlignY=35&desc=Cybersecurity%20%7C%20CEH%20Certified&descAlignY=55&descColor=8b949e&animation=fadeIn)

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=20&duration=2500&pause=800&color=00FF41&center=true&vCenter=true&width=600&lines=whoami+%3D%3E+Certified+Ethical+Hacker;Offense+%2B+Defense+%7C+Red+%26+Blue;Breaking+things+in+labs+to+learn+how+to+stop+them;nmap+-sV+-sC+-p-+target+%7C+tee+scan.log" alt="Typing SVG" /></a>

![Profile Views](https://komarev.com/ghpvc/?username=haiderjamal&color=00ff41&style=flat-square&label=PROFILE+VIEWS)
![Status](https://img.shields.io/badge/status-hunting_vulnerabilities-00ff41?style=flat-square&labelColor=161b22)
![Focus](https://img.shields.io/badge/mode-lab_isolated-00ff41?style=flat-square&labelColor=161b22)

</div>

<br>

<div align="center">

```
┌──────────────────────────────────────────────────────────┐
│  root@haider:~# cat mission.txt                           │
│  Recon → Enum → Exploit → Detect → Respond → Repeat        │
│  Every attack I run, I can also explain how to catch.      │
└──────────────────────────────────────────────────────────┘
```

</div>

<br>

## `~/about`

```yaml
focus:         Cybersecurity — offensive (recon, exploitation) and defensive (detection, monitoring, response)
certification: CEH (Certified Ethical Hacker) — Corvit, NAVTTC — Completed
also_studying: CCNP, Huawei (GNS3 / eNSP)
philosophy:    Labs > theory. Evidence > claims. Every attack I run, I can also explain how to catch.
```

<br>

## `~/lab-infrastructure`

Everything below runs in an isolated, host-only virtualized lab — Kali as the attack box, Metasploitable2/Windows as intentionally vulnerable targets, Wazuh as the monitoring layer, never against anything I don't own or have authorization for.

| Layer | Stack |
|---|---|
| **Virtualization** | VMware Workstation, EVE-NG, GNS3, Cisco Packet Tracer |
| **Attack box** | Kali Linux |
| **Targets** | Metasploitable 2, Windows 7/10/11 VMs (XAMPP-simulated services), Cisco 3640 (GNS3) |
| **Monitoring/SIEM** | Wazuh (Rocky Linux) |
| **Networking gear (virtual)** | Cisco routers/switches (IOS), HSRP/VRRP/GLBP labs |

<br>

## `~/skills`

![Networking](https://img.shields.io/badge/Networking-Subnetting_|_VLANs_|_NAT_|_ACLs_|_OSPF/RIP/BGP-161b22?style=for-the-badge&logo=cisco&logoColor=00ff41&labelColor=161b22)
![Systems](https://img.shields.io/badge/Systems-Linux(Kali/Debian/RHEL)_|_Windows_Server_|_AD-161b22?style=for-the-badge&logo=linux&logoColor=00ff41&labelColor=161b22)
![Offensive](https://img.shields.io/badge/Offensive-Recon_|_Enumeration_|_Exploitation_|_Post--Exploitation-161b22?style=for-the-badge&logo=hackthebox&logoColor=00ff41&labelColor=161b22)
![Defensive](https://img.shields.io/badge/Defensive-SIEM_|_Log_Analysis_|_Alert_Triage_|_Incident_Response-161b22?style=for-the-badge&logo=wazuh&logoColor=00ff41&labelColor=161b22)
![WebSec](https://img.shields.io/badge/Web_Security-OWASP_Top_10_|_DAST_|_Manual_Validation-161b22?style=for-the-badge&logo=owasp&logoColor=00ff41&labelColor=161b22)
![Net](https://img.shields.io/badge/Network_Attacks-ARP_Poisoning_|_MITM_|_Packet_Analysis-161b22?style=for-the-badge&logo=wireshark&logoColor=00ff41&labelColor=161b22)

**Tools:**

`Nmap · Gobuster · Shodan · SearchSploit · Metasploit/Meterpreter · John the Ripper · Hydra · Nessus · OpenVAS/Greenbone · OWASP ZAP · Burp Suite · Wireshark · Ettercap · Lynis · Aircrack-ng · Wazuh (SIEM/EDR) · Sysmon`

<div align="center">

<img src="https://skillicons.dev/icons?i=linux,bash,python,docker,aws,azure,kali&theme=dark" />

<img src="https://img.shields.io/badge/Wireshark-161b22?style=for-the-badge&logo=wireshark&logoColor=00ff41" />
<img src="https://img.shields.io/badge/Metasploit-161b22?style=for-the-badge&logo=metasploit&logoColor=00ff41" />
<img src="https://img.shields.io/badge/Burp_Suite-161b22?style=for-the-badge&logo=burpsuite&logoColor=00ff41" />

</div>

<br>

## `~/evidence-portfolio`

> Documented, reproducible work on both sides — not just "I installed the tool."

```
[+] Metasploitable 2 — Nessus Vulnerability Assessment
    436 findings | 28 Critical · 99 High · 148 Medium · 20 Low · 141 Info
    Critical: Apache PHP-CGI RCE, Shellshock, bind-shell backdoor,
              phpMyAdmin SQLi exposure, UnrealIRCd backdoor, weak VNC creds

[+] Metasploitable 2 — Controlled Exploitation & Assessment Report
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
    forwarding to stay transparent → intercept with a packet analyzer. Same lab doubles as a
    detection exercise: this is exactly the traffic pattern a NIDS/ARP-watch rule should catch.

[+] Network Forensics — Malware Delivery + C2 Investigation (PCAP)
    Victim requested /update.exe x4 over HTTP:8000 → outbound TCP:4444 to C2 host
    ~566KB transferred in <1s post-handshake, ~67s sustained bidirectional session
    Pattern consistent with staged Meterpreter payload + interactive C2
    Analyzed purely from the defender's seat: identifying the delivery, staging, and
    C2 beacon phases from packet capture alone.

[+] Nessus / Wireshark — Windows Network Scan Analysis
    15,621 packets / ~16 min capture | ~623 TCP ports probed via SYN scan
    SMB/RPC enumeration (LSA, SAMR, share enum) + default SNMP "public" string found
    Correctly distinguished recon/enum activity from actual exploitation

[+] Wazuh SIEM Deployment — Rocky Linux
    Built a SIEM server from scratch (manager, indexer, dashboard) and onboarded endpoints
    as agents to practice log collection, alert triage, and rule tuning — the monitoring
    counterpart to the offensive labs above.

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

[+] AI-Assisted Security Tooling
    HexStrike AI & pentest-ai (ptai) — MCP-driven security tool orchestration (150+ modules,
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
+ Building out a Wazuh SIEM lab for detection/monitoring practice
+ Sharpening both exploitation workflows and the detections that catch them
+ Preparing for entry-level cybersecurity roles across SOC and offensive-adjacent work
```

<br>

<div align="center">

`Everything above was performed in isolated, authorized lab environments — Metasploitable2, self-hosted VMs, and virtual network topologies. No unauthorized targets.`

<br><br>

<img src="https://img.shields.io/badge/CEH-Certified-00ff41?style=for-the-badge&labelColor=161b22" />
<img src="https://img.shields.io/badge/Ethics-Authorized_Testing_Only-00ff41?style=for-the-badge&labelColor=161b22" />

<br><br>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:00ff41,100:0d1117&height=100&section=footer)

</div>
