# Incident Report

## Incident Information

Project: Wireshark Network Traffic Analysis

Severity: Informational

Status: Closed

---

## Incident Summary

A packet capture was performed using Wireshark to analyze live network traffic generated from normal user activity.

The investigation focused on identifying network protocols, destination hosts, and indicators of suspicious communication.

---

## Tools Used

- Wireshark

---

## Evidence Collected

- PCAPNG capture
- DNS traffic
- TLS traffic
- TCP sessions
- Packet screenshots

---

## Investigation

Network traffic was captured while visiting trusted websites and executing basic network commands.

Analysis identified successful DNS resolution, encrypted HTTPS communication, and normal TCP sessions.

---

## Analysis

Observed traffic included:

- DNS queries
- TLS encrypted sessions
- TCP acknowledgements
- Keep-Alive packets

Traffic matched expected workstation behavior.

No malicious communications were observed.

---

## Impact Assessment

No impact to confidentiality, integrity, or availability.

---

## Recommendations

Continue monitoring:

- Unknown domains
- Suspicious DNS requests
- Unexpected outbound connections
- Non-standard ports

---

## Conclusion

The network capture represents legitimate workstation activity.

No further action required.