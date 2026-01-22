# Sample Security Alerts

This document provides example alerts generated in the Blue Team Detection Lab.

Each alert demonstrates how detection logic translates into actionable
security events for SOC analysts.

---

## Alert 1 — Brute Force Login Attempt

- **Severity:** High
- **Category:** Authentication
- **Source:** Windows Security Logs
- **Detection Trigger:**
  - More than 5 failed login attempts within 5 minutes
- **Affected Asset:** Domain Controller
- **Analyst Action:**
  - Validate source IP
  - Check for successful login after failures
  - Escalate if persistence is observed

---

## Alert 2 — Suspicious PowerShell Execution

- **Severity:** Medium
- **Category:** Execution
- **Source:** Sysmon Event ID 1
- **Detection Trigger:**
  - PowerShell executed with encoded command
- **Affected Asset:** User Workstation
- **Analyst Action:**
  - Decode PowerShell command
  - Check parent process
  - Review user activity

---

## Alert 3 — Malware Signature Match

- **Severity:** Critical
- **Category:** Malware
- **Source:** Endpoint Security Logs
- **Detection Trigger:**
  - Hash match with known malware
- **Affected Asset:** Application Server
- **Analyst Action:**
  - Isolate affected host
  - Preserve forensic artifacts
  - Escalate to Incident Response

---

## Alert 4 — Privilege Escalation Attempt

- **Severity:** High
- **Category:** Privilege Abuse
- **Source:** Windows Security Event ID 4672
- **Detection Trigger:**
  - Special privileges assigned to a new logon
- **Affected Asset:** Domain Controller
- **Analyst Action:**
  - Validate user role
  - Review recent account activity
  - Escalate if unauthorized

---

## Notes

- Alerts may be correlated into incidents
- False positives are documented for tuning
- Alerts align with MITRE ATT&CK techniques
