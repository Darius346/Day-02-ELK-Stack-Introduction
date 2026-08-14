# Day-02-ELK-Stack-Introduction
30‑Day MyDFIR SOC Analyst Challenge ELK Stack Introduction

# 📌 Objective
Gain a foundational understanding of the ELK Stack (Elasticsearch, Logstash, Kibana) and how it supports log ingestion, parsing, searching, visualization, and SOC operations.

# 🧠 Skills Learned
- Understanding how Elasticsearch stores and queries log data
- Understanding Logstash pipelines, filtering, and parsing
- Understanding Kibana for dashboards, visualizations, and log exploration
- Understanding Beats and Elastic Agent for telemetry collection
- Mapping ELK components to traditional SIEM architecture (indexer, forwarder, search head)
- Recognizing ELK’s benefits: centralized logging, flexibility, scalability, ecosystem integrations

# 🛠️ Tools & Components
- Elasticsearch – Log storage + ES|QL querying
- Logstash – Pipelines, filtering, parsing, transformations
- Kibana – Dashboards, Discover tab, visualizations, ML features
- Elastic Beats
  - Filebeat (logs)
  - Metricbeat (metrics)
  - Packetbeat (network)
  - Winlogbeat (Windows event logs)
  - Auditbeat (audit data)
  - Heartbeat (uptime monitoring)
- Elastic Agent – Unified telemetry collector
- REST APIs & JSON – Programmatic interaction with Elasticsearch

# 📝 Lab Notes
1. Elasticsearch Overview
- Stores logs from Windows, firewalls, syslogs, etc.
- Supports ES|QL (Elastic Search Query Language)
- Can be queried via REST API or Kibana’s web console
2. Logstash Overview
- Acts as the pipeline engine
- Collects telemetry from Beats or Elastic Agent
- Filters logs based on criteria (e.g., only ingest Event ID 4624)
- Parses fields (e.g., mapping “SRC IP” → “source.ip”)
- Allows custom parsers for logs without built‑in field mappings
3. Beats & Elastic Agent
- Beats = specialized collectors
- Elastic Agent = unified collector for all telemetry
- Used to forward logs into Logstash or directly into Elasticsearch
4. Kibana Overview
- Web interface for searching, visualizing, and analyzing logs
- Features include:
  - Discover tab (ES|QL queries)
  - Lens (drag‑and‑drop visualizations)
  - Machine learning (anomaly detection)
  - Maps (geospatial data)
  - Alerts & dashboards
5. ELK Stack Benefits
- Centralized logging
- Flexible ingestion
- Executive‑friendly dashboards
- Scalable architecture
- Large ecosystem + community support
