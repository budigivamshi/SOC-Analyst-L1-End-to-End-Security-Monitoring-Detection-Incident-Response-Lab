# 🛡️ SOC Analyst L1 — End-to-End Security Monitoring, Detection & Incident Response Lab

![SOC](https://img.shields.io/badge/Role-SOC%20Analyst%20L1-blue)
![Splunk](https://img.shields.io/badge/SIEM-Splunk-orange)
![Sysmon](https://img.shields.io/badge/Endpoint-Sysmon-red)
![Wireshark](https://img.shields.io/badge/Network-Wireshark-blue)
![VirusTotal](https://img.shields.io/badge/Threat%20Intel-VirusTotal-green)
![PhishTool](https://img.shields.io/badge/Email-PhishTool-purple)
![Jira](https://img.shields.io/badge/ITSM-Jira-blue)

---

## 📌 Project Overview

This project is a practical **SOC Analyst L1 Security Monitoring and Incident Response Lab** designed to simulate real-world SOC operations.

The project demonstrates an end-to-end SOC workflow involving:

- Windows endpoint monitoring
- Security log collection and analysis
- SIEM-based threat detection
- SPL queries and investigations
- Security dashboards and alerts
- IOC investigation
- Network packet analysis
- Phishing email analysis
- Incident documentation
- Incident escalation and resolution

---

# 🧰 Tools Used

| Tool | Purpose |
|------|---------|
| **Sysmon** | Windows endpoint monitoring and telemetry |
| **Splunk** | SIEM, log analysis, detection, dashboards and alerts |
| **VirusTotal** | IOC investigation |
| **Wireshark** | Network and packet analysis |
| **PhishTool** | Phishing email analysis |
| **Jira** | Incident management and documentation |

---

# 🏗️ SOC Architecture

```text
                Windows Endpoint
                       │
                       ▼
                    Sysmon
                       │
                       ▼
              Windows Event Logs
                       │
                       ▼
                    Splunk
                       │
                Detection / Alert
                       │
                       ▼
                  Investigation
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
     VirusTotal    Wireshark    PhishTool
          │            │            │
          └────────────┼────────────┘
                       ▼
                 IOC Correlation
                       │
                       ▼
                     Jira
                       │
                       ▼
               Escalation / Closure
