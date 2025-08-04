# 🛡️ Brute Force Detection Lab with Elastic Stack

A mini SOC (Security Operations Center) lab setup on my home lab to simulate brute force attack detection using the Elastic Stack (Elasticsearch + Kibana). This project includes uploading custom logs, detecting failed login attempts, generating alerts, managing cases, and building dashboards.

---

## 📁 Project Folder Structure

This repository contains the following directories to organize different components of the mini SOC lab:

| Folder Name        | Description |
|--------------------|-------------|
| `logs/`            | Contains the `.ndjson` log file uploaded to Elastic, simulating brute force authentication failures. |
| `detection_rules/` | Contains the detection rule configured to catch repeated failed login attempts. |
| `alerts/`          | Screenshots of the Security → Alerts page showing the triggered alerts. |
| `case/`            | Evidence of case management — includes a closed case with remarks after investigating the alerts. |
| `dashboard/`       | Exported dashboard and screenshots showing Kibana Lens visualizations created for case analysis and it's presentation. |
| `dataview/`        | Shows the Data View (field names and data types) generated after uploading the log data. |

---

## ⚙️ Detection Rule

- Custom rule created in Elastic Security  
- Triggers when logs depicting a brute force attack are detected
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

- Manual ingestion of logs given an ndjson file
- Writing KQL-based detection rules  
- Managing alerts & cases in Elastic Security  
- Creating Kibana dashboards  
- Simulating real-world SOC workflows  
