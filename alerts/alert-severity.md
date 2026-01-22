# Alert Severity Classification

This document defines how alert severity is assigned in the Blue Team Detection Lab.

Severity reflects the potential impact, confidence, and urgency of a security alert.

---

## Severity Levels

### Informational
- No immediate security risk
- Used for visibility and baselining
- Example:
  - Successful login
  - New device observed

---

### Low
- Suspicious but low confidence
- May indicate misconfiguration or user error
- Example:
  - Single failed login attempt
  - Rare but benign process execution

---

### Medium
- Confirmed suspicious activity
- Requires analyst review
- Example:
  - Multiple failed login attempts
  - Execution of known dual-use tools

---

### High
- Strong indication of malicious behavior
- Immediate investigation required
- Example:
  - Brute-force attack detected
  - Malware execution alert

---

### Critical
- Active compromise or high-impact threat
- Requires escalation to incident response
- Example:
  - Privilege escalation detected
  - Ransomware activity

---

## Severity Assignment Criteria

Severity is based on:

- Impact to systems or data
- Confidence of detection logic
- Scope of affected assets
- Presence of corroborating signals

---

## Severity Handling Guidelines

| Severity | Analyst Action |
|---|---|
| Informational | Monitor only |
| Low | Review if recurring |
| Medium | Investigate |
| High | Immediate response |
| Critical | Escalate to incident |

---

## Notes

- Severity is independent of detection complexity
- False positives are used to tune severity levels
