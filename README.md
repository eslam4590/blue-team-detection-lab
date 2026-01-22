# Blue Team Detection Lab (Elastic Stack)

A hands-on Blue Team detection lab designed to simulate real-world SOC workflows,
from log ingestion to alerting and incident response.

This project demonstrates practical experience in detection engineering,
alert triage, visualization, and security operations governance.

---

## 🎯 Project Objectives

- Build a realistic SOC detection environment
- Simulate real Linux and Windows log sources
- Create meaningful detections and alerts
- Visualize security events using dashboards
- Apply RBAC and incident response best practices

---

## 🧱 Lab Architecture

The lab is built using the Elastic Stack and simulates a small SOC environment.

**High-level flow:**

Logs → Logstash → Elasticsearch → Detections → Alerts → Incidents → Dashboards

📁 See detailed architecture:
- `architecture/README.md`
- `architecture/architecture-diagram.png`

---

## 📥 Log Sources

Realistic sample logs are used to simulate attacker behavior.

### Linux
- SSH authentication logs
- Brute-force attempts
- Privilege escalation via sudo

📄 `log-sources/linux/auth.log`

### Windows
- Process creation
- Network connections
- Persistence via registry

📄 `log-sources/windows/sysmon-config.xml`

---

## 🔄 Log Processing

Logstash pipelines are used to parse and normalize logs before indexing.

📁 `logstash/`

Key features:
- Grok parsing
- Field normalization
- Timestamp alignment

---

## 🛡️ Detections

Detection rules identify suspicious or malicious activity.

Examples:
- SSH brute-force attacks
- Suspicious PowerShell execution
- Registry-based persistence
- Reverse shell indicators

📁 `detections/`

---

## 🔔 Alerts

Alerts are generated when detections match malicious behavior.

Alert handling includes:
- Severity classification
- Analyst triage
- Escalation to incidents

📁 `alerts/`
- `README.md`
- `alert-severity.md`
- `sample-alerts.md`

---

## 📊 Dashboards

Dashboards provide visibility into:
- Authentication activity
- Detection trends
- Alert volume
- Suspicious behavior

📁 `dashboards/`

Screenshots:
- `dashboard-ssh.png`
- `dashboard-sysmon.png`

---

## 🚨 Incidents & Response

Alerts may be escalated into incidents following defined playbooks.

Included playbooks:
- SSH Brute Force
- Malware Detection
- Privilege Escalation

📁 `incidents/`

---

## 🔐 Role-Based Access Control (RBAC)

RBAC is implemented to reflect real SOC environments.

Roles include:
- SOC Analyst
- Detection Engineer
- SOC Manager
- Platform Administrator

📁 `rbac/`
- `README.md`
- `roles-matrix.md`

---

## 🧠 Skills Demonstrated

- SIEM architecture (Elastic Stack)
- Log parsing and normalization
- Detection engineering
- Alert triage and prioritization
- Incident response workflows
- Security dashboards
- RBAC and SOC governance

---

## 📌 Use Cases

- SOC Analyst training
- Detection engineering practice
- Blue Team portfolio project
- Interview demonstration lab

---

## 🚀 Future Enhancements

- Threat intelligence enrichment
- SOAR playbook automation
- MITRE ATT&CK mapping
- Cloud log sources (AWS / Azure)

---

## 📄 License

This project is for educational and demonstration purposes only.
