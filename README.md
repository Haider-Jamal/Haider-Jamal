# Haider Jamal

<p align="center">
  <strong>Cybersecurity • Ethical Hacking • SOC • Network Security • Security Research</strong>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/haider--jamal/">LinkedIn</a> •
  <a href="https://github.com/mango00y">GitHub</a>
</p>

---

## `whoami`

I'm **Haider Jamal**, a cybersecurity learner building toward a practical **SOC / defensive-security** profile while maintaining strong hands-on exposure to offensive security, vulnerability assessment, network security, OSINT, malware analysis, and security research.

My work is lab-driven: I build isolated environments, test attack paths, inspect the evidence, document findings, and connect offensive activity to defensive detection and remediation.

> **Focus:** `SOC / SIEM` `Detection` `Network Security` `Vulnerability Management` `Pentesting` `Malware Analysis` `OSINT` `Security Research` `AI Security`

---

## ⚡ What I Actually Build

| Area | Hands-on work |
|---|---|
| 🛡️ SOC / SIEM | Wazuh Manager/Agent/Indexer/Dashboard, Sysmon telemetry, Suricata IDS/IPS |
| 🔎 Recon & OSINT | Nmap, Gobuster, Shodan, subdomain discovery, infrastructure research |
| 🧪 Vulnerability Management | Nessus, OpenVAS/Greenbone, CVE/CWE analysis, CVSS prioritization, remediation |
| 💥 Controlled Pentesting | Metasploitable2, Metasploit/Meterpreter, service enumeration and validation |
| 🌐 Web Security | OWASP ZAP, Burp Suite exposure, DVWA, Mutillidae, TWiki, phpMyAdmin |
| 🕵️ Network Forensics | Wireshark, PCAP analysis, IOC extraction, scan/beaconing/DNS-tunneling indicators |
| 🐧 Linux Security | Kali Linux, Rocky Linux, Lynis hardening audits |
| 🌐 Network Engineering | Cisco IOS, routing, switching, VLANs, ACLs, NAT/PAT, HSRP/VRRP/GLBP, GNS3/EVE-NG |
| 🤖 AI Security | PT-AI / Pentest-AI, HexStrike AI, AI-assisted security-tool orchestration |

---

# 🔥 Featured Security Projects

## 01 — Multi-Sensor Home SOC
**Wazuh + Windows/Sysmon + Suricata + Kali + Rocky Linux**

Built a multi-layer security monitoring lab instead of stopping at a basic SIEM installation.

- Deployed **Wazuh Manager, Agent, Indexer and Dashboard**
- Added Windows and Kali telemetry
- Configured **Windows Sysmon** and integrated its operational telemetry into Wazuh
- Deployed **Suricata IDS/IPS** on Rocky Linux
- Forwarded network-security telemetry toward Wazuh
- Worked with alerting, rules, investigation and detection workflows
- Designed the lab around an attack → telemetry → detection → investigation → remediation loop

**Security concepts:** SIEM, endpoint telemetry, IDS/IPS, alert triage, IOC analysis, detection engineering

---

## 02 — Network Forensics & C2 Investigation
**Wireshark + PCAP analysis**

Analyzed controlled-lab packet captures to reconstruct suspicious activity rather than simply looking at individual packets.

Documented evidence included:

- HTTP delivery of a Windows PE executable
- Outbound **TCP/4444** communication consistent with staged C2 behavior
- A separate PCAP containing **SYN-without-ACK scanning**
- Periodic **TCP/5555** communication consistent with possible beaconing
- ~40 high-entropy DNS queries consistent with possible DNS tunneling/data transfer
- HTTP artifacts and suspicious download/request patterns
- IOC and detection recommendations based on traffic behavior

The work connects packet-level evidence to the SOC question:

> **What happened, what evidence proves it, and what should a defender detect?**

---

## 03 — Vulnerability Assessment & Controlled Exploitation
**Metasploitable 2 + Nessus + Nmap + Metasploit**

Performed vulnerability assessment and controlled validation against an intentionally vulnerable lab target.

A documented Nessus assessment contained:

- **436 total findings**
- **28 Critical**
- **99 High**
- **148 Medium**
- **20 Low**
- **141 Informational**

Selected vulnerabilities were manually validated in the isolated lab, including:

- Bind-shell backdoor
- UnrealIRCd backdoor
- VNC weak-password exposure
- Apache PHP-CGI argument-injection/RCE path

The reports paired exploitation evidence with remediation guidance rather than treating scanner output alone as proof.

---

