# BlueTeam-SOC-Lab
Personal Wazuh SIEM lab with Windows agent, Sysmon integration, alert monitoring and threat hunting for junior SOC analyst portfolio.

Personal home lab for Security Operations Center (SOC) practice using Wazuh SIEM/XDR.

## Overview

This project simulates a real-world SOC environment with:
- Wazuh all-in-one deployment (manager, indexer, dashboard) via Docker on Ubuntu 22.04.
- Windows 11 endpoint with Wazuh agent and Sysmon (SwiftOnSecurity config).

- Log collection, alert generation, threat hunting, and MITRE ATT&CK mapping.

Perfect for junior SOC analyst portfolio – demonstrates SIEM monitoring, agent management, and alert triage.

## Features

- Wazuh v4.8.2 dashboard with active agent.
- Sysmon-enriched Windows logs (process creation, network connections).
- SCA (Security Configuration Assessment) – CIS Windows 11 benchmark.
- Threat Hunting module for alert analysis.

## Screenshots
<img width="1849" height="831" alt="overviewGitHub" src="https://github.com/user-attachments/assets/922f1c87-45c8-4703-8f50-b54530ec6dcf" />

<img width="1849" height="820" alt="ThreatHuntingGitHUb" src="https://github.com/user-attachments/assets/d17f352d-cfd2-4b04-a1c3-8de8c58e9f9a" />

## Setup

1. Ubuntu 24.04.3 LTS
2. Docker + Wazuh Docker single-node deployment
3. Windows 11 VM with Wazuh agent and Sysmon (SwiftOnSecurity config)

## Future Improvements

- Custom Wazuh rules for high-severity registry persistence alerts.
- TheHive SOAR integration.
- MISP threat intelligence feed.

## Author

Junior Cybersecurity Analyst | Aspiring SOC Analyst
Open to junior SOC / Blue Team roles.
