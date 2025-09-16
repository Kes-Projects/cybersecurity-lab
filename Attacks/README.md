# Explanation and Images of Attacks on **Windows** and **Ubuntu** Machines

## Attacks on Windows Machine

Executed an authorized lab exercise simulating unauthorized access using a brute-force attack on a remote desktop with a password wordlist for detection and logging validation.

**RDP Attack Screenshot:**  
![RDP Attack](https://github.com/user-attachments/assets/1d34ac7a-a26e-48d9-ba70-68e50a3d72b9)

I used `smbclient` to enumerate shares and attempt authentication against the target host using the account "Kay Bee".

**SMB Enumeration Screenshot:**  
![SMB Enumeration](https://github.com/user-attachments/assets/54c3a379-f1de-46c6-9c7f-482f9ad03c46)


I used Nmap to perform network reconnaissance, including discovering active hosts, scanning open ports, identifying running services and their versions, and detecting the operating system. Despite these scans, the activity was not detected or flagged by the Wazuh SIEM on the target system.


---

## Attacks on Ubuntu Machine

**SSH Attack Screenshot:**
![SSH Attack](https://github.com/user-attachments/assets/af5670f5-cce0-4eb3-aee8-f9b4438e7975)
