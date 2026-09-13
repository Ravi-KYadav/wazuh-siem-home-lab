# Detection 03 — Security Log Clearing / Audit-Trail Tampering

**Status:** Planned / lab validation pending

## Objective
Surface events indicating that Windows security logging may have been cleared or otherwise tampered with, then determine whether the activity is administrative, expected or suspicious.

## Data sources
- Windows Security event telemetry
- Wazuh alert context
- Related account and process activity

## Investigation sequence
1. Identify the log-clearing event and timestamp.
2. Identify the initiating user/account where available.
3. Review nearby process and authentication activity.
4. Check for preceding suspicious activity that could explain the action.
5. Assess whether the event is expected administrative maintenance.

## L1 triage questions
- Who performed the action?
- Was the action authorised?
- What happened immediately before it?
- Were there failed/successful logons or suspicious processes nearby?
- Is escalation required to preserve evidence and investigate further?

## Expected analyst output
Produce a concise timeline, evidence summary, verdict, severity and recommended next action.

> This document defines an investigation approach and does not claim that log tampering has occurred in a production environment.
