# Secure Docker Network Architecture

## Overview
This project is a proof-of-concept for a secure, segmented containerized environment. I designed and implemented a Docker architecture consisting of three separate networks (Private, DMZ, and Public), each tailored with distinct permission boundaries and monitoring requirements.

## Key Features & Architecture
* **Network Segmentation:** Enforced strict isolation between Private, DMZ, and Public Docker networks to limit lateral movement.
* **Network Security:** Configured a Suricata router for Intrusion Detection/Prevention (IDS/IPS) and integrated CoreDNS for internal network resolution.
* **Internal Observability Stack:** Deployed a comprehensive monitoring and security logging stack natively within the environment utilizing:
  * **Prometheus & Grafana** for metrics and visual monitoring.
  * **Wazuh Manager** for SIEM and security posture management.

## Tech Stack
* Docker / Docker Compose
* Suricata
* CoreDNS
* Prometheus & Grafana
* Wazuh

*(Note: This project was built as part of my Networking and Cloud Automation studies at Fontys University.)*