
![Alt text](/CloudTrail-Even-History-Screenshot.png)
![Alt text](/Microsoft-Sentinel-Data-connector-Screenshot.png)
![Alt text](/Microsoft-Sentinel-Log-Screenshot.png)
![Alt text](/Microsoft-SentinelLog-from-CloudTrail.png)


# AWS-Threat-Detection-Incident-Simulation-Lab

## 📌 Overview
This project simulates real-world cloud attack scenarios in AWS and builds detection workflows using CloudTrail, GuardDuty, and Microsoft Sentinel.

The goal was to understand how attacker behavior appears in logs and how security teams detect, investigate, and respond to threats in cloud environments.

---

## 🧠 Key Capabilities
- Cloud threat detection using GuardDuty + Sentinel  
- CloudTrail log analysis for incident investigation  
- IAM abuse and privilege escalation detection  
- End-to-end incident response workflow  

---

## 🏗️ Architecture

![Architecture Diagram](./screenshots/architecture-diagram.png)

---

## ⚔️ Attack Scenarios Simulated

- Credential compromise (stolen IAM keys)
- Privilege escalation via IAM misconfiguration
- Unauthorized API activity
- Resource enumeration (IAM, S3)
- Suspicious console/CLI usage

---

## 🔍 Detection Workflow

1. Simulate attacker behavior in AWS
2. Capture activity via CloudTrail
3. Analyze GuardDuty findings
4. Forward logs to Microsoft Sentinel
5. Create and tune detection rules
6. Investigate and document response actions

---

## 📊 Key Outcomes

- Improved detection visibility for IAM-based attacks  
- Built correlation rules to identify suspicious API behavior  
- Reduced noise by tuning alert thresholds in Sentinel  
- Developed a structured incident investigation workflow  

---

## 🧪 Example Detection

| Scenario | Detection Method |
|----------|----------------|
| IAM Privilege Escalation | CloudTrail API pattern analysis |
| Credential Abuse | GuardDuty anomaly detection |
| Enumeration Activity | Sentinel correlation rules |

---

## 📁 Repository Structure

```bash
.
├── detections/
├── logs/
├── incident-response/
├── screenshots/
└── README.md

