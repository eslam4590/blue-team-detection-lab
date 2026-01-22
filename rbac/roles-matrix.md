# Roles & Permissions Matrix

This matrix defines role-based access control (RBAC) for the Blue Team Detection Lab.

---

## Roles

| Role | Primary Responsibility |
|---|---|
| SOC Analyst | Monitor alerts and investigate security events |
| Detection Engineer | Build and maintain detection logic |
| SOC Manager | Oversight, reporting, and operational visibility |
| Platform Administrator | Manage SIEM infrastructure and security |

---

## Access Matrix

| Resource / Capability | SOC Analyst | Detection Engineer | SOC Manager | Admin |
|---|---|---|---|---|
| View Security Logs | ✅ | ✅ | ✅ | ✅ |
| Search & Filter Logs | ✅ | ✅ | ✅ | ✅ |
| View Dashboards | ✅ | ✅ | ✅ | ✅ |
| Create / Edit Dashboards | ❌ | ❌ | ✅ | ✅ |
| Create / Edit Detections | ❌ | ✅ | ❌ | ✅ |
| Enable / Disable Detections | ❌ | ✅ | ❌ | ✅ |
| Export Reports | ❌ | ❌ | ✅ | ✅ |
| Modify Log Pipelines | ❌ | ❌ | ❌ | ✅ |
| Manage Users & Roles | ❌ | ❌ | ❌ | ✅ |

---

## RBAC Principles Applied

- Least Privilege
- Separation of Duties
- Read vs Write Access Control

---

## Notes

- This RBAC model is tool-agnostic
- Designed to reflect real SOC environments
- Applicable to Elastic, Sentinel, and Splunk
