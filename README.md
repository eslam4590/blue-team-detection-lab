# 🛡️ Blue Team Detection Lab – ELK Stack

## 📌 Overview

This repository contains a **hands-on Blue Team / SOC Detection Lab** built using the **ELK Stack (Elasticsearch, Logstash, Kibana)**.

The project simulates real-world **Security Operations Center (SOC)** activities such as log ingestion, parsing, detection engineering, anomaly-focused visualization, and access control.

This lab is designed to demonstrate **practical Blue Team skills** rather than theoretical knowledge.

---

## 🎯 Project Goals

* Centralize security logs in a SIEM platform
* Parse and normalize logs early in the pipeline
* Build reusable detection queries for common attack techniques
* Visualize anomalous behavior instead of raw log volume
* Implement role-based access control (RBAC)
* Audit log visibility to avoid blind spots

---

## 🧰 Tools & Technologies

* Elasticsearch
* Logstash
* Kibana
* Filebeat / Winlogbeat
* Sysmon (Windows)
* Docker

---

## 🧱 High-Level Architecture

The lab follows a standard SIEM pipeline:

```
Log Sources  →  Beats  →  Logstash  →  Elasticsearch  →  Kibana
                       (Parsing)        (Storage)        (Detection & Dashboards)
```

---

## 🔍 Detection Coverage (Planned)

* Brute force authentication attempts
* Privilege escalation events
* Suspicious PowerShell execution
* Abnormal login behavior (time-based / geo-based)

---

## 📊 Visualization Strategy

Dashboards are designed to:

* Highlight suspicious behavior
* Reduce analyst noise
* Support fast investigation

---

## 🔐 Security & Access Control

The lab includes:

* Role separation between SOC Analysts and Admins
* Limited access to sensitive indices

---

## 📁 Repository Structure

> Each folder represents a specific SOC responsibility.

```
(Structure will be built step by step)
```

---

## 👤 Author

**Eslam Badawy**

---

## 🚀 Status

🚧 Lab under active development. Components will be added incrementally.

---

> This repository reflects real-world Blue Team best practices and SOC workflows.

