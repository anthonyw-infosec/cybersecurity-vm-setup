# 🛡️ Blue Team Cybersecurity VM (Ubuntu ARM + VMware Fusion)

A lightweight, defense-focused cybersecurity virtual machine built on **Ubuntu ARM** inside **VMware Fusion**, designed for learning real Blue Team tools and workflows.

---

## 🔧 Overview

This project documents the setup of my personal **cybersecurity-ready virtual machine** preloaded with essential Blue Team tools. It serves as a personal playground to practice:

- Log analysis
- Intrusion detection
- Packet inspection
- Basic threat simulation

---

## ⚙️ Environment

| Item         | Details                  |
|--------------|--------------------------|
| OS           | Ubuntu 22.04 ARM64       |
| Hypervisor   | VMware Fusion (Mac)      |
| Focus        | Blue Team / Defensive Sec|
| GUI          | GNOME                    |

---

## 🛠️ Tools Installed

| Tool       | Use Case |
|------------|----------|
| **Fail2Ban**   | Blocks brute-force attacks automatically |
| **auditd**     | Monitors system activity & user actions |
| **ClamAV**     | Scans for malware (basic AV) |
| **rkhunter**   | Rootkit and backdoor detection |
| **Wireshark**  | Packet analysis for network traffic |
| **Scapy**      | Python tool for packet crafting/scripting |
| **Hydra**      | Brute-force password testing |
| **SQLMap**     | SQL injection testing (for defensive sim) |
| **Burp Suite** | Manual HTTP traffic inspection (.jar version) |

---

## 🎯 What This VM Is For

- 💻 Practicing Blue Team analysis tools
- 🔐 Simulating simple attacks to learn detection
- 📜 Reviewing Linux logs and network behavior
- 📚 Building a cybersecurity habit and foundation

---

## 🧠 Future Additions

- Bash scripts for automating log triage  
- Setup instructions for ELK Stack or Wazuh  
- Simple alerts and system health scripts  
- TryHackMe integration for guided labs

---

## 🚀 How to Use This VM

1. Download Ubuntu 22.04 ARM64 ISO
2. Install inside VMware Fusion (select ARM if using M1/M2 Mac)
3. Update packages: `sudo apt update && sudo apt upgrade -y`
4. Follow `tools-installed.md` to install each tool
5. Take snapshots after key installs
6. Practice log reading, detection, and packet capture

---

## 🙋 About Me

Aspiring Blue Team cybersecurity analyst currently studying at Chaffey College. Building hands-on skills in Linux security, network defense, and log analysis with the goal of joining a SOC or blue team in the next year.

This repo is part of my self-directed learning and certification prep.
