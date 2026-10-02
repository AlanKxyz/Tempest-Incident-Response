# Executive Summary

During the investigation a Windows workstation was identified as compromised following execution of a malicious Microsoft Word document.

The attack leveraged PowerShell to download and execute additional payloads, establish persistence, and communicate with attacker-controlled infrastructure.

Analysis of Sysmon logs, Windows Event Logs, endpoint telemetry and captured network traffic enabled full reconstruction of the attack lifecycle.

## Impact Assessment

Severity: High

Affected Assets:
- Windows Workstation

Potential Risks:
- Credential Theft
- Remote Access
- Data Exfiltration
- Further Lateral Movement

## Key Findings

- Initial access achieved through malicious Office document
- PowerShell used for payload execution
- Persistence successfully established
- External command-and-control communication observed
- Indicators of Compromise identified and documented

## Analyst Conclusion

The attack demonstrates a common phishing-to-malware chain frequently observed in enterprise environments and highlights the importance of PowerShell monitoring, Office child process detection, and endpoint telemetry collection.
