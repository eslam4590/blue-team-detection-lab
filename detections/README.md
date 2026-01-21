# Detection Engineering

## Overview
This folder contains detection queries designed to identify common attack techniques observed in enterprise environments.

Each detection focuses on behavior-based indicators rather than single events.

---

## Detection Philosophy
- Prefer behavioral patterns over signatures
- Reduce false positives by using thresholds
- Align detections with real-world SOC use cases

---

## Included Detections
| Detection | Description |
|--------|------------|
| Brute Force Login | Multiple failed authentication attempts |
| Privilege Escalation | Unauthorized elevation of privileges |
| Suspicious PowerShell | Encoded or hidden PowerShell execution |
| Impossible Travel | Logins from distant locations in short time |

---

## Notes
- Queries are written in Kibana Query Language (KQL)
- Detections are designed for lab and demonstration purposes
