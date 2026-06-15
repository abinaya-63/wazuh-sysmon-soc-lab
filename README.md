# Wazuh + Sysmon SOC Monitoring Lab

## Project Overview

This project demonstrates how to integrate Wazuh SIEM with Sysmon on a Windows 10 endpoint for Security Operations Center (SOC) monitoring and threat detection.

The lab collects Windows events, Sysmon logs, PowerShell activity, and failed login attempts, then analyzes them using Wazuh custom detection rules.

---

## Architecture

Windows 10 (Sysmon Installed)
        |
        |
   Wazuh Agent
        |
        |
 Ubuntu Wazuh Manager
        |
        |
 Wazuh Dashboard

---

## Technologies Used

- Wazuh SIEM
- Sysmon
- Windows 10
- Ubuntu Server
- VMware Workstation
- PowerShell

---

## Detection Use Cases

### 1. PowerShell Activity Detection

Detected PowerShell execution using Sysmon Event ID 1.

Custom Rule:

- Rule ID: 100100
- Level: 10

Description:

Custom Alert: PowerShell Discovery Activity Detected

---

### 2. Failed Login Detection

Detected Windows failed logon attempts using Event ID 4625.

Custom Rule:

- Rule ID: 100101
- Level: 12

Description:

Custom Alert: Windows Failed Login Detected

---

## Custom Wazuh Rules

See:

local_rules.xml

---

## Screenshots

Screenshots are available in the Screenshots folder.

---

## Skills Demonstrated

- SIEM Monitoring
- Threat Hunting
- Log Analysis
- Sysmon Configuration
- Wazuh Rule Creation
- Windows Event Monitoring
- Security Operations (SOC)

---

## Outcome

Successfully built a SOC monitoring lab capable of:

- Detecting PowerShell activity
- Monitoring Windows failed logins
- Creating custom Wazuh rules
- Centralizing endpoint security logs
- Performing threat hunting using Wazuh Dashboard

---

## Author

Abinaya S

B.E CSE (Cyber Security)

Dr. Mahalingam College of Engineering and Technology
