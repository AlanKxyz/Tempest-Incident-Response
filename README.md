# Tempest Incident Response

DFIR investigation of a compromised Windows workstation using Sysmon, Windows Event Logs, Wireshark, PowerShell, and network traffic analysis.

---

## Overview

This repository documents a complete incident response investigation performed against a simulated malware infection scenario.

The goal of the project was to investigate a suspected endpoint compromise, identify attacker activity, extract Indicators of Compromise (IOCs), reconstruct the attack timeline, map observed techniques to MITRE ATT&CK, and develop detection opportunities.

This project simulates the responsibilities typically performed by a:

- SOC Analyst Level 1
- Junior Incident Responder
- Cybersecurity Analyst
- DFIR Analyst

---

## Executive Summary

A Windows workstation was compromised after a user executed a malicious Microsoft Word document.

The document launched PowerShell, which was subsequently used to download and execute additional malware components.

Analysis of endpoint telemetry and network traffic revealed:

- Malicious document execution
- PowerShell abuse
- Payload delivery
- Persistence establishment
- Command-and-Control communication
- Potential credential access activity

The complete attack chain was reconstructed using Sysmon logs, Windows Event Logs, endpoint artifacts, and packet capture analysis.

---

## Investigation Objectives

The investigation aimed to:

- Identify the initial access vector
- Determine how malware executed
- Investigate attacker activity
- Discover persistence mechanisms
- Extract Indicators of Compromise
- Reconstruct a forensic timeline
- Map activity to MITRE ATT&CK
- Create detection opportunities
- Recommend remediation actions

---

## Environment

### Evidence Sources

- Sysmon Logs
- Windows Event Logs
- Security Alerts
- Network Packet Capture (PCAP)
- Endpoint Artifacts

### Tools Used

- Sysmon
- Windows Event Viewer
- Wireshark
- Timeline Explorer
- PowerShell
- MITRE ATT&CK Navigator

---

## Skills Demonstrated

### Incident Response

- Alert Triage
- Incident Investigation
- Evidence Correlation

### Windows Forensics

- Process Analysis
- Event Log Analysis
- Sysmon Investigation

### Network Forensics

- DNS Analysis
- HTTP Traffic Analysis
- C2 Identification

### Threat Hunting

- IOC Extraction
- Timeline Reconstruction
- Behavioral Analysis

### Detection Engineering

- Sigma Rule Development
- Detection Recommendations
- ATT&CK Mapping

### Documentation

- Incident Reporting
- Technical Writing
- Investigation Workflow

---

## Attack Flow
