# Project 04 - Network Discovery with Nmap

## Objective

Perform a defensive network discovery using Nmap to identify active hosts, open ports, and running services on a local Windows network.

---

## Environment

- Operating System: Windows 11 Pro
- Tool: Nmap 7.99
- Scan Target: Local Network
- Target Host: 192.168.58.210

---

## Commands Executed

```powershell
ipconfig

nmap -sn 192.168.58.0/24

nmap 192.168.58.210

nmap -sV 192.168.58.210
```

---

## Findings

### Host Discovery

Two active hosts were identified.

| IP Address | Description |
|------------|-------------|
| 192.168.58.134 | Default Gateway |
| 192.168.58.210 | Windows 11 Workstation |

---

### Open Ports

| Port | Service | Version |
|------|---------|----------|
| 135 | MSRPC | Microsoft Windows RPC |
| 139 | NetBIOS-SSN | Microsoft Windows NetBIOS |
| 445 | Microsoft-DS | SMB |

---

## Analysis

The workstation exposes only standard Windows networking services.

No unexpected ports or unauthorized services were identified.

The scan results indicate a normal Windows 11 workstation within a trusted network.

---

## Recommendations

- Disable unnecessary network services.
- Restrict SMB access using Windows Firewall.
- Keep Windows updated.
- Perform periodic network scans.

---

## Skills Demonstrated

- Nmap
- Network Discovery
- Host Enumeration
- Port Scanning
- Service Detection
- Security Assessment
- Documentation