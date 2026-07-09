# Project 02 - Windows Process Creation Investigation

## Objective

Investigate Windows Security Event ID 4688 to analyze a newly created process, determine its parent process, and assess whether the activity represents legitimate Windows behavior or a potential security threat.

---

## Environment

- Operating System: Windows 11 Pro
- Tool: Windows Event Viewer
- Log Name: Security

---

## Event Information

| Field | Value |
|-------|-------|
| Event ID | 4688 |
| Event Name | Process Creation |
| Audit Result | Success |
| Task Category | Process Creation |

---

## Investigation

A Windows Security Event ID 4688 was identified while monitoring the Security event log.

The event recorded the creation of a new Windows process.

The investigation focused on:

- Identifying the newly created process
- Determining the parent process
- Reviewing the security context
- Assessing whether the activity was expected

---

## Investigation Findings

| Item | Value |
|------|-------|
| New Process | `C:\Windows\System32\lsass.exe` |
| Parent Process | `C:\Windows\System32\wininit.exe` |
| Process ID | `0x21c` |
| Parent Process ID | `0x3a4` |
| Token Elevation | Default (1) |
| Integrity Level | System Mandatory Level |

---

## Analysis

The investigation identified the creation of **lsass.exe (Local Security Authority Subsystem Service)**.

The parent process was **wininit.exe**, which is responsible for starting essential Windows services during system startup.

The executable was launched from the legitimate Windows System32 directory.

No abnormal parent-child relationship was identified.

No suspicious command-line arguments were present.

No Indicators of Compromise (IOCs) were observed.

---

## Conclusion

This event represents expected Windows operating system behavior.

The creation of **lsass.exe** by **wininit.exe** is a normal part of the Windows boot process.

No malicious activity was identified.

---

## Skills Demonstrated

- Windows Event Log Analysis
- Event ID 4688 Investigation
- Process Analysis
- Parent-Child Process Analysis
- Windows Internals
- Incident Documentation
- Security Monitoring

---

## Project Files

- Incident Report
- Evidence
- Timeline
- Screenshots