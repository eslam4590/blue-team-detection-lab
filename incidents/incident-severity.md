# Incident Severity Classification

This document defines how incident severity is assigned in the Blue Team Detection Lab.

Incident severity reflects business impact, scope, and urgency of response.

---

## Severity Levels

### Low
- Minimal security impact
- Limited to single user or system
- No data loss
- Example:
  - Misconfigured account permissions
  - Isolated policy violation

---

### Medium
- Confirmed malicious activity with limited spread
- No critical systems affected
- Example:
  - Malware blocked on endpoint
  - Suspicious lateral movement attempt

---

### High
- Active threat affecting multiple systems
- Potential data exposure
- Example:
  - Successful brute-force leading to account compromise
  - Unauthorized privilege escalation

---

### Critical
- Severe business impact
- Data breach or service disruption
- Example:
  - Ransomware outbreak
  - Domain-wide compromise

---

## Severity Assignment Criteria

Severity is determined by:

- Scope of affected assets
- Sensitivity of impacted data
- Persistence of attacker
- Ability to contain the threat

---

## Severity Response Expectations

| Severity | Response Time |
|---|---|
| Low | Business hours |
| Medium | Same day |
| High | Immediate |
| Critical | Immediate + Management Notification |

---

## Notes

- Incident severity may differ from alert severity
- Severity can be reclassified during investigation
