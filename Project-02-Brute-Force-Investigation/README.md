Project 2: Brute-Force Attack Investigation and Incident Response

Overview

This project demonstrates controlled Windows authentication failures, brute-force detection, Splunk alerting, and evidence-based incident investigation.

Environment

- Windows
- Splunk Enterprise
- Windows Security Event Logs
- PowerShell

Detection

- Event ID 4625 – Failed logon
- Event ID 4624 – Successful logon review
- Event ID 4672 – Privileged logon
- Event ID 4688 – Process creation
- Splunk threshold detection – 5 failures within 5 minutes

Investigation Findings

- Five failed logons against FakeUser
- Source address: ::1 (IPv6 loopback)
- No successful FakeUser logon observed
- FakeUser does not exist as a local account
- No process creation evidence referencing FakeUser found
- Splunk alert successfully triggered

Incident Response

Authentication activity was investigated, successful access was checked, privileged logons and process creation were reviewed, and containment was assessed based on evidence.

Recommendations

- Monitor repeated authentication failures
- Review successful logons after failed attempts
- Configure account lockout policies
- Investigate suspicious accounts and source addresses
- Maintain evidence and investigation records

Project Files

- Evidence: screenshots of investigation and alert results
- Reports: investigation report
- Splunk-Queries: detection and investigation SPL
  
