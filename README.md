# Automated Threat Intel Hub

> **Centralized Threat Intelligence Aggregator with Enrichment & Alerting**

## Overview

This project automates the collection and enrichment of threat intelligence data from public sources using `n8n` for orchestration and `Python` for enrichment. The enriched data can then be used for alerting, firewall updates, or SOC dashboards.

### Key Features
- Pulls from multiple threat intel feeds (AlienVault OTX, AbuseIPDB, etc.)
- Enriches IPs/domains via VirusTotal and/or Shodan
- Sends enriched alerts via Slack or Email
- Logs all data to Google Sheets or JSON
- Designed to run via `n8n` (importable workflow included)

---

## Use Cases
- Blue Team threat awareness dashboards
- Blocklist automation for firewalls
- Analyst enrichment on IOC sightings
- SOC alert automation pipeline

---

## Architecture

![Architecture Diagram](docs/architecture.png)

---

## Folder Structure

| Folder         | Description                                       |
|----------------|---------------------------------------------------|
| `src/`         | Python enrichment and helper scripts              |
| `n8n_workflows/`| JSON exports of n8n workflow(s)                   |
| `data/`        | Sample output and IOC logs                        |
| `docs/`        | Diagrams or architecture documentation            |
| `tests/`       | Unit tests                                        |

---

## Getting Started

### Requirements
- Python 3.10+
- n8n self-hosted (or desktop)
- API keys: VirusTotal, Shodan, Slack Webhook, Google Sheets

### Install Python Requirements

```bash
pip install -r requirements.txt
