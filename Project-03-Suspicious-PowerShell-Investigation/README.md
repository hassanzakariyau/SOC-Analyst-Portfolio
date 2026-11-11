Project 3: Suspicious PowerShell Activity Investigation

Overview

This project demonstrates the detection and investigation of suspicious PowerShell execution using Windows process creation logs and Splunk Enterprise.

Objectives

- Identify PowerShell process executions.
- Examine PowerShell command-line arguments.
- Detect encoded PowerShell execution.
- Review process creation information.
- Build and validate a Splunk detection alert.
- Investigate suspicious activity and determine an appropriate analyst verdict.

Environment

- Windows endpoint
- Splunk Enterprise
- Windows Security Event ID 4688
- PowerShell

Investigation Highlights

- Identified PowerShell process execution activity.
- Reviewed command-line arguments and PowerShell execution patterns.
- Investigated encoded PowerShell execution.
- Decoded a controlled Base64 payload.
- Created a detection for encoded PowerShell execution.
- Validated the scheduled Splunk alert.

Detection

Encoded PowerShell execution was detected using Windows Event ID 4688 and the "-EncodedCommand" argument.

Alert Validation

A controlled encoded PowerShell command successfully triggered the scheduled Splunk alert.

Incident Verdict

Benign controlled simulation.

The decoded payload was "Write-Output note". No malicious behavior was identified in the simulated payload.

Response

No containment or remediation was required. Detection and alert functionality were successfully validated.

Evidence

Screenshots documenting the investigation, detection, and alert validation are available in the Evidence folder.

Skills Demonstrated

- Windows process investigation
- PowerShell command-line analysis
- Windows event log analysis
- Splunk SPL
- Detection engineering
- Alert validation
- Incident triage
- False-positive assessment
