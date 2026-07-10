# Evidence

## Investigation Details

**Tool:** Nmap 7.99

**Operating System:** Windows 11 Pro

**Target Network:** 192.168.58.0/24

**Target Host:** 192.168.58.210

---

## Host Discovery

### Command

```powershell
nmap -sn 192.168.58.0/24
```

### Results

| IP Address | Description |
|------------|-------------|
| 192.168.58.134 | Default Gateway |
| 192.168.58.210 | Windows Workstation |

---

## Port Scan

### Command

```powershell
nmap 192.168.58.210
```

### Results

| Port | State | Service |
|------|-------|----------|
| 135 | Open | MSRPC |
| 139 | Open | NetBIOS Session Service |
| 445 | Open | Microsoft-DS (SMB) |

---

## Service Detection

### Command

```powershell
nmap -sV 192.168.58.210
```

### Service Information

| Port | Service | Version |
|------|---------|---------|
| 135 | MSRPC | Microsoft Windows RPC |
| 139 | NetBIOS Session Service | Microsoft Windows NetBIOS |
| 445 | Microsoft-DS | Windows SMB |

---

## Screenshots

- host-discovery.png
- port-scan.png
- service-detection.png

---

## Scan Results

- nmap-scan.txt

---

## Conclusion

The network scan identified expected Windows networking services.

No unauthorized hosts, suspicious ports, or Indicators of Compromise were observed.