## 04 — Web Application Security Assessment
**OWASP ZAP + DVWA + Mutillidae + TWiki + phpMyAdmin**

Performed a lab web-application assessment using OWASP ZAP.

Documented scope included:

- DVWA
- Mutillidae II
- TWiki
- phpMyAdmin
- WebDAV
- Root web content
- `sitemap.xml`
- `robots.txt`

The assessment documented **23 findings**, including examples such as:

- MD5-crypt hash disclosure
- Missing Content Security Policy
- Application error disclosure
- Directory browsing
- Missing anti-clickjacking protection
- Security-header/cookie weaknesses
- Version/banner disclosure

---

## 05 — Cisco Network Security & Vulnerability Assessment
**Cisco IOS + GNS3 + EVE-NG + Nessus**

Built and assessed Cisco lab environments covering:

- Routing and switching
- VLAN segmentation
- Inter-VLAN routing
- ACLs
- NAT/PAT
- DHCP
- RIP / OSPF / EIGRP / BGP concepts
- HSRP / VRRP / GLBP
- STP and switching-loop behavior
- Management-plane security

A Cisco 3640 Nessus assessment documented **88 findings**:

`4 Critical • 45 High • 14 Medium • 2 Low • 23 Informational`

Notable security issues included default SNMP community configuration, unencrypted Telnet, legacy services and unsupported software.

---

## 06 — OSINT Reconnaissance — Real-World Domain Analysis

Performed a structured reconnaissance / OSINT exercise around a real-world domain.

Workflow included:

- Domain and subdomain discovery
- DNS / hosting research
- Technology fingerprinting
- Infrastructure and attack-surface mapping
- Shodan-based exposure research
- Subdomain enumeration
- Recon tooling including **Subfinder**
- `crt.sh` certificate-based discovery
- Organizing findings into a structured investigation

**Tools / concepts:** OSINT, Subfinder, crt.sh, Shodan, Netcraft, DNS enumeration, attack-surface discovery

> Real-world reconnaissance should always respect authorization, scope and applicable law.

---

## 07 — Malware Analysis Lab
**njRAT / RAT Behavior & Detection Study**

Built an isolated malware-analysis environment using Windows virtual machines.

The lab focused on understanding RAT behavior and the defensive evidence it can generate, including:

- Isolated VM analysis
- Malware behavior observation
- Remote-access / C2 concepts
- Process and network indicators
- Payload behavior
- Detection opportunities for endpoint and network telemetry

The work is framed as **controlled malware-analysis / adversary-emulation research**, not production deployment.

---

## 08 — ICMP Flood Attack & Defense Lab

Built a controlled lab to study denial-of-service behavior and defensive response.

The project focused on:

- ICMP traffic behavior
- Flooding concepts
- Network impact
- Monitoring and detection
- Defensive controls
- Comparing attack traffic with normal traffic

All traffic-generation work belongs in isolated, authorized environments.

---

## 09 — AI Pentesting Agent — Setup, Testing & Bug Reporting

Worked with AI-assisted penetration-testing tooling and agentic security workflows.

Documented work includes:

- AI-driven pentesting agent setup
- Tool/orchestration testing
- Specialist-agent architecture concepts
- Security-tool integration
- Reproducible testing
- Bug reporting

### Security research contribution

I identified and reported **two reproducible bugs** in the PTAI / AI pentesting-agent project:

- **Issue #29**
- **Issue #35**

This is an important part of my portfolio because it demonstrates not only tool usage, but also **testing, reproduction, documentation and responsible reporting**.

---

## 10 — Wazuh SIEM Deployment — Multi-Agent Detection Lab

Built a dedicated Wazuh deployment on **Rocky Linux** and worked with a multi-agent architecture.

Focus areas:

- Wazuh Manager
- Agents
- Indexer
- Dashboard
- Windows telemetry
- Kali telemetry
- Rocky Linux sensor environment
- Alert generation
- Rule configuration
- Security-event collection
- Network telemetry integration

This project is part of the larger multi-sensor SOC architecture.

---

## 11 — Linux Security Audit
**Lynis**

Performed a Linux security audit using Lynis.

Documented assessment:

- **269 tests**
- **1 warning**
- **49 suggestions**
- **60/100 hardening index**

Recommendations covered areas such as:

- Fail2ban
- GRUB protection
- Password policy
- PAM controls
- Package/update management
- Umask settings
- Host-hardening controls

---

## 12 — OSINT Tooling
**Aliens Eye + MailAccess**

Worked with OSINT tooling in isolated environments.

### Aliens Eye

