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

My research is engineered to bridge the gap between exploitation and actionable defense, cross-referenced with the **NIST SP 800-61 R3** lifecycle.

| Tactic | Technique | ID | Tradecraft Implementation |
| --- | --- | --- | --- |
| **Reconnaissance** | Active Scanning | **T1595.002** | **VaporTrace**: Shadow API discovery & recursive endpoint fuzzing. |
| **Initial Access** | Supply Chain Compromise | **T1195.002** | **Ghost-Pipeline**: Poisoning CI/CD runners via workflow injection. |
| **Initial Access** | Exploit Public-Facing App | **T1190** | **Log4Shell-PoC**: JNDI/LDAP injection vectors for RCE audit. |
| **Persistence** | Server Software Component | **T1505.003** | **Ghost-Pipeline**: Hijacking OIDC trust for credential-less access. |
| **Privilege Escalation** | Abuse Elevation Control | **T1548** | **VaporTrace**: BFLA exploitation for API token scope upgrade. |
| **Defense Evasion** | Obfuscated Files/Info | **T1027** | **Hydra-C2**: Direct Syscalls & polymorphic payload wrapping. |
| **Defense Evasion** | Indicator Removal | **T1070** | **Hydra-Worm**: Automated log cleaning & Timestomping. |
| **Discovery** | Network Service Scanning | **T1046** | **Hydra-Worm**: Low-noise ARP/SYN scanning for internal mapping. |
| **Lateral Movement** | Remote Services | **T1021.002** | **Hydra-Worm**: Automated propagation via Pass-the-Ticket (PtT). |
| **Command & Control** | Application Layer Protocol | **T1071.001** | **Hydra-C2**: NHPP-based jitter (DNS/Webhooks) to break pattern analysis. |
| **Impact** | Data Encrypted | **T1486** | **APEX-PRO**: Testing backup integrity against AES-256 simulation. |

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
