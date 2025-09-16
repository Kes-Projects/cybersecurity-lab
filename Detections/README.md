# Detections From Kali Lunix Attacks On Both Windows 11 and Ubuntu Server

## Windows 11 Detections


Shows the unauthorized login attempt from the Kali machine using Hydra tool with remote desktop protocol. All failed logs were sent to the SIEM.

**Failed RDP Detection Screenshot:**
![Login Attempts](https://github.com/user-attachments/assets/9bfb7fb5-f623-4a20-9ac1-fad1e6c85771)

Logs from the Wazuh SIEM shows the smbclient attack on the windows machine that attempts to log in as an authorized user has failed.

**SMBClient Detection Screenshot:**
![SMBClient](https://github.com/user-attachments/assets/61400437-9d83-4d93-a10c-8e69b490961d)


----

## Ubuntu Server Detections


This document describes an SSH attack launched from the Kali machine, including the attacker’s IP address and the username used to access the Ubuntu server. 

**SSH Detection Screenshot:**
![SSH](https://github.com/user-attachments/assets/645f4645-b533-4c9b-8d04-3fc628727340)

Shows that the ssh attack from Kali was unsuccessful against the Ubuntu Server machine

**SSH Unsuccessful Login Detection Screenshot:**
![SSH](https://github.com/user-attachments/assets/36b821ee-c677-4723-9ddb-5fccdaa58242)

Wazuh SIEM detected a failed SSH login attempt from the Kali machine, showing information about the attacker and indicating that the maximum number of authentication attempts was exceeded.

**SSH Brute Force Unsuccessful Detection Screenshot:**
![SSH](https://github.com/user-attachments/assets/34e5efb9-b2fb-4458-9e43-68086a264561)


Apache was installed on the Ubuntu server to record logs of Nikto scans launched from the Kali machine. The logs capture vulnerability scanning activity performed by Nikto on the Ubuntu server.

**Apache2 Shows Detection Logs From Nikto Attacks Screenshot:**
![APACHE](https://github.com/user-attachments/assets/5099186b-dda4-40be-846f-621b5cd8967e)

The Wazuh SIEM dashboard displays the total number of authentication failures as well as the count of successful logins.

**Wazuh Dashboard with Total Detections From Authentication Failure Screenshot:**
![DASHBOARD](https://github.com/user-attachments/assets/16bdc400-b2e0-4c06-b6e7-6175c387157d)



