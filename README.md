# Wazuh SIEM Home Lab

**SOC Analyst L1 Lab · SIEM Deployment · Security Monitoring**

> 🟢 **Status: Active — evidence and detections are being expanded**

### 🧰 Stack
<img src="https://img.shields.io/badge/Wazuh-4A90E2?logo=wazuh&logoColor=white" alt="Wazuh"> <img src="https://img.shields.io/badge/Windows-0078D4?logo=windows&logoColor=white" alt="Windows"> <img src="https://img.shields.io/badge/SIEM-Security_Monitoring-555555" alt="SIEM">

## 🎯 Why I built this lab
I want hands-on experience with the full SIEM workflow — from getting useful telemetry into the platform to investigating an alert and explaining what the evidence means.

## 🏗️ Lab architecture

```text
[ Monitored Endpoint ]
          |
     Wazuh Agent
          |
   [ Wazuh Manager ]
          |
   [ Wazuh Indexer ]
          |
   [ Wazuh Dashboard ]
```

## 🔎 Analyst workflow

1. Deploy the Wazuh Manager, Indexer and Dashboard.
2. Register Wazuh Agent(s) on monitored endpoints.
3. Onboard relevant Windows/Linux security logs.
4. Validate ingestion and baseline alerting.
5. Create or customise detections for selected security events.
6. Investigate alert volume, severity and affected endpoints.
7. Document the finding as an analyst handoff.

## 🧠 What this lab is teaching me
**Telemetry quality → detection quality → investigation quality.**

A SIEM is only useful to a SOC analyst when the underlying data is available, the detection is meaningful and the alert can be investigated with enough context.

## 📌 Evidence roadmap

The lab will be expanded with sanitised evidence covering:

- Wazuh dashboard overview
- Agent registration and health
- Triggered security alert
- Detection-rule configuration
- Raw event/log evidence
- Analyst-style alert write-ups

## Scope & ethics
Controlled home-lab environment only. No unauthorised production systems are targeted.
