# 🛡️ Brute Force Detection Lab with Elastic Stack

A mini SOC (Security Operations Center) lab setup by a student to simulate brute force attack detection using the Elastic Stack (Elasticsearch + Kibana). This project includes uploading custom logs, detecting failed login attempts, generating alerts, managing cases, and building dashboards.

---

## 🚀 What’s Included

### 📄 Simulated Logs  
Custom-generated `.ndjson` logs using ChatGPT simulating failed SSH login attempts: (here's an example)
```json
{"@timestamp":"2025-08-01T12:00:00Z","event":{"action":"authentication_failed"},"user":{"name":"admin"},"source":{"ip":"192.168.1.10"}}
{"@timestamp":"2025-08-01T12:00:05Z","event":{"action":"authentication_failed"},"user":{"name":"root"},"source":{"ip":"192.168.1.10"}}
{"@timestamp":"2025-08-01T12:00:10Z","event":{"action":"authentication_failed"},"user":{"name":"guest"},"source":{"ip":"192.168.1.10"}}
```
## ⚙️ Detection Rule

- Custom rule created in Elastic Security  
- Triggers on `event.action: "authentication_failed"`  
- Generates alerts based on frequency of failed logins  

---

## 📬 Alerts & 📁 Case Management

- Alerts created from detection rule  
- Alerts escalated into cases with investigation notes  
- Cases reviewed and closed after analysis  

---

## 📊 Dashboards

Visualizations built in Kibana using Lens:

- 🔢 Count of Failed Logins Over Time  
- 👤 Most Targeted Usernames  
- 🌍 Source IP Distribution  

---

## 💡 Key Skills Practiced

- Log ingestion via Kibana  
- Writing KQL-based detection rules  
- Managing alerts & cases in Elastic Security  
- Creating Kibana dashboards  
- Simulating real-world SOC workflows  
