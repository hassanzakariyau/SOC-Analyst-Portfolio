Project 5 — SOC Investigation Dashboard with Splunk

Overview

This project involved building a SOC investigation dashboard in Splunk Enterprise to monitor, analyze, and visualize Windows security events. The dashboard provides visibility into authentication activity, privileged accounts, Windows Defender detections, remediation actions, and Windows Security, System, and Application event trends.

Objectives

- Monitor failed and successful logon activity.
- Analyze failed logins by user account and source IP.
- Monitor privileged account activity.
- Analyze authentication activity by logon type.
- Monitor Windows Defender threat detections and remediation actions.
- Analyze Windows Security, System, and Application events.
- Build a centralized SIEM dashboard for security monitoring and investigation.

Tools Used

- Splunk Enterprise
- Windows
- Windows Event Logs
- Windows Defender
- Splunk Search Processing Language (SPL)

Data Sources

- Windows Security logs
- Windows System logs
- Windows Application logs
- Windows Defender Operational logs

Dashboard Panels

Security Overview

- Total Security Events
- Failed Login Attempts
- Windows Defender Threat Detections
- Windows Defender Remediation Actions

Authentication Investigations

- Failed Login Attempts Over Time
- Failed Login Attempts by User Account
- Failed Login Attempts by Source IP
- Successful Logins by User Account

Account and Logon Analysis

- Privileged Account Activity
- Successful Logons by Logon Type
- Failed Logons by Logon Type

Event Analysis

- Top 10 Windows Security Events
- Windows Security Events Over Time
- Top 10 Windows System Events
- Top 10 Windows Application Events
- Top 10 Windows Defender Events

SPL Techniques

- "spath" for XML field extraction.
- "rex" for extracting usernames, source IP addresses, logon types, and other fields.
- "stats" for event aggregation.
- "timechart" for event timeline analysis.
- Filtering and sorting events by Event ID and frequency.

Security Event IDs Examined

Event ID| Description
4624| Successful logon
4625| Failed logon
4672| Special privileges assigned to a new logon
4688| Process creation

Skills Demonstrated

- SIEM dashboard development
- Splunk SPL
- Windows event log analysis
- Authentication monitoring
- Privileged account monitoring
- Endpoint security monitoring
- XML log extraction
- Security data visualization
- SOC investigation techniques

Limitations

This project was developed in a local Windows lab environment. Available event data depended on system activity, audit configuration, and log collection settings. Event records were analyzed within context, as individual event occurrences do not independently establish malicious activity.

Project Deliverables

- SOC Investigation Dashboard
- SPL Queries Reference
- Investigation Report
- Dashboard Evidence Screenshots

Conclusion

This project demonstrates the practical use of Splunk Enterprise for Windows security monitoring and investigation. It strengthened hands-on skills in SIEM dashboard development, log analysis, authentication monitoring, endpoint security monitoring, and SPL-based investigation workflows.
