# Wazuh SIEM Home Lab

**SOC Analyst L1 Portfolio Project · SIEM Deployment & Security Monitoring**

> **Status: Active / being expanded with lab evidence**

## Objective
Build practical understanding of the SIEM workflow by deploying Wazuh, onboarding endpoint telemetry, validating log ingestion, configuring detections and using dashboards for security monitoring.

## Planned Lab Architecture

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

## Core Workflow

1. Deploy the Wazuh Manager, Indexer and Dashboard.
2. Install and register Wazuh Agent(s) on monitored endpoints.
3. Onboard relevant Windows/Linux security logs.
4. Validate ingestion and baseline alerting.
5. Create or customize detection rules for selected security events.
6. Use dashboards to investigate alert volume, severity and affected endpoints.
7. Document observations as an analyst handoff.

## SOC Skills Demonstrated

- SIEM deployment and configuration
- Log-source onboarding
- Detection-rule concepts
- Alert investigation
- Dashboard-based monitoring
- Understanding the log collection → correlation → alerting pipeline

## Evidence Roadmap

The repository will be expanded with sanitized screenshots covering:

- Wazuh dashboard overview
- Agent registration and health
- Triggered security alert
- Detection rule configuration
- Raw event/log evidence

## Analyst Perspective

This lab is designed to demonstrate that effective SOC monitoring depends on **good telemetry, meaningful detections and evidence-based investigation** rather than simply deploying a security platform.

## Scope & Ethics

Controlled home-lab environment only. No unauthorized production systems are targeted.