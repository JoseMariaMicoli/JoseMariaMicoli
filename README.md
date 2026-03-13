# 🛡️ José María Micoli

![Red Team](https://img.shields.io/badge/Red%20Team-Adversary%20Operations-darkred)
![Adversary Emulation](https://img.shields.io/badge/Adversary-Emulation-black)
![Security Validation](https://img.shields.io/badge/Security-Validation-blue)

### Senior Offensive Security Engineer

Adversary Emulation • Red Team Operations • Security Validation Engineering
Identity Attack Modeling • API Security • Cloud IAM Abuse Simulation

---

# Offensive Security Engineering Portfolio

I design adversary tradecraft and offensive security platforms to measure **defensive effectiveness in modern enterprise environments.**

My work focuses on structured **adversary simulation and continuous security validation**, bridging:

• Red Team operations
• Detection engineering validation
• Identity attack-path modeling
• API security testing
• Cloud IAM abuse simulation
• SOC detection capability measurement

The objective is **not compromise demonstration.**

The objective is **defensive assurance through measurable adversary simulation.**

---

# Executive Overview

Modern organizations deploy increasingly complex security stacks:

• EDR
• SIEM
• IAM
• Cloud security controls
• API gateways
• Zero-trust architectures

However, most security programs still rely on **point-in-time penetration testing**.

This creates a fundamental question:

> Do these controls actually work against real adversary behavior?

This portfolio contains research platforms, adversary simulation infrastructure, and offensive engineering tooling designed to **continuously validate security controls under realistic attacker tradecraft.**

---

## Strategic Security Platforms

The following platforms represent the core systems within this offensive security engineering portfolio.
Each repository focuses on adversary simulation, security validation, or attack-surface intelligence across enterprise environments.

| Platform                                                                                  | Domain                       | Purpose                                            |
| ----------------------------------------------------------------------------------------- | ---------------------------- | -------------------------------------------------- |
| 🛡 **[VectorVue](https://github.com/nyxeralabs/VectorVue)**                                 | Security Validation Platform | Continuous control validation & compliance mapping |
| 🔴 **[SpectraStrike](https://github.com/nyxeralabs/SpectraStrike)**                         | Red Team Orchestration       | Structured adversary simulation campaigns          |
| 🌐 **[VaporTrace](https://github.com/josemariamicoli/VaporTrace)**                               | API Risk Intelligence        | Automated API attack-path discovery                |
| 🧪 **[VaporLab](https://github.com/nyxeralabs/VaporLab)**                                   | API & AI Exploitation        | Offensive research and testing environment         |
| 📡 **[Nyxera Eye](https://github.com/nyxeralabs/Nyxera-Eye)**                               | IoT / ICS Intelligence       | Global attack surface discovery                    |
| ⚙️ **[Ghost-Pipeline](https://github.com/josemariamicoli/Ghost-Pipeline)**                       | CI/CD Security               | OIDC token abuse & supply-chain simulation         |
| 💀 **[APEX-PRO](https://github.com/josemariamicoli/APEX-PRO)**                                   | Ransomware Emulation         | Incident response readiness measurement            |
| 🐙 **[Hydra-C2](https://github.com/josemariamicoli/Hydra-C2)**                                   | Red Team Infrastructure      | Multi-platform command and control                 |
| 🐍 **[Hydra-Worm](https://github.com/josemariamicoli/Hydra-Worm)**                               | Adversarial Propagation      | Lateral movement & segmentation testing            |
| 🧨 **[Log4Shell-PoC](https://github.com/josemariamicoli/Log4Shell-PoC)**                         | Vulnerability Research       | Detection validation and WAF analysis              |
| 🧱 **[Adversary Simulation Lab](https://github.com/josemariamicoli/Adversary-Simulation-Lab)**   | Red Team Lab                 | Structured adversary training infrastructure       |
| 📑 **[Pentest Reports Portfolio](https://github.com/josemariamicoli/Pentest-Reports-Portfolio)** | Security Reporting           | Executive-grade reporting models                   |

---

### Portfolio Domains

This repository ecosystem covers multiple offensive security domains:

* 🔴 Red Team Operations & Adversary Emulation
* 🛡 Continuous Security Validation
* 🔍 API & Application Security
* ☁️ Cloud & CI/CD Attack Surface
* 📡 IoT / ICS Security Intelligence
* 🧬 Vulnerability Research
* 📊 Security Reporting & Risk Intelligence

---

# Adversary Infrastructure Architecture

Example adversary infrastructure used in Red Team simulations.

```mermaid
flowchart TD

Operator[Red Team Operator]

Operator --> C2Framework
C2Framework --> Redirector
Redirector --> PayloadServer
PayloadServer --> TargetEnvironment

TargetEnvironment --> AD
TargetEnvironment --> Cloud
TargetEnvironment --> APIs

AD --> LateralMovement
Cloud --> IAMAbuse
APIs --> AuthorizationAbuse
```

This infrastructure supports simulations of:

• Identity privilege escalation
• API authorization attacks
• Cloud IAM abuse
• lateral movement campaigns
• command-and-control detection testing

---

# Adversary Simulation Workflow

Structured offensive methodology used across projects.

```mermaid
flowchart TD

Recon[Reconnaissance]

Recon --> Weaponization
Weaponization --> InitialAccess
InitialAccess --> PrivEsc
PrivEsc --> LateralMove
LateralMove --> Persistence
Persistence --> CommandControl
CommandControl --> Impact
Impact --> DetectionValidation
```

Each phase is mapped to **MITRE ATT&CK techniques and detection validation objectives.**

---

# MITRE ATT&CK Coverage

The adversary simulation platforms in this portfolio map offensive activity to **ATT&CK tactics and techniques** to measure defensive visibility.

| ATT&CK Phase         | Example Techniques Simulated                  |
| -------------------- | --------------------------------------------- |
| Reconnaissance       | T1595 – Active Scanning                       |
| Initial Access       | T1566 – Phishing                              |
| Execution            | T1059 – Command and Scripting Interpreter     |
| Persistence          | T1547 – Boot or Logon Autostart Execution     |
| Privilege Escalation | T1068 – Exploitation for Privilege Escalation |
| Defense Evasion      | T1070 – Indicator Removal on Host             |
| Credential Access    | T1003 – OS Credential Dumping                 |
| Discovery            | T1087 – Account Discovery                     |
| Lateral Movement     | T1021 – Remote Services                       |
| Command & Control    | T1071 – Application Layer Protocol            |
| Exfiltration         | T1041 – Exfiltration Over C2 Channel          |
| Impact               | T1486 – Data Encrypted for Impact             |

---

# Detection Validation Framework

Offensive simulations are used to measure **security control performance** across detection layers.

| Security Control    | Validation Objective           |
| ------------------- | ------------------------------ |
| EDR                 | Behavioral detection coverage  |
| SIEM                | Correlation rule effectiveness |
| NGFW                | Network anomaly detection      |
| Identity Monitoring | Privilege abuse detection      |
| API Gateways        | Authorization bypass detection |
| Cloud Security      | IAM abuse monitoring           |

---

# Identity-Centric Attack Modeling

Modern breaches frequently originate from **identity abuse rather than software vulnerabilities.**

Example attack path simulation:

```mermaid
flowchart TD

Phishing --> TokenTheft
TokenTheft --> CloudAccess
CloudAccess --> IAMPrivilegeEscalation
IAMPrivilegeEscalation --> ResourceControl
```

This model allows organizations to evaluate:

• OAuth / OIDC token abuse
• cross-account IAM privilege escalation
• federation trust boundary exploitation

---

# API Security Validation Model

API security simulations focus on **authorization logic abuse and identity trust boundary failures** rather than traditional injection vulnerabilities.

Key attack patterns tested:

• Broken Object Level Authorization (BOLA)
• Broken Function Level Authorization (BFLA)
• OAuth misconfiguration abuse
• JWT trust boundary weaknesses
• API gateway policy bypass

---

# Methodological Foundations

The offensive engineering and adversary simulation methodologies implemented here align with:

• MITRE ATT&CK®
• NIST SP 800-115
• Threat-Informed Defense
• Structured Rules of Engagement

All offensive activity is designed to produce **measurable defensive insights.**

---

# Professional Security Reporting

Security validation engagements generate structured outputs including:

• Detection gap analysis
• Attack-path modeling
• root-cause attack path analysis
• executive remediation strategy
• audit-ready validation evidence

The objective is not vulnerability enumeration.

The objective is **security maturity improvement.**

---

# Legal & Ethical Notice

All research and tooling in this repository are used **exclusively in authorized security engagements or controlled laboratory environments.**

This portfolio exists to **strengthen defensive security capabilities.**

---

# Contact

**José María Micoli**
Senior Offensive Security Engineer

Red Team • Adversary Emulation • Security Validation • Cloud & API Security

---

### Professional Links

**LinkedIn**
https://linkedin.com/in/jmmicoli

**Nyxera Labs**
https://nyxera.cloud

---

### Contact

**Professional Email**
[jmicoli@nyxera.cloud](mailto:jmicoli@nyxera.cloud)

**Alternative Contact**
[josemaria.micoli@gmail.com](mailto:josemaria.micoli@gmail.com)

---
