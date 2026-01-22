# Brute Force Attack Incident Playbook

This playbook defines the response steps for a detected brute-force
authentication attack.

---

## Incident Overview

- **Category:** Authentication Attack
- **Typical Severity:** High
- **Source Alerts:**
  - Multiple failed login attempts
  - Suspicious authentication patterns

---

## Objectives

- Identify the source of the attack
- Prevent account compromise
- Protect authentication services
- Preserve evidence

---

## Detection Triggers

- Repeated failed login attempts from a single IP
- Multiple accounts targeted from one source
- Failed logins followed by successful authentication

---

## Investigation Steps

1. Identify affected accounts
2. Review authentication logs
3. Check for successful logins after failures
4. Analyze source IP reputation
5. Verify geolocation anomalies

---

## Containment Actions

- Block malicious IP addresses
- Temporarily lock targeted accounts
- Enforce MFA if not already enabled

---

## Eradication Actions

- Reset compromised account credentials
- Remove unauthorized access tokens
- Review authentication policies

---

## Recovery Actions

- Unlock accounts after verification
- Monitor login activity closely
- Restore normal access controls

---

## Post-Incident Actions

- Tune detection thresholds
- Document false positives
- Update alert severity if needed
- Conduct lessons learned

---

## Notes

- Brute-force attacks may precede lateral movement
- Correlate with other alerts for broader context
