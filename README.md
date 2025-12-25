# BlueTeam-SOC-Lab

Hands-on SOC home lab built with Wazuh SIEM/XDR to practice Windows security monitoring, alert triage, threat hunting, and detection engineering concepts.

This project is designed as a **junior SOC analyst portfolio lab**, focusing on how alerts are generated, investigated, validated, and documented in a realistic environment.

---

## Overview

This lab simulates a small-scale enterprise SOC environment with centralized log collection and endpoint visibility.

It demonstrates:
- SIEM deployment and management
- Windows endpoint telemetry collection
- Alert analysis and triage
- Threat hunting using real Windows event data
- MITRE ATT&CK–aligned detections

The goal is not just to generate alerts, but to understand **why alerts fire, when they don’t, and how detection gaps are identified**.

---

## Architecture

- **Wazuh SIEM/XDR (v4.8.2)**  
  - Manager, Indexer, Dashboard deployed via Docker  
- **Ubuntu 24.04 LTS**  
  - Hosts the Wazuh stack  
- **Windows 11 VM**  
  - Wazuh agent installed  
  - Sysmon enabled (SwiftOnSecurity configuration)

---

## Key Capabilities

- Centralized Windows log ingestion (Security, System, PowerShell)
- Sysmon-enriched telemetry:
  - Process creation
  - Command-line logging
  - Network activity
- Alert monitoring and investigation via Wazuh Dashboard
- Threat hunting using indexed event data
- MITRE ATT&CK mapping for relevant alerts
- Security Configuration Assessment (SCA):
  - CIS Windows 11 benchmark

---

## Example Use Cases

- Investigating Windows authentication events
- Reviewing PowerShell Script Block Logging (Event ID 4104)
- Analyzing service configuration changes (e.g., BITS startup type)
- Distinguishing informational vs suspicious alerts
- Practicing SOC-style alert documentation and closure decisions

---

## Screenshots

**Wazuh Dashboard Overview**
<img width="1849" height="831" alt="overviewGitHub" src="https://github.com/user-attachments/assets/922f1c87-45c8-4703-8f50-b54530ec6dcf" />

**Threat Hunting Interface**
<img width="1849" height="820" alt="ThreatHuntingGitHUb" src="https://github.com/user-attachments/assets/d17f352d-cfd2-4b04-a1c3-8de8c58e9f9a" />

---

## Setup Summary

1. Ubuntu 24.04.3 LTS
2. Docker & Docker Compose
3. Wazuh single-node Docker deployment
4. Windows 11 virtual machine
5. Wazuh agent + Sysmon (SwiftOnSecurity config)

---

## Current Focus

- Alert triage and SOC-style investigation notes
- Understanding detection logic and limitations
- Identifying detection gaps in PowerShell and Windows telemetry

---

## Planned Enhancements

- Custom Wazuh rules for persistence and defense evasion techniques
- Detection gap analysis and documentation
- TheHive SOAR integration
- MISP threat intelligence integration

---

## Author

Junior Cybersecurity Analyst  
Aspiring SOC / Blue Team Analyst  

This lab reflects continuous learning and practical SOC workflows rather than automated “alert spam” demonstrations.
