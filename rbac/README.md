# RBAC – Role-Based Access Control

## Overview

This folder documents how Role-Based Access Control (RBAC) is applied in this Blue Team Detection Lab.

RBAC ensures that users only have access to the data and actions required for their job role, which is critical in SOC environments to reduce risk and prevent misuse.

---

## Why RBAC Matters in Blue Team Operations

In a real SOC:

* Not every analyst should see all logs
* Not every user should be able to modify detections or dashboards
* Administrative actions must be tightly controlled

RBAC helps to:

* Enforce least privilege
* Protect sensitive security data
* Prevent accidental or malicious changes
* Meet compliance and audit requirements

---

## RBAC Scope in This Lab

RBAC is demonstrated conceptually using common SOC roles mapped to Elasticsearch / Kibana permissions.

The lab focuses on **access design**, not identity management.

---

## Defined Roles

The following roles are used in this lab:

* SOC Analyst (Tier 1 / Tier 2)
* Detection Engineer
* SOC Manager
* Platform Administrator

Each role has different permissions over:

* Logs
* Detections
* Dashboards
* Configuration

Detailed permissions are documented in `roles-matrix.md`.

---

## Example Mapping to Kibana

| Role               | Kibana Access                   |
| ------------------ | ------------------------------- |
| SOC Analyst        | Read-only dashboards and logs   |
| Detection Engineer | Create and edit detections      |
| SOC Manager        | View all dashboards and reports |
| Admin              | Full platform access            |

---

## Security Principles Applied

* Least Privilege
* Separation of Duties
* Read vs Write access separation

---

## Notes

This RBAC model reflects real-world SOC environments and can be adapted to:

* Elastic Stack
* Microsoft Sentinel
* Splunk

The goal is to demonstrate security thinking, not tool-specific syntax.
