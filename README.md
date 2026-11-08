# Week 2 Final Project Report: Footprinting & Network Scanning

## 📌 Executive Summary
This repository contains the comprehensive Week 2 Final Report for the Networkwalks Cybersecurity & Ethical Hacking Internship (Batch B084). 

The objective of this project was to simulate the workflow of a penetration tester by combining passive reconnaissance (OSINT) and active network scanning. This report details the methodologies used, the evidence collected, the risk analysis of the findings, and actionable remediation recommendations for the target environment.

## 🎯 Targets & Scope
* **Target 1 (Passive Recon):** `networkwalks.com` (Authorized educational target)
* **Target 2 (Active Scanning):** Local Virtual LAN Subnet (Owned environment)
* **Disclaimer:** All activities were performed strictly within an authorized lab environment and comply with the Networkwalks liability disclaimer.

## 🛠️ Modules Covered & Tools Used

### 1. Footprinting & Reconnaissance (W2-PM1)
Conducted passive information gathering against a live domain using Kali Linux terminal tools to map the attack surface without alerting the target.
* **`whois`:** Extracted domain registration details and hosting provider (HostGator).
* **`whatweb`:** Fingerprinted the web technologies (WordPress, WP Download Manager, server IP).
* **`nslookup`:** Resolved the domain to its real IP address.
* **`curl -I`:** Analyzed HTTP response headers and exposed API endpoints.
* **`wafw00f`:** Detected the presence of a Web Application Firewall (ModSecurity).
* **`dnsrecon`:** Enumerated DNS records (MX, TXT, SRV) to map the infrastructure.

### 2. Network Scanning with Zenmap (W2-PM5)
Conducted active network discovery on a local subnet using Zenmap (Nmap GUI).
* **Local Discovery:** Identified the host IP and subnet mask using Windows CMD (`ipconfig`).
* **Ping Scan:** Discovered all live hosts, their IP addresses, and MAC addresses.
* **Topology Mapping:** Generated a visual network topology graph and exported it to PDF.

## 🚨 Key Findings & Risk Analysis
The report includes a detailed risk matrix categorizing the findings. Key observations include:
* **Information Leakage:** Publicly exposed CMS versions (WordPress 7.0.4) could allow attackers to search for known exploits.
* **Security Architecture:** The presence of a WAF means naive attacks will be blocked, requiring attackers to find bypasses.
* **Network Visibility:** Active hosts on the local network were easily mapped, highlighting the need for network access controls and device verification.

## 📄 The Final Report
The complete, professionally formatted PDF report includes:
1. Liability Disclaimer
2. Introduction
3. Tools Used
4. Activities Performed (with Screenshots)
5. Risk Analysis / Impact
6. Recommendations
7. Conclusion

👉 **[Click here to read the full PDF Report](WK2-FINAL-REPORT-ASIBEY-KITIABI-KOFFI-EMMANUEL.pdf)

---
**Author:** Asibey-Kitiabi Koffi Emmanuel
**Batch:** B084
**Instructor:** Waqas Karim CCIE
**Program:** Cybersecurity & Ethical Hacking Internship at Networkwalks
