# Project 03 - Wireshark Network Traffic Analysis

## Objective

Capture and analyze live network traffic using Wireshark to identify protocols, network communication, and determine whether any suspicious activity is present.

---

## Environment

- Operating System: Windows 11 Pro
- Tool: Wireshark
- Capture Format: PCAPNG

---

## Traffic Generated

The following activities were performed during the capture:

- Browsed to Google
- Browsed to GitHub
- Browsed to Wikipedia
- Executed `ping google.com`
- Executed `nslookup google.com`

---

## Protocols Observed

- DNS
- TCP
- TLS 1.2

---

## Investigation Findings

### DNS

Observed DNS queries for:

- google.com
- assets.msn.com

DNS responses were successfully received.

### TLS

Encrypted HTTPS traffic was observed between the local system and external servers.

### TCP

TCP sessions completed normally using acknowledgements and keep-alive packets.

No abnormal retransmissions or resets were observed.

---

## Analysis

The captured traffic represents legitimate user web browsing and system background activity.

DNS resolution completed successfully.

Encrypted HTTPS communication occurred as expected.

No Indicators of Compromise (IOCs) were identified.

---

## Conclusion

The captured traffic is consistent with normal Windows workstation activity.

No suspicious communications or malicious network behavior were detected.

---

## Skills Demonstrated

- Packet Capture
- Wireshark Analysis
- DNS Analysis
- TCP Analysis
- TLS Analysis
- Network Traffic Investigation
- Incident Documentation