# Evidence

## Evidence Source

- Tool: Windows Event Viewer
- Log Name: Security
- Event Source: Microsoft Windows Security Auditing

---

## Event Details

| Field | Value |
|-------|-------|
| Event ID | 4688 |
| Event Name | Process Creation |
| Audit Result | Success |
| New Process Name | `C:\Windows\System32\lsass.exe` |
| Creator Process Name | `C:\Windows\System32\wininit.exe` |
| New Process ID | `0x21c` |
| Creator Process ID | `0x3a4` |
| Token Elevation Type | Default (1) |
| Mandatory Label | System Mandatory Level |
| Creator Security ID | SYSTEM |
| Creator Logon ID | `0x3E7` |

---

## Screenshot

`Screenshots/event-4688-process-creation.png`

---

## Observations

- Windows recorded the creation of a new process.
- The process created was **lsass.exe**.
- The parent process was **wininit.exe**.
- The executable was launched from the legitimate Windows System32 directory.
- The process executed under the SYSTEM account.
- No suspicious process creation behavior was observed.