
# Logstash Configuration

## Purpose
This folder contains Logstash configurations responsible for parsing, normalizing, and enriching security logs before indexing them into Elasticsearch.

Early parsing ensures higher detection accuracy and cleaner dashboards.

---

## Responsibilities
- Parse raw logs using Grok patterns
- Extract structured fields (IP, user, action, process)
- Normalize data across multiple log sources

---

## Folder Structure
- pipelines/ : Logstash pipeline configurations
- grok-patterns/ : Custom Grok patterns used for parsing

---

## Design Notes
- Parsing is performed before indexing to reduce noise
- Only security-relevant fields are extracted
- Configuration is simplified for lab demonstration purposes
