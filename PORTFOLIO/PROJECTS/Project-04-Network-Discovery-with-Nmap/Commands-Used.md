# Commands Used

## Display Network Configuration

```powershell
ipconfig
```

---

## Host Discovery

```powershell
nmap -sn 192.168.58.0/24
```

---

## Port Scan

```powershell
nmap 192.168.58.210
```

---

## Service Detection

```powershell
nmap -sV 192.168.58.210
```

---

## Save Scan Results

```powershell
nmap -sV 192.168.58.210 > nmap-scan.txt
```