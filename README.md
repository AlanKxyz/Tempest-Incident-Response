# Tempest Incident Response (SOC Analyst L1 Portfolio Project)

## Project Overview

This repository documents my investigation of the **Tempest Incident Response** scenario.

The objective was to simulate the work of a SOC Level 1 analyst responsible for triaging, investigating, and documenting a malware intrusion using Windows forensic artifacts and network traffic.

Rather than simply answering challenge questions, this project focuses on demonstrating:

- Incident investigation workflow
- Log analysis
- IOC extraction
- Timeline reconstruction
- MITRE ATT&CK mapping
- Detection engineering
- Professional incident documentation

---

## Scenario

A critical security alert was escalated from the SOC monitoring team.

Initial evidence suggested the execution of a malicious Microsoft Word document that initiated a multi-stage malware infection.

Available evidence included:

- Windows Event Logs
- Sysmon Logs
- PCAP Capture
- Security Alerts

---

## Investigation Goals

- Determine initial access
- Identify executed malware
- Trace attacker activity
- Discover persistence mechanisms
- Extract Indicators of Compromise
- Build attack timeline
- Recommend detection improvements

---

## Tools Used

- Sysmon
- Windows Event Viewer
- Wireshark
- Timeline Explorer
- PowerShell
- MITRE ATT&CK Navigator

---

## Skills Demonstrated

✔ Incident Response

✔ Log Analysis

✔ Windows Forensics

✔ Network Forensics

✔ IOC Hunting

✔ MITRE ATT&CK Mapping

✔ Malware Investigation

✔ Documentation

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

Persistence
↓

Command & Control Communication
↓

Privilege Escalation
↓

Credential Access

---

## Repository Structure

Timeline/

IOC/

Detection/

MITRE-ATTACK/

Evidence/

Lessons-Learned/

---

## Key Takeaways

This project improved my ability to:

- correlate multiple log sources
- identify attacker behavior
- document an investigation
- understand attacker TTPs
- communicate findings clearly

The repository is intended to represent the type of documentation expected from a junior SOC Analyst or Incident Responder.
