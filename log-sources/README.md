# Log Sources

## Overview
This folder documents the security log sources used in this lab.
The selected logs represent common data sources monitored in real-world SOC environments.

---

## Windows Logs
Windows endpoints generate high-value security events.

### Source
- Sysmon
- Windows Security Event Logs

### Use Cases
- Process creation monitoring
- Privilege escalation detection
- Suspicious command execution

> Sysmon configuration is provided as a reference and is not intended for production use.

---

## Linux Logs
Linux systems provide critical authentication and system activity logs.

### Source
- /var/log/auth.log

### Use Cases
- SSH brute force attempts
- Unauthorized access
- Privilege escalation events

---

## Notes
- Sample logs are anonymized.
- No sensitive or real production data is included.

