# Detection 02 — Suspicious PowerShell Execution

**Status:** Planned / lab validation pending

## Objective
Identify PowerShell activity that deserves investigation based on execution context, command characteristics and surrounding endpoint events.

## Data sources
- Windows process telemetry
- PowerShell logging where enabled
- Related authentication and endpoint events

## Investigation signals
Review for combinations of:

- Unusual parent/child process relationships
- Encoded or obfuscated command content
- Unexpected execution by a user or service
- Execution from unusual paths
- Related network connections

## L1 triage questions
1. Who launched PowerShell?
2. What was the parent process?
3. What command or script was executed?
4. Is the execution expected for the host/user?
5. Are there related network, persistence or credential events?

## Expected analyst output
Record the process chain, user, host, timestamps, relevant command evidence, verdict, severity and escalation recommendation.

> This document defines a lab detection/investigation approach. It does not represent a confirmed malicious event.
