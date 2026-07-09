# Project 01 – Windows Successful Logon Investigation

## Objective

Analyze Windows Security Event ID 4624 to understand successful authentication events and identify whether the activity appears legitimate.

## Environment

- Operating System: Windows 11 Pro
- Tool: Windows Event Viewer

## Event Details

| Field | Value |
|-------|-------|
| Event ID | 4624 |
| Event Name | Successful Logon |
| Logon Type | 5 (Service Logon) |
| Audit Result | Success |
| Account | MORANTS |

## Analysis

A successful logon event (4624) was observed in the Windows Security log.

The authentication used **Logon Type 5**, indicating that a Windows service authenticated successfully rather than an interactive user.

No evidence of suspicious behavior was observed during this investigation.

## Conclusion

This event represents expected Windows service activity.

No indicators of compromise (IOCs) were identified.

## Skills Demonstrated

- Windows Event Log Analysis
- Authentication Investigation
- Event Viewer
- Security Monitoring