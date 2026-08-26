# Wazuh SIEM Home Lab

A self-built home lab implementing Wazuh as a SIEM to collect, parse, correlate, and alert on security events — built to gain hands-on experience with the core SIEM workflows used in a SOC.

## 🎯 Objective

To understand how a SIEM works in practice — not just in theory — by deploying one from scratch, feeding it real log data, writing detection rules, and building visibility into a monitored environment.

## 🧰 Environment & Tools

| Component | Details |
|---|---|
| SIEM Platform | Wazuh (Manager + Indexer + Dashboard) |
| Host OS | *<!-- e.g. Ubuntu Server 22.04 on VirtualBox / VMware -->* |
| Monitored Endpoint(s) | *<!-- e.g. Windows 10 VM with Wazuh Agent installed -->* |
| Virtualization | *<!-- VirtualBox / VMware / Proxmox -->* |
| Network | *<!-- host-only / NAT network setup -->* |

## 🏗️ Architecture

```
[ Monitored Endpoint(s) ]  --Wazuh Agent-->  [ Wazuh Manager ]  -->  [ Wazuh Indexer ]  -->  [ Wazuh Dashboard ]
```

*<!-- Replace with your actual architecture diagram/screenshot -->*

## 🔧 Methodology

1. **Deployment**
   - Installed the Wazuh stack (Manager, Indexer, Dashboard) on a dedicated VM
   - Installed the Wazuh Agent on the monitored endpoint(s) and registered it with the Manager
2. **Log Source Configuration**
   - Configured log collection for *<!-- e.g. Windows Event Logs, Sysmon, auth logs -->*
   - Verified log ingestion was flowing correctly into the Indexer
3. **Detection Rule / Alert Configuration**
   - Reviewed default Wazuh ruleset and ran test events to confirm baseline alerting
   - Created/customized rules for *<!-- e.g. failed login attempts, new process execution, file integrity changes -->*
4. **Dashboard & Visualization**
   - Built dashboards to visualize alert volume, top event types, and affected endpoints
   - Configured alert severity thresholds

## 🔍 Key Findings / Screenshots

*<!-- Add 3–5 screenshots here: Wazuh dashboard overview, a triggered alert, the rule that generated it, and the raw log entry. Each screenshot should have a one-line caption explaining what it shows. -->*

**Example caption format:**
> Screenshot: Wazuh Dashboard showing X alerts triggered over 24 hours, majority classified as [severity level].

## 🧠 Skills Demonstrated

- SIEM deployment and configuration
- Log source onboarding and normalization
- Custom detection rule writing
- Alert triage using dashboard visualizations
- Understanding of the log collection → correlation → alerting pipeline

## 📚 What I Learned

*<!-- Write 3-4 sentences in your own words: what was harder than expected, what you'd do differently, and how this connects to what a SOC L1 analyst does day-to-day (e.g. "This gave me a first-hand understanding of why log source coverage matters — an alert is only as good as the data feeding it.") -->*

## 🔗 Related

Part of a 5-project SOC Analyst portfolio. See also: [SOC Alert Triage Practice](https://github.com/Ravi-KYadav/soc-alert-triage-practice) · [MITRE ATT&CK Mapping](https://github.com/Ravi-KYadav/mitre-attack-threat-intel-mapping)
