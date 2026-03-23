# 📊 AI-Powered Operational Workflow Auditor
### 🌟 Overview
A scheduled oversight system that acts as a "Watchman" for other automations. It periodically aggregates logs from active incident resolvers and uses AI to identify patterns that traditional rule-based systems might miss.

### 🛠️ Technical Architecture
- **Scheduled Aggregation:** Runs on a Cron-job trigger to pull 24-hour log snapshots from a central database.

- **Anomaly Synthesis:** Feeds aggregated logs into a Gemini agent with a specific "Auditor" persona to find logical inconsistencies.

- **Escalation Protocol:** Routes critical findings to a dedicated Slack channel while archiving "Healthy" reports to a database.

### ⚙️ Tech stack
- **Primary Engine:** n8n (self hosted)
- **AI/LLM:** Google gemini / OpenAI
- **Data processing:** Log Aggregation Logic
- **Communication:** Slack Webhooks
