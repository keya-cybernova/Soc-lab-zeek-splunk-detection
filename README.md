# Soc-lab-zeek-splunk-detection
SOC lab project detecting port scanning attacks using Zeek and Splunk SIEM
# 🔐 SOC Lab: Threat Detection using Zeek & Splunk

## 📌 Project Overview

This project demonstrates a real-world SOC (Security Operations Center) workflow where network traffic is monitored, logs are forwarded, and attacks are detected using SIEM.
 🧩 Architecture

* Ubuntu → Zeek (Network Monitoring)
* Kali Linux → Attacker (Nmap) + Splunk Universal Forwarder
* Windows → Splunk Enterprise (SIEM)

---
⚙️ How the Project Works

1. Zeek captures network traffic and generates logs (conn.log)
2. Kali Linux simulates an attack using Nmap
3. Splunk Universal Forwarder sends logs to Splunk SIEM
4. Splunk analyzes logs and detects suspicious activity

## 🚨 Attack Simulation

* Tool used: Nmap
* Command:

```bash
nmap -sS 192.168.56.103
```

* Type: Port Scanning Attack

---
🔍 Detection in Splunk

The attack was detected by analyzing repeated TCP connection attempts from a single source IP.

👉 Attacker IP: **192.168.56.101**
👉 Behavior: Multiple port scanning attempts

---

## 📸 Screenshots

![Detection](detection.png)

---

## 🛠️ Tools & Technologies

* Zeek
* Splunk Enterprise
* Splunk Universal Forwarder
* Kali Linux
* Nmap
* Ubuntu Linux

---

## 🎯 Key Learnings

* Built end-to-end SOC pipeline
* Log analysis using Splunk
* Detection of reconnaissance attacks
* Troubleshooting real-world issues

---

## 🚀 Conclusion

Successfully built a SOC lab and detected a port scanning attack using Zeek and Splunk.

