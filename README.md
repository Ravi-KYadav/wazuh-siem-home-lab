# Wazuh SIEM Home Lab

**SOC Analyst L1 Lab · SIEM Deployment · Security Monitoring**

> 🟢 **Status: Active — evidence and detections are being expanded**

### 🧰 Stack
<img src="https://img.shields.io/badge/Wazuh-4A90E2?logo=wazuh&logoColor=white" alt="Wazuh"> <img src="https://img.shields.io/badge/Windows-0078D4?logo=windows&logoColor=white" alt="Windows"> <img src="https://img.shields.io/badge/SIEM-Security_Monitoring-555555" alt="SIEM">

## 🎯 Lab objective
Build a repeatable SIEM workflow using Wazuh and Windows telemetry, from endpoint log collection through alert investigation and L1 analyst handoff.

## 🗺️ Repository map

| Path | Purpose |
|---|---|
| [`docs/`](docs/) | Lab architecture, setup and analyst workflow |
| [`detections/`](detections/) | Detection concepts and L1 investigation playbooks |
| [`cases/`](cases/) | Sanitised investigation cases and reporting template |
| [`evidence/`](evidence/) | Evidence naming, quality and sanitisation standard |

## 🏗️ Lab architecture

```text
[ Monitored Windows Endpoint ]
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

1. **Identify** the alert, host, user, timestamp and severity.
2. **Validate** whether the activity is expected or anomalous.
3. **Collect** supporting endpoint, account and network evidence.
4. **Correlate** related events into a timeline.
5. **Assess** confidence, impact and urgency.
6. **Decide** whether to close, monitor or escalate.
7. **Document** the evidence, verdict and next action.

## 🛡️ Detection catalogue

| Detection / investigation | Focus | Status |
|---|---|---|
| [Repeated failed logons](detections/01-brute-force-detection.md) | Authentication anomaly / brute-force investigation | 🟡 Lab validation |
| [Suspicious PowerShell](detections/02-suspicious-powershell.md) | Process context / command investigation | 🟡 Lab validation |
| [Log clearing / audit tampering](detections/03-log-clearing-investigation.md) | Security telemetry tampering | 🟡 Lab validation |

> **Important:** Detection documents describe the investigation methodology. They are not presented as confirmed production detections until they are validated with lab evidence.

## 🧠 Analyst principle
**Telemetry quality → detection quality → investigation quality.**

A useful SIEM workflow depends on reliable telemetry, meaningful detections and enough context to support an evidence-based conclusion.

## 📌 Evidence roadmap

Planned sanitised evidence includes:

- Wazuh dashboard overview
- Agent registration and health
- Triggered security alerts
- Detection-rule configuration
- Raw event/log evidence
- Analyst-style case write-ups

## Scope & ethics
Controlled home-lab environment only. No unauthorised production systems are targeted. Secrets and sensitive data are excluded from public evidence.