- Git-based setup
- Python virtual environment
- Username-based OSINT workflows
- Platform correlation
- Domain checks
- Reporting workflow

### MailAccess

- Python virtual environment
- Email-harvesting workflows
- Investigation and diagnostic commands
- Shell integration
- Troubleshooting and command-path handling

---

# 🧪 Security Research & Contributions

### God's Eye View

**God's Eye View** — deployed as a project and included in my security/project portfolio.

### Open-Source Security Research

I have also worked on security testing of open-source / AI security tooling, including reproducible bug discovery and reporting.

**PTAI findings:** `#29` and `#35`

---

# 🛠️ Technical Stack

### Security / SOC
`Wazuh` `Suricata` `Sysmon` `MITRE ATT&CK` `IOC Analysis` `Alert Triage`

### Offensive Security
`Nmap` `Metasploit` `Meterpreter` `Gobuster` `Hydra` `John the Ripper` `SearchSploit`

### Vulnerability Management
`Nessus` `OpenVAS/Greenbone` `CVE` `CWE` `CVSS` `Remediation`

### Web Security
`OWASP ZAP` `Burp Suite` `DVWA` `Mutillidae` `TWiki` `phpMyAdmin`

### Network Security
`Cisco IOS` `VLANs` `ACLs` `NAT/PAT` `DHCP` `RIP` `OSPF` `EIGRP` `BGP` `STP` `HSRP` `VRRP` `GLBP`

### Forensics
`Wireshark` `PCAP Analysis` `IOC Extraction` `C2 Analysis` `DNS Analysis`

### Linux / Virtualization
`Kali Linux` `Rocky Linux` `Lynis` `VMware Workstation` `GNS3` `EVE-NG`

### OSINT
`Shodan` `Subfinder` `crt.sh` `Aliens Eye` `MailAccess` `Netcraft`

### AI Security
`PT-AI / Pentest-AI` `HexStrike AI` `AI-assisted security orchestration`

---

# 🎓 CEH

**Certified Ethical Hacker (CEH)**

My CEH training covered a practical progression through:

`Networking → Reconnaissance → Enumeration → Vulnerability Analysis → Exploitation → Malware Analysis → Sniffing → Wireless Security → Social Engineering → Web Security → Defensive/SOC concepts`

The documented training was heavily practical, with lab environments, virtual machines, networking exercises and security tooling.

---

# 📊 Evidence-Based Portfolio

| Deliverable | Evidence |
|---|---:|
| Metasploitable 2 Nessus assessment | 436 findings |
| Cisco 3640 Nessus assessment | 88 findings |
| OWASP ZAP web assessment | 23 findings |
| Lynis Linux audit | 269 tests |
| PCAP / network-forensics investigation | 409-packet investigation + larger Nessus capture |
| SOC architecture | Wazuh + Sysmon + Suricata |
| Controlled exploitation | Metasploitable 2 |
| Security research | PTAI bugs #29 and #35 |
| Malware research | njRAT / RAT behavior study |
| Recon / OSINT | Domain, subdomain, infrastructure and exposure analysis |

---

# 🧭 My Security Workflow

```text
        RECON
          │
          ▼
     ENUMERATION
          │
          ▼
   VULNERABILITY
      ANALYSIS
          │
          ▼
   CONTROLLED TEST
          │
          ▼
       EVIDENCE
          │
          ├──────────────┐
          ▼              ▼
     REMEDIATION      DETECTION
          │              │
          └──────┬───────┘
                 ▼
             INVESTIGATE
                 │
                 ▼
          DOCUMENT / REPORT
```

I try to go beyond:

> **"I ran the tool."**

and document:

> **"I found it → validated it → captured evidence → understood the impact → considered detection → documented remediation."**

---

# 📚 Current Learning Direction

My current direction is increasingly centered around:

- SOC operations
- Detection engineering
- Wazuh
- Sysmon
- Suricata
- Network forensics
- Incident investigation
- Vulnerability management
- Windows security
- Active Directory security
- MITRE ATT&CK mapping
- AI-assisted security tooling

---

# 🤝 Connect

<p align="center">
  <a href="https://www.linkedin.com/in/haider--jamal/">
    <img src="https://img.shields.io/badge/LinkedIn-Haider%20Jamal-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="https://github.com/mango00y">
    <img src="https://img.shields.io/badge/GitHub-mango00y-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
</p>

---

<p align="center">
  <strong>Build. Break. Detect. Investigate. Improve.</strong>
</p>

<p align="center">
  <sub>All offensive-security demonstrations are intended for owned, isolated or explicitly authorized environments.</sub>
</p>

