

# Security Homelab with pfSense, Wazuh, Windows, Ubuntu, and Kali

## Overview

This project demonstrates the design and deployment of a virtualized security homelab environment.
The goal is to simulate **real-world enterprise security monitoring** by using pfSense as a firewall/router, Wazuh for endpoint security monitoring, and Kali Linux for penetration testing.

---

## Lab Architecture

* **pfSense** → Firewall & Router with 3 LANs

  * Server LAN → `10.x.x.x/24`
  * Client LAN → `10.x.x.x/24`
  * Management LAN (Wazuh) → `10.x.x.x/24`

* **Windows Server 2022** →  Test server with wazuh agent
* **Windows 11 Client** → Test desktop with wazuh agent
* **Ubuntu Server** → Test server with wazuh agent 
* **Ubuntu Desktop** → Test desktop with wazuh agent
* **Kali Linux** → Attacker machine for penetration testing
* **Wazuh Manager** → Endpoint detection and response (EDR)

*(Insert network diagram image here)*

---

## Features Implemented

Configured pfSense with multiple LAN segments
Installed and configured **Wazuh agent** on Windows Server, Windows 11, Ubuntu Server & Ubuntu Desktop
Simulated **attacks from Kali Linux** against Windows & Ubuntun machines (brute force, network scans, exploits)
Verified endpoint logging & alerting in **Wazuh**

---

## Attack & Detection Scenarios

1. **Nmap Scanning from Kali → Server LAN**
   * Logs captured by Wazuh
  
2. **Brute Force RDP/SMB Attempt from Kali → Windows 11**
   * Detected and logged by Wazuh/Splunk
    
3. **Malicious file execution on Windows client**
   * Endpoint alerts in Wazuh

---

## Tools & Technologies

* pfSense
* Wazuh
* Kali Linux
* Windows Server 2022
* Windows 11
* Ubuntu Server
* Ubuntu Desktop

---

## Future Improvements

* Add Suricata or Snort for **network intrusion detection**
* Simulate ransomware or phishing attacks in a safe lab environment
* Automate log forwarding to Splunk with custom dashboards
* Expand to include Linux servers as additional monitored endpoints
* Add Splunk for advanced search & analytics with threat hunting

---

