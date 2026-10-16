---
name: incident-response-triage
description: Triage a suspected security incident using evidence preservation, scoping, containment planning, and a clear incident timeline. Use when reviewing suspicious logs, endpoint alerts, network indicators, or an incident report.
---

# Incident Response Triage

## 1. Establish scope and safety
Confirm the affected organization, systems, time window, reporting timezone, authority to investigate, and operational constraints. Treat alerts as leads rather than proof. Do not disrupt critical services or access systems beyond the authorized scope.

## 2. Preserve evidence
- Record when and how each artifact was obtained.
- Preserve original logs and files; analyze working copies where possible.
- Record host identifiers, time sources, hashes when appropriate, and chain-of-custody details.
- Normalize timestamps to a stated timezone while retaining original timestamps.
- Avoid cleanup, rebooting, or reimaging before evidence needs are considered, unless urgent containment requires it.

## 3. Build a timeline
Correlate endpoint, identity, DNS, proxy, firewall, VPN, cloud audit, and application logs as available. Separate observed events from inferred explanations. Record gaps, clock skew, and conflicting evidence.

## 4. Assess and scope
Determine affected assets, accounts, privileges, data, persistence indicators, initial access hypothesis, lateral movement, and external communication. Use confidence labels and identify what evidence would confirm or disprove each hypothesis. Avoid attributing activity to a person or group without adequate evidence.

## 5. Containment planning
Prioritize stopping ongoing harm while preserving critical evidence. Candidate actions may include isolating an endpoint, disabling compromised credentials, revoking sessions, blocking confirmed indicators, or restricting a vulnerable service. State the expected impact and rollback path for each action. Obtain the required incident commander or system-owner approval.

## 6. Eradication and recovery
Remove the root cause, rotate exposed secrets, patch exploited weaknesses, rebuild systems when integrity is uncertain, and restore from trusted backups. Validate monitoring and business-critical functionality before returning systems to service.

## 7. Report
Include executive summary, scope, timeline, evidence, indicators, impact, root-cause assessment, containment, recovery, and follow-up actions with owners. Mark unknowns explicitly and distinguish confirmed findings from hypotheses.

## Guardrails
Do not publish sensitive indicators or personal data unnecessarily. Do not execute malware or perform intrusive actions outside an isolated, authorized environment. Preserve the difference between “not observed” and “did not occur.”
