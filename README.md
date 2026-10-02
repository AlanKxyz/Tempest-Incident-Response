# Tempest Incident Response

## Executive Summary

This project documents a complete DFIR (Digital Forensics & Incident Response) investigation of a compromised Windows workstation.

The investigation identified a malicious Microsoft Word document as the initial infection vector. The document executed PowerShell commands which downloaded additional malware payloads, established persistence, and communicated with external infrastructure.

The objective of this project was to simulate the responsibilities of a SOC Level 1 Analyst and demonstrate the ability to:

- Triage security alerts
- Analyze Windows forensic artifacts
- Investigate attacker activity
- Extract Indicators of Compromise (IOCs)
- Reconstruct an attack timeline
- Map activity to MITRE ATT&CK
- Create detection content
- Produce professional incident documentation

---

## Scenario

A security alert was escalated from the SOC monitoring platform after suspicious activity was detected on a Windows workstation.

Evidence suggested execution of a malicious Microsoft Word document followed by PowerShell activity, malware download behavior, persistence creation, and outbound communication to attacker-controlled infrastructure.

Available evidence included:

- Windows Security Logs
- Sysmon Logs
- Network Packet Capture (PCAP)
- Endpoint Security Alerts

---

## Investigation Objectives

- Identify initial access vector
- Determine malware execution chain
- Investigate attacker behavior
- Identify persistence mechanisms
- Extract Indicators of Compromise
- Reconstruct attack timeline
- Map techniques to MITRE ATT&CK
- Develop detection opportunities
- Recommend security improvements

---

## Tools Used

| Tool | Purpose |
|--------|----------|
| Sysmon | Endpoint telemetry |
| Windows Event Viewer | Log analysis |
| Wireshark | Network traffic analysis |
| Timeline Explorer | Timeline reconstruction |
| PowerShell | Artifact analysis |
| MITRE ATT&CK Navigator | Technique mapping |

---

## Skills Demonstrated

### Incident Response

- Alert triage
- Incident investigation
- Evidence correlation

### Forensics

- Windows log analysis
- Sysmon event analysis
- Timeline reconstruction

### Threat Hunting

- IOC extraction
- Process activity analysis
- Network investigations

### Detection Engineering

- Sigma rule creation
- Detection recommendations
- ATT&CK mapping

---

## Attack Flow

Initial Access
↓
Malicious Word Document
↓
PowerShell Execution
↓
Payload Download
↓
Persistence Creation
↓
C2 Communication
↓
Privilege Escalation
↓
Credential Access

---

## Repository Structure

```text
Tempest-Incident-Response
│
├── Timeline
│   └── Attack Timeline.md
│
├── IOC
│   └── IOC Report.md
│
├── Detection
│   └── Detection Opportunities.md
│
├── Sigma
│   └── Suspicious PowerShell Download.yml
│
├── MITRE Mapping
│   └── ATTACK Mapping.md
│
└── Lessons Learned
    └── Lessons Learned.md
``
