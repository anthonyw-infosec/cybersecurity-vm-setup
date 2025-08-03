# 🛠️ Tools Installed — Ubuntu Cybersecurity VM

Documentation of all tools installed on my Blue Team-focused Ubuntu ARM virtual machine. Each includes purpose, command used, and any special notes.

---

## ✅ Base System Info

| Detail         | Info               |
|----------------|--------------------|
| OS             | Ubuntu 22.04 ARM64 |
| Platform       | VMware Fusion      |
| Shell          | Bash               |

---

## 1. 🔐 Fail2Ban

- **Command**:  
  `sudo apt install fail2ban -y`

- **Purpose**: Blocks IP addresses after repeated failed SSH or login attempts.

- **Status Check**:  
  `sudo fail2ban-client status`

---

## 2. 📜 auditd

- **Command**:  
  `sudo apt install auditd -y`

- **Purpose**: Tracks system changes, command execution, file access, and more.

- **Enabled via**:  
  `sudo systemctl enable auditd`

---

## 3. 🧼 ClamAV

- **Command**:  
  `sudo apt install clamav -y`

- **Purpose**: Antivirus scanner for Linux.

---

## 4. 👁️‍🗨️ Rkhunter

- **Command**:  
  `sudo apt install rkhunter -y`

- **Purpose**: Detects rootkits and potential backdoors.

- **Scan command**:  
  `sudo rkhunter --check`

---

## 5. 🌐 Wireshark

- **Command**:  
  `sudo apt install wireshark -y`

- **Purpose**: Captures and analyzes network packets.

- **During install**: Enabled non-root packet capture.

---

## 6. 🧬 Scapy

- **Command**:  
  `sudo apt install python3-scapy -y`

- **Purpose**: Craft and analyze network packets using Python.

---

## 7. 💣 Hydra

- **Command**:  
  `sudo apt install hydra -y`

- **Purpose**: Brute-force login testing for multiple services.

---

## 8. 🐍 SQLMap

- **Command**:  
  `sudo apt install sqlmap -y`

- **Purpose**: Automates detection and exploitation of SQL injection flaws.

---

## 9. 🧪 Burp Suite (Manual Install)

- **Download From**: [https://portswigger.net/burp](https://portswigger.net/burp)

- **Command**:  
  `java -jar burpsuite_community_v2025.x.x.jar`

- **Note**: ARM-compatible version installed via `.jar` due to platform limitations.

---

## 📁 Directory Structure Used

~/cyber-labs/
├── tools/ ← Manual installs or downloads
├── logs/ ← Saved log outputs for analysis
├── scripts/ ← Custom bash/Python tools
└── notes/ ← Markdown files & study notes

---

## 📌 Notes

- Most tools were installed using `apt`, except Burp Suite (.jar)
- Snapshots were created at critical setup points (highly recommended)
- The VM is ARM64-based, which sometimes limits x86-compatible tools
- Future additions will include custom scripts, monitoring rules, and log filters

---

**Last updated**: August 2025  
