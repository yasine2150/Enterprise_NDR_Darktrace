# Enterprise Network Detection & Response (NDR) Architecture & Deployment

## 🛡️ Project Overview
This repository details the complete lifecycle of acquiring, designing, and implementing a Network Detection and Response (NDR) solution within a highly regulated financial institution . Designed to comply with stringent regulatory frameworks (BCT Circular 2006-19), this project bridges the "internal blind spot" left by legacy signature-based Intrusion Detection Systems (IDS) and Next-Generation Firewalls (NGFW).

By leveraging **Darktrace** and unsupervised Machine Learning (ML), the deployed architecture successfully identifies zero-day threats, lateral movement, and advanced persistent threats (APTs) using behavioral baselining rather than static rules.

## 🏗️ Architectural Design
The deployment was integrated into the primary data center with a focus on zero-latency and high availability:
* **Passive Traffic Ingestion:** Utilized SPAN port mirroring to ensure zero disruption to operational technology and banking services.
* **Forensic Synchronization:** Integrated with internal NTP infrastructure for highly accurate, timestamped forensic logging.
* **Secure Telemetry:** Established a least-privilege firewall whitelist for the Call-Home telemetry channel to maintain data sovereignty.
* **Management:** Allocated static management IP routing for secure SOC access.

## 🧠 Core Capabilities
* **Unsupervised Machine Learning:** Moving beyond reactive, signature-based security to mathematical modeling of "normal" enterprise behavior.
* **Cyber AI Analyst:** Autonomous investigation and correlation of anomalous events, dramatically reducing alert fatigue (condensing 5.8 billion raw network events into 30 structured, high-fidelity incidents).
* **Definitive "Ground Truth":** Utilizing raw network packets to bypass the limitations of manipulatable SIEM log data.

## 🔍 Documented Threat Case Studies
The effectiveness of the NDR deployment was validated against real-world network traffic, including:
1. **Vulnerability Scanning vs. Malicious Reconnaissance:** Distinguishing authorized Tenable vulnerability scans from malicious HTTP probing (e.g., Nikto URI signatures).
2. **C2 Beaconing via Port 443:** Autonomous detection of stealthy, malware-generated outbound communications to external rare endpoints without standard HTTP User-Agent headers.
3. **Multi-Device DGA Malware Correlation:** Identification of a coordinated malware campaign utilizing Domain Generation Algorithms (DGA) across multiple internal endpoints simultaneously.

## 🛠️ Technologies & Concepts
`Darktrace` `Network Detection & Response (NDR)` `Unsupervised Machine Learning` `SPAN/Port Mirroring` `Zero-Day Threat Detection` `SOC Visibility Triad` `Cybersecurity Architecture`
