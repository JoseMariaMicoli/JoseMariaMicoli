# 🛡️ [xoce@darkarch]:~# José María Micoli

**Senior Red Team Operator | Offensive Security R&D Engineer | Tradecraft Developer**

> **"Security is a process of constant R&D. The adversary is always building; we must build faster."**

I specialize in **Research-Driven Adversary Emulation**, simulating sophisticated threat actor behaviors by developing proprietary tradecraft to bypass modern EDR/AV and Next-Gen Firewall solutions. My work focuses on the engineering of stealthy persistence, custom C2 architectures, and the exploitation of modern attack surfaces (OIDC/CI-CD/APIs).

---

### 🛠️ Strategic R&D & Offensive Engineering

*Advanced security ecosystems engineered for cross-platform adversarial simulation, heuristic risk intelligence, and NIST-compliant auditing.*

| Project | Focus Area | Core Stack |
| --- | --- | --- |
| **[Hydra-Worm](https://github.com/JoseMariaMicoli/Hydra-Worm)** | **Adversarial Propagation:** Next-gen breach simulation framework. Features a **Rust-based Agent** for memory-safe stealth and a **Go-based Orchestrator** for LotL propagation and polymorphic evasion. | `Rust` `Go` |
| **[Hydra-C2](https://github.com/JoseMariaMicoli/Hydra-C2)** | **Command & Control:** Modular Evasion-first framework with dedicated persistent agents for **Windows, Linux, and Android** mobile environments. | `Rust` `Python` `Kotlin` |
| **[VaporTrace](https://github.com/JoseMariaMicoli/VaporTrace)** | **API Risk Intelligence:** Advanced Heuristic Analysis suite engineered in Go. Delivers surgical reconnaissance and transforms raw telemetry into structured compliance evidence. | `Go` |
| **[Ghost-Pipeline](https://github.com/JoseMariaMicoli/Ghost-Pipeline)** | **Supply Chain Security:** CI/CD Post-Exploitation & OIDC Trust Hijacking for modern DevOps infrastructure audits. | `Python` `Go` |
| **[APEX-PRO](https://github.com/JoseMariaMicoli/APEX-PRO)** | **Crisis Readiness:** High-fidelity Ransomware Emulation designed for enterprise Incident Response (IR) validation. | `C#` `PowerShell` |
| **[Log4Shell-PoC](https://github.com/JoseMariaMicoli/Log4Shell-PoC)** | **Vulnerability R&D:** High-Fidelity JNDI Exploitation & Evasion Audit focusing on deep-packet inspection (DPI) bypass. | `Java` `Python` |
| **[VectorVue](https://github.com/JoseMariaMicoli/VectorVue)** | **Operational Reporting:** NIST-aligned Red Team engine that transforms raw telemetry into executive risk summaries. | `Python` |
| **[Pentest-Audit-Archive](https://github.com/JoseMariaMicoli/Pentest-Audit-Portfolio)** | **Methodology Lab:** Curated repository of **HTB Penetration Testing Reports** and **NIST-compliant security audits**. | `Markdown` `Mermaid` |

---

### 📊 ADVANCED ADVERSARIAL TTP MAPPING (**MITRE ATT&CK®**)

My research is engineered to bridge the gap between exploitation and actionable defense, cross-referenced with the **MITRE ATT&CK®** framework and **NIST SP 800-61 R3** lifecycle.

| Tactic | Technique | ID | Tool / Project | Implementation Detail |
| --- | --- | --- | --- | --- |
| **Recon** | Active Scanning | `T1595.002` | **VaporTrace** | OpenAPI/Swagger harvesting & recursive endpoint fuzzing. |
|  | Search Victim Sites | `T1594` | **Hydra-Worm** | Probing Cloud IMDSv2 (169.254) for instance identity/roles. |
|  | Gather Host Info | `T1592` | **VaporTrace** | JS Static Analysis/Mining for hidden client-side routes. |
|  | Gather Identity Info | `T1589` | **VaporTrace** | Param Mining & API version brute-forcing (Legacy ID). |
| **Initial Access** | Supply Chain | `T1195.002` | **Ghost-Pipeline** | Poisoning CI/CD runners via `weaver` workflow injection. |
|  | Exploit Public App | `T1190` | **Log4Shell-PoC** | JNDI/LDAP injection vectors for RCE audit emulation. |
| **Execution** | Command Interpreter | `T1059.001` | **Hydra-C2** | JSON-based platform-aware command dispatch (Rust/Kotlin). |
|  | Shared Modules | `T1129` | **Hydra-Android** | "Head Mode" full hardware & FS access integration. |
| **Persistence** | System Process | `T1543.003` | **Hydra-C2** | Systemd (Linux) & Registry (Win) hijacking for agents. |
|  | Server Software | `T1505.003` | **Ghost-Pipeline** | Hijacking GitHub OIDC trust for credential-less access. |
|  | Startup Items | `T1137` | **Hydra-Android** | "Ghost Service" background execution with WakeLock. |
| **Priv Escalation** | Abuse Elevation | `T1548` | **VaporTrace** | BOLA/BFLA exploitation for API token scope upgrade. |
| **Def Evasion** | Obfuscated Info | `T1027` | **Apex-Pro** | Polymorphic payload wrapping & AES-256 log encryption. |
|  | Indicator Removal | `T1070` | **Hydra-Worm** | Automated log zeroing & `bash_history` sanitization. |
|  | Protocol Impersonation | `T1001.003` | **Hydra-Worm** | Mimicking DNS/NTP/ICMP traffic via manual construction. |
|  | Proxy Usage | `T1090.003` | **VaporTrace** | Multi-hop IP rotation pools to bypass rate-limiting. |
|  | Modify Tools | `T1562.001` | **VaporTrace** | Header/UA Randomization to evade Signature-based WAFs. |
|  | Sandbox Evasion | `T1497` | **Hydra-Worm** | Detection of `/.dockerenv` to identify container constraints. |
| **Credential Access** | Steal Access Token | `T1528` | **Ghost-Pipeline** | Intercepting GitHub OIDC JWTs from CI/CD runners. |
|  | Input Capture | `T1056.001` | **Hydra-Android** | Accessibility Keylogger (Bypassing TCL v3.0). |
|  | Forge Web Credentials | `T1606` | **VaporTrace** | JWT Algorithm Downgrade & Forge attacks. |
| **Discovery** | Network Service Scan | `T1046` | **VaporTrace** | SSRF targeting internal cloud metadata services. |
|  | System Info | `T1082` | **Hydra-C2** | Telemetry: Hostname, OS, RAM, Battery, & Network SSID. |
|  | Remote System | `T1018` | **Hydra-Worm** | mDNS (UDP/5353) & ARP analysis for local mesh mapping. |
|  | File/Dir Discovery | `T1083` | **Hydra-Worm** | Targeting `known_hosts` and `ssh_history` for pivots. |
| **Lateral Movement** | Remote Services | `T1021.004` | **Hydra-Worm** | Propagation via SSH utilizing harvested credentials. |
| **Collection** | Audio Capture | `T1123` | **Hydra-C2** | Background mic recording & exfil (MPEG4-AAC/WAV). |
|  | Data from Local Sys | `T1637` | **Hydra-Android** | Automated SMS/Contact extraction modules. |
|  | Archive Collected | `T1560` | **VaporTrace** | Framework-tagged persistence in `vaportrace.db`. |
| **C2** | App Layer Protocol | `T1071.001` | **Hydra-C2** | NHPP-based jitter (DNS/Webhooks) to break pattern analysis. |
|  | Proxy | `T1090` | **Hydra-C2** | Reverse Proxy / SOCKS5 Tunneling for internal pivoting. |
|  | Protocol Tunneling | `T1572` | **Ghost-Pipeline** | Tunneling shell traffic through local-to-cloud relays. |
|  | Dynamic Resolution | `T1568` | **Hydra-Worm** | Stochastic jitter heartbeats to bypass frequency analysis. |
| **Exfiltration** | Over C2 Channel | `T1041` | **Apex-Pro** | Manual download & recursive chunked log retrieval. |
|  | Automated Exfil | `T1020` | **Hydra-C2** | Real-time GPS & Audio intelligence streaming. |
|  | Exfil Over Alt Proto | `T1011.001` | **Ghost-Pipeline** | Recursive chunked log retrieval via HTTP webhooks. |
| **Impact** | Data Encrypted | `T1486` | **Apex-Pro** | Testing backup integrity against AES-256 simulation. |
|  | Data Manipulation | `T1496` | **VaporTrace** | Mass Assignment (BOPLA) payload injection. |
|  | Endpoint DoS | `T1499` | **VaporTrace** | Resource Exhaustion (Symmetric DoS) via API abuse. |
|  | Internal Defacement | `T1491.001` | **Apex-Pro** | Automated UI/Internal state manipulation testing. |

---

### ⚙️ TECHNICAL ECOSYSTEM

* **Offensive Engineering:** Custom C2 Development, EDR/AV Evasion (Direct Syscalls), Binary Analysis, Reverse Engineering (Ghidra/JADX), Android Native Analysis.
* **Target Landscapes:** Active Directory (On-prem/Azure), Cloud Native (AWS/GCP/Azure), Microservices (REST/GraphQL), Mobile Security.
* **Infrastructure Mastery:** Sophos/Fortinet/Cisco NGFW, Linux Kernel Hardening, OIDC/OAuth2 Trust Models, CI/CD Security.

---

### 🌐 INTEL & CONNECTIVITY

* **Research Blog:** [josemariamicoli.github.io](https://josemariamicoli.github.io/) (Ghost-Hydra Intelligence)
* **Professional:** [LinkedIn](https://ar.linkedin.com/in/jmmicoli)
* **Technical/Offensive:** [HackTheBox](https://app.hackthebox.com/users/954485)
* **Standard Communication:** [josemaria.micoli@gmail.com](mailto:josemaria.micoli@gmail.com)
* **Encrypted Communication:** [ghost-hydra@proton.me](mailto:ghost-hydra@proton.me)
* **Video PoCs:** [YouTube @josemariamicoli](https://www.youtube.com/@josemariamicoli)

---
