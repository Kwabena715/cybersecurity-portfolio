# Incident Report

## Incident Information

**Project:** Network Discovery with Nmap

**Severity:** Informational

**Status:** Closed

---

## Executive Summary

A defensive network discovery assessment was performed using Nmap to identify active hosts, open ports, and running services on the local network.

The objective was to establish a baseline of network assets and identify any unexpected exposure.

---

## Scope

Target Network:

192.168.58.0/24

Target Host:

192.168.58.210

---

## Tools Used

- Nmap 7.99
- Windows PowerShell

---

## Investigation

Host discovery identified two active devices.

The Windows workstation was scanned for open TCP ports.

Service detection identified standard Microsoft Windows networking services.

---

## Findings

Open Ports

- TCP/135 – Microsoft RPC
- TCP/139 – NetBIOS Session Service
- TCP/445 – Microsoft-DS (SMB)

Host Discovery

- 192.168.58.134 (Default Gateway)
- 192.168.58.210 (Windows Workstation)

---

## Risk Assessment

No suspicious hosts were identified.

The open ports correspond to legitimate Windows networking services.

Although SMB is commonly targeted by attackers, no evidence of malicious activity was observed.

---

## Recommendations

- Disable unused services.
- Restrict SMB access.
- Continue routine network assessments.
- Keep operating system patches current.

---

## Conclusion

The network scan identified only expected devices and services.

No Indicators of Compromise (IOCs) were detected.

No further action required.