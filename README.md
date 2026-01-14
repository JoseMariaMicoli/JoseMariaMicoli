# Hi, I'm José María Micoli 🛡️💻

**Senior Red Team Operator | Offensive Security Engineer | Tradecraft Developer**

I specialize in simulating advanced threat actor behaviors by building custom offensive tooling. My focus is on moving beyond automated scanning to test organizational resilience through engineered bypasses and stealthy persistence.

---

### 🛠️ Featured Tradecraft

* **[Hydra-C2](https://github.com/JoseMariaMicoli/Hydra-C2)**: A modular Command & Control framework designed for stealthy communication and EDR evasion. (Rust/Python/Kotlin)
* **[APEX-PRO](https://github.com/JoseMariaMicoli/APEX-PRO)**: A controlled ransomware simulator for auditing backup integrity and detection thresholds. (C#/Python/Powershell)
* **[VectorVue](https://github.com/JoseMariaMicoli/VectorVue)**: Red Team & Penetration Testing Reporting Framework (Python)
* **[Log4Shell-PoC](https://github.com/JoseMariaMicoli/Log4Shell-PoC)**: Log4Shell PoC is a high-fidelity exploitation environment designed to replicate the CVE-2021-44228 vulnerability. (Java/Python)
* **[EtherdogsC](https://savannah.nongnu.org/git/?group=etherdogsc)**: Low-level 802.3 network sniffer for deep-packet analysis. (C)

---

### 📊 Adversarial Tactic & Technique Mapping (MITRE ATT&CK®)

My tradecraft is engineered to simulate specific TTPs (Tactics, Techniques, and Procedures) as defined by the MITRE ATT&CK® framework.

| Tactic | Technique (ID) | Tooling / Implementation |
| --- | --- | --- |
| **Initial Access** | Exploit Public-Facing App (T1190) | **Log4Shell-PoC** (JNDI Injection) |
| **Execution** | PowerShell (T1059.001) | **APEX-PRO** / **Log4Shell-PoC** (Java RCE) |
| **Persistence** | Registry Run Keys / Startup Folder (T1547.001) | **APEX-PRO** (Persistence module) |
| **Discovery** | Network Service Scanning (T1046) / Network Share Discovery (T1135) | **EtherdogsC** / **APEX-PRO** |
| **Defense Evasion** | Obfuscated Files or Information (T1027) | **Hydra-C2** & **APEX-PRO** |
| **Command & Control** | Application Layer Protocol (T1071) / Encrypted Channel (T1573) | **Hydra-C2** / **Log4Shell-PoC** (LDAP/RMI) |
| **Exfiltration** | Exfiltration Over C2 Channel (T1041) / Over Bluetooth (T1011) | **APEX-PRO** (Data stage & exfil) |
| **Impact** | Data Encrypted for Impact (T1486) / Internal Defacement (T1491.001) | **APEX-PRO** (Ransomware simulation) |

---

### 🧰 Tech Stack

* **Languages:** Rust, C/C++, Python, Ruby, Powershell, Java/Kotlin.
* **Ops:** Red Teaming, Active Directory Exploitation, Web, Mobile & API Pentesting.
* **Infrastructure:** NGFW (Sophos/Fortinet/Cisco), Linux Hardening, Cisco Networking.

---

### 📫 Connect with Me

* **LinkedIn:** [ar.linkedin.com/in/jmmicoli](https://ar.linkedin.com/in/jmmicoli)
* **YouTube Channel:** [www.youtube.com/@josemariamicoli](https://www.youtube.com/@josemariamicoli)
* **Email:** [josemaria.micoli@gmail.com](mailto:josemaria.micoli@gmail.com)

---