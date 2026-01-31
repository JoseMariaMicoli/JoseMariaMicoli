# 🛡️ [xoce@darkarch]:~# José María Micoli

**Senior Red Team Operator | Offensive Security R&D Engineer | Tradecraft Developer**

> **"Security is a process of constant R&D. The adversary is always building; we must build faster."**

I specialize in **Research-Driven Adversary Emulation**, simulating sophisticated threat actor behaviors by developing proprietary tradecraft to bypass modern EDR/AV and Next-Gen Firewall solutions. My work focuses on the engineering of stealthy persistence, custom C2 architectures, and the exploitation of modern attack surfaces (OIDC/CI-CD/APIs).

---

### 🛠️ FEATURED TRADECRAFT (R&D)

| Project | Focus Area | Core Stack |
| --- | --- | --- |
| **[Hydra-Worm](https://github.com/JoseMariaMicoli/Hydra-Worm)** | Next-Gen Breach & Lateral Movement Simulation | `Go` `Rust` |
| **[Hydra-C2](https://github.com/JoseMariaMicoli/Hydra-C2)** | Modular C2 Framework with Evasion-first listeners | `Rust` `Python` `Kotlin` |
| **[VaporTrace](https://github.com/JoseMariaMicoli/VaporTrace)** | Surgical API Exploitation (OWASP API Top 10: 2023) | `Go` |
| **[Ghost-Pipeline](https://github.com/JoseMariaMicoli/Ghost-Pipeline)** | CI/CD Post-Exploitation & OIDC Trust Hijacking | `Python` `Go` |
| **[APEX-PRO](https://github.com/JoseMariaMicoli/APEX-PRO)** | High-fidelity Ransomware Emulation (IR Readiness) | `C#` `PowerShell` |
| **[Log4Shell-PoC](https://github.com/JoseMariaMicoli/Log4Shell-PoC)** | High-Fidelity JNDI Exploitation & Evasion Audit | `Java` `Python` |
| **[VectorVue](https://github.com/JoseMariaMicoli/VectorVue)** | NIST-aligned Red Team Reporting Engine | `Python` |

---

### 📊 ADVANCED ADVERSARIAL TTP MAPPING (**MITRE ATT&CK®**)

| Tactic | Technique | ID | Tool / Project | Implementation Detail | OWASP / Risk |
| --- | --- | --- | --- | --- | --- |
| **Recon** | Active Scanning | `T1595.002` | **VaporTrace** | OpenAPI/Swagger harvesting & recursive endpoint fuzzing. | API9: Inventory |
|  | Search Victim Sites | `T1594` | **Hydra-Worm** | Probing Cloud IMDSv2 (169.254) for instance identity/roles. | API7: SSRF |
|  | Gather Host Info | `T1592` | **VaporTrace** | JS Static Analysis/Mining for hidden client-side routes. | API9: Inventory |
|  | Gather Identity Info | `T1589` | **VaporTrace** | Param Mining & API version brute-forcing (Legacy ID). | - |
| **Initial Access** | Supply Chain | `T1195.002` | **Ghost-Pipeline** | Poisoning CI/CD runners via `weaver` workflow injection. | - |
|  | Exploit Public App | `T1190` | **Log4Shell-PoC** | JNDI/LDAP injection vectors for RCE audit emulation. | - |
| **Execution** | Command Interpreter | `T1059.001` | **Hydra-C2** | JSON-based platform-aware command dispatch (Rust/Kotlin). | API5: BFLA |
|  | Shared Modules | `T1129` | **Hydra-Android** | "Head Mode" full hardware & FS access integration. | - |
| **Persistence** | System Process | `T1543.003` | **Hydra-C2** | Systemd (Linux) & Registry (Win) hijacking for agents. | - |
|  | Server Software | `T1505.003` | **Ghost-Pipeline** | Hijacking GitHub OIDC trust for credential-less access. | - |
|  | Startup Items | `T1137` | **Hydra-Android** | "Ghost Service" background execution with WakeLock. | - |
| **Priv Escalation** | Abuse Elevation | `T1548` | **VaporTrace** | BOLA/BFLA exploitation for API token scope upgrade. | **API1 / API5** |
| **Def Evasion** | Obfuscated Info | `T1027` | **Apex-Pro** | Polymorphic payload wrapping & AES-256 log encryption. | - |
|  | Indicator Removal | `T1070` | **Hydra-Worm** | Automated log zeroing & `bash_history` sanitization. | - |
|  | Protocol Impersonation | `T1001.003` | **Hydra-Worm** | Mimicking DNS/NTP/ICMP traffic via manual construction. | - |
|  | Proxy Usage | `T1090.003` | **VaporTrace** | Multi-hop IP rotation pools to bypass rate-limiting. | - |
|  | Modify Tools | `T1562.001` | **VaporTrace** | Header/UA Randomization to evade Signature-based WAFs. | - |
|  | Sandbox Evasion | `T1497` | **Hydra-Worm** | Detection of `/.dockerenv` to identify container constraints. | - |
| **Credential Access** | Steal Access Token | `T1528` | **Ghost-Pipeline** | Intercepting GitHub OIDC JWTs from CI/CD runners. | API2: Auth |
|  | Input Capture | `T1056.001` | **Hydra-Android** | Accessibility Keylogger (Bypassing TCL v3.0). | - |
|  | Forge Web Credentials | `T1606` | **VaporTrace** | JWT Algorithm Downgrade & Forge attacks. | API2: Auth |
| **Discovery** | Network Service Scan | `T1046` | **VaporTrace** | SSRF targeting internal cloud metadata services. | **API7: SSRF** |
|  | System Info | `T1082` | **Hydra-C2** | Telemetry: Hostname, OS, RAM, Battery, & Network SSID. | - |
|  | Remote System | `T1018` | **Hydra-Worm** | mDNS (UDP/5353) & ARP analysis for local mesh mapping. | - |
|  | File/Dir Discovery | `T1083` | **Hydra-Worm** | Targeting `known_hosts` and `ssh_history` for pivots. | - |
| **Lateral Movement** | Remote Services | `T1021.004` | **Hydra-Worm** | Propagation via SSH utilizing harvested credentials. | - |
| **Collection** | Audio Capture | `T1123` | **Hydra-C2** | Background mic recording & exfil (MPEG4-AAC/WAV). | - |
|  | Data from Local Sys | `T1637` | **Hydra-Android** | Automated SMS/Contact extraction modules. | - |
|  | Archive Collected | `T1560` | **VaporTrace** | Framework-tagged persistence in `vaportrace.db`. | - |
| **C2** | App Layer Protocol | `T1071.001` | **Hydra-C2** | NHPP-based jitter (DNS/Webhooks) to break pattern analysis. | - |
|  | Proxy | `T1090` | **Hydra-C2** | Reverse Proxy / SOCKS5 Tunneling for internal pivoting. | API7: SSRF |
|  | Protocol Tunneling | `T1572` | **Ghost-Pipeline** | Tunneling shell traffic through local-to-cloud relays. | - |
|  | Dynamic Resolution | `T1568` | **Hydra-Worm** | Stochastic jitter heartbeats to bypass frequency analysis. | - |
| **Exfiltration** | Over C2 Channel | `T1041` | **Apex-Pro** | Manual download & recursive chunked log retrieval. | - |
|  | Automated Exfil | `T1020` | **Hydra-C2** | Real-time GPS & Audio intelligence streaming. | - |
|  | Exfil Over Alt Proto | `T1011.001` | **Ghost-Pipeline** | Recursive chunked log retrieval via HTTP webhooks. | - |
| **Impact** | Data Encrypted | `T1486` | **Apex-Pro** | Testing backup integrity against AES-256 simulation. | - |
|  | Data Manipulation | `T1496` | **VaporTrace** | Mass Assignment (BOPLA) payload injection. | API6: Unsafe |
|  | Endpoint DoS | `T1499` | **VaporTrace** | Resource Exhaustion (Symmetric DoS) via API abuse. | API4: Resource |
|  | Internal Defacement | `T1491.001` | **Apex-Pro** | Automated UI/Internal state manipulation testing. | - |

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
