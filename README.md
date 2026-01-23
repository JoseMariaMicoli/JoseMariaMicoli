# Hi, I'm José María Micoli 🛡️💻

**Senior Red Team Operator | Offensive Security Engineer | Tradecraft Developer**

I specialize in simulating advanced threat actor behaviors by building custom offensive tooling. My focus is on moving beyond automated scanning to test organizational resilience through engineered bypasses and stealthy persistence.

---

### 🛠️ Featured Tradecraft

* **[Hydra-C2](https://github.com/JoseMariaMicoli/Hydra-C2)**: A modular Command & Control framework designed for stealthy communication and EDR evasion. (Rust/Python/Kotlin)
* **[VaporTrace](https://github.com/JoseMariaMicoli/VaporTrace)**: Surgical API Exploitation Suite covering the full OWASP API Top 10 (2023). (Go)
* **[Ghost-Pipeline](https://github.com/JoseMariaMicoli/Ghost-Pipeline)**: CI/CD post-exploitation framework targeting OIDC trust relationships. (Python/Shell/Go)
* **[APEX-PRO](https://github.com/JoseMariaMicoli/APEX-PRO)**: A controlled ransomware simulator for auditing backup integrity and detection thresholds. (C#/Python/Powershell)
* **[Log4Shell-PoC](https://github.com/JoseMariaMicoli/Log4Shell-PoC)**: High-fidelity exploitation environment for CVE-2021-44228. (Java/Python)
* **[VectorVue](https://github.com/JoseMariaMicoli/VectorVue)**: Red Team & Penetration Testing Reporting Framework. (Python)
* **[Hydra-Worm](https://github.com/JoseMariaMicoli/Hydra-Worm)**: is a research-oriented breach simulation framework featuring a Rust-based Agent for stealth, a Go-based Orchestrator for high-concurrency C2, and advanced capabilities for LotL propagation, polymorphic evasion, and cross-platform lateral movement. (Go/Rust)
* **[EtherdogsC](https://savannah.nongnu.org/git/?group=etherdogsc)**: Low-level 802.3 network sniffer for deep-packet analysis. (C)



---

### 📊 Adversarial Tactic & Technique Mapping (MITRE ATT&CK®)

My tradecraft is engineered to simulate specific TTPs (Tactics, Techniques, and Procedures) as defined by the MITRE ATT&CK® framework.

| Tactic | Technique (ID) | Tooling / Implementation |
| --- | --- | --- |
| **Reconnaissance** | Active Scanning (T1595.002) | **VaporTrace** (Shadow API mining/JS scraping) |
| **Initial Access** | Exploit Public-Facing App (T1190) | **Log4Shell-PoC** / **VaporTrace** (BOLA/BFLA/SSRF) |
| **Initial Access** | Supply Chain Compromise (T1195.002) | **Ghost-Pipeline** (Weaver agent injection) |
| **Execution** | PowerShell (T1059.001) / Java RCE | **APEX-PRO** / **Log4Shell-PoC** |
| **Persistence** | Compromise Client Software Binary (T1554) | **Ghost-Pipeline** (Post-exploitation CI/CD poisoning) |
| **Privilege Escalation** | Abuse Elevation Control (T1548) | **VaporTrace** (BFLA) / **Ghost-Pipeline** (OIDC to IAM) |
| **Credential Access** | Steal Application Access Token (T1528) | **Ghost-Pipeline** (OIDC JWT Hijacking) |
| **Discovery** | Network Service Scanning (T1046) | **EtherdogsC** / **VaporTrace** (Endpoint Mapping) |
| **Defense Evasion** | Obfuscated Files or Info (T1027) | **Hydra-C2** / **Ghost-Pipeline** (AES-256-GCM exfil) |
| **Command & Control** | Application Layer Protocol (T1071) | **Hydra-C2** / **Ghost-Pipeline** (ngrok/webhook) |
| **Exfiltration** | Exfiltration Over C2 Channel (T1041) | **APEX-PRO** / **Ghost-Pipeline** (Log-based leaking) |
| **Impact** | Data Encrypted for Impact (T1486) | **APEX-PRO** (Ransomware simulation) |

---

### 🧰 Tech Stack

* **Languages:** Rust, Go, C/C++, Python, Ruby, Powershell, Java/Kotlin.
* **Ops:** Red Teaming, CI/CD Security, Active Directory Exploitation, Web & API Pentesting (OWASP Top 10).
* **Infrastructure:** NGFW (Sophos/Fortinet/Cisco), Linux Hardening, Cisco Networking (NSE4 aligned).

---

### 📫 Connect with Me

* **LinkedIn Profile:** [ar.linkedin.com/in/jmmicoli](https://ar.linkedin.com/in/jmmicoli)
* **YouTube Channel:** [www.youtube.com/@josemariamicoli](https://www.youtube.com/@josemariamicoli)
* **Ghost-Hydra Intelligence Blog:** [josemariamicoli.github.io/](https://josemariamicoli.github.io/)
* **Personal e-mail:** [josemaria.micoli@gmail.com](mailto:josemaria.micoli@gmail.com)

---