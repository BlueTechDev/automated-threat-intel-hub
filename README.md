# 🛡️ Automated Threat Intelligence Hub

A no-code/low-code threat detection pipeline built using [n8n](https://n8n.io), [VirusTotal](https://www.virustotal.com/), and [Google Sheets](https://workspace.google.com/products/sheets/). This project enriches suspicious IPs from log files, identifies repeat offenders, and sends real-time alerts — all without the need for a full SIEM solution.

---

## 📊 Live Demo

**🔗 Threat Dashboard (Google Sheets - View Only)**  
[https://docs.google.com/spreadsheets/d/1hlN1f3yuDyc5j7VDzsQImhwNjSc_kqs-QU-OAMdnXEw/edit?usp=sharing]

---

## ⚙️ Features

- 🧠 **IP Enrichment via VirusTotal & GeoIP**
- 📄 **Log Parsing**: Extracts IPs from raw firewall/syslog inputs
- 📈 **Repeat Offender Tracking**: Updates count of IPs seen multiple times
- 🗂️ **Structured Google Sheet Storage**: Real-time logging of scan results
- 🚨 **Slack Alerts**: Get notified when known malicious IPs are detected
- 📌 **Fully Automated**: Hands-free operation using n8n Cloud

---

## 🧩 Stack & Integrations

| Tool         | Purpose                         |
|--------------|----------------------------------|
| [n8n](https://n8n.io) | Workflow automation engine |
| [VirusTotal API](https://www.virustotal.com/gui/home/search) | IP reputation lookups |
| [GeoJS](https://www.geojs.io/) | Geolocation API |
| Google Sheets | Dashboard + data storage |
| Slack | Real-time alerting |

---

## 📸 Screenshots

| n8n Workflow Overview | Google Sheets Threat Log |
|------------------------|--------------------------|
| ![n8n workflow](./screenshots/n8n-workflow.png) | ![Threat log](./screenshots/google-sheet.png) |

---

## 🧠 Why It Matters

Most small teams or IT pros don’t have access to enterprise SIEMs. This project creates a lightweight threat intel pipeline that enriches and tracks suspicious IPs — perfect for:
- Solo analysts
- SMBs with limited budgets
- Security automation portfolios

---

## 🛠️ How It Works

1. **Logs parsed via n8n**
2. **IP addresses extracted**
3. **Each IP enriched via VirusTotal + GeoIP**
4. **Results logged in Google Sheets**
5. **If malicious → alert sent via Slack**
6. **Repeat IPs flagged and tracked**

---

## 📂 Folder Structure


---

## 🚀 Getting Started

Coming soon: deployment instructions & n8n workflow imports.

> For now, check out the [live dashboard](https://docs.google.com/spreadsheets/d/1hlN1f3yuDyc5j7VDzsQImhwNjSc_kqs-QU-OAMdnXEw/edit?usp=sharing) and browse the workflow overview in `/screenshots`.

---

## 👤 Author

**Jonah Kroll**  
Security Automations Engineer • IT & Cybersecurity  
[LinkedIn Profile](https://www.linkedin.com/in/jonahkroll-cybersecurity)

---

## 📄 License

MIT License
