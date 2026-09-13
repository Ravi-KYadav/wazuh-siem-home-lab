# Detection 01 — Windows Brute-Force / Repeated Failed Logons

**Status:** Planned / lab validation pending

## Objective
Identify repeated failed authentication activity against a Windows endpoint and provide enough context for L1 triage.

## Data source
- Windows Security event telemetry collected by Wazuh
- Authentication events

## Detection logic
Look for repeated failed logon events within a defined time window, then correlate:

- Target account
- Source host/IP where available
- Timestamp pattern
- Logon type
- Successful logon following failures

## L1 triage questions
1. Is the account a valid user or service account?
2. Is the source expected for that account?
3. Did a successful authentication follow the failures?
4. Are there related endpoint or network alerts?
5. Does the activity justify escalation?

## Expected analyst output
Document the alert, affected account/host, evidence timeline, verdict, severity and recommended action.

> This document defines the detection approach. It does not claim a production detection or confirmed malicious activity.
