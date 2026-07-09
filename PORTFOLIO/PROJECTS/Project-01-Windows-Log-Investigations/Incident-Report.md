# Incident Report

## Incident Information

**Project:** Windows Successful Logon Investigation

**Date of Investigation:** 8 July 2026

**Investigator:** Kelvin Boamah

**Severity:** Informational

**Status:** Closed

---

## Incident Summary

A Windows Security Event ID 4624 (Successful Logon) was identified during routine log analysis using Windows Event Viewer. The event was investigated to determine whether it represented legitimate system activity or a potential security concern.

---

## Objective

Analyze a successful Windows logon event and determine whether the authentication was expected or suspicious.

---

## Tools Used

- Windows 11 Pro
- Windows Event Viewer

---

## Evidence Collected

- Event ID: 4624
- Logon Type: 5 (Service Logon)
- Logon ID: 0x3E7
- Security ID: SYSTEM
- Audit Result: Success

Evidence Screenshot:

`Screenshots/event-4624-successful-logon.png`

---

## Investigation

The Windows Security log was filtered for Event ID 4624.

The selected event showed a successful authentication with Logon Type 5, indicating that a Windows service authenticated successfully rather than an interactive user.

The Security ID was SYSTEM, and the Logon ID (0x3E7) is commonly associated with the Local System account.

No unusual accounts, unauthorized logon types, or suspicious behavior were observed.

---

## Analysis

The investigation determined that this event represents normal Windows operating system activity.

No indicators of compromise (IOCs) were identified.

No evidence of unauthorized access or malicious authentication attempts was found.

---

## Impact Assessment

No impact to system confidentiality, integrity, or availability was identified.

---

## Recommendations

- Continue monitoring Windows Security logs.
- Investigate any unusual logon types such as Remote Desktop (Logon Type 10) if unexpected.
- Review Event ID 4625 (Failed Logon) events if they occur repeatedly.
- Correlate future logon events with Event IDs 4672 and 4688 to detect privileged activity and process execution.

---

## Conclusion

The analyzed Event ID 4624 represents a legitimate Windows service logon.

The event is consistent with normal operating system behavior, and no further action is required.

---

## Skills Demonstrated

- Windows Event Log Analysis
- Authentication Investigation
- Security Monitoring
- Event Correlation
- Incident Documentation