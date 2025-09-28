# 🚀 n8n Automation Gallery

A collection of **ready-to-use n8n workflows** for real-world business automation and process optimization.  
Each workflow comes with a JSON file you can import into n8n.  
⚠️ Note: These are **templates** – they require customization to work in your environment.  

---

## 📑 Workflows

- [📄 Invoice Processing & Slack Alerts](#-invoice-processing--slack-alerts)
- [👥 CRM Lead Auto-Enrichment](#-crm-lead-auto-enrichment)
- [📅 Social Media Auto-Scheduler](#-social-media-auto-scheduler)
- [💾 Weekly Data Backup Automation](#-weekly-data-backup-automation)
- [💬 Customer Feedback Sentiment Analyzer](#-customer-feedback-sentiment-analyzer)
- [📊 Invoice-to-Cashflow Automation](#-invoice-to-cashflow-automation)
- [🤝 Sponsor Inquiry Automation](#-Sponsor-Inquiry-Automation)

---

## 📄 Invoice Processing & Slack Alerts
**Description:** Automates invoice management by extracting invoice data from emails, saving to Google Sheets, and sending real-time Slack alerts.  
**Business Value:** Saves ~10 hours/month by removing manual entry.

**Workflow file:** [invoice-automation.json](./invoice-automation.json)

### 🚀 How to Use
1. Import the JSON into n8n.  
2. Connect your own email inbox (IMAP).  
3. Add Google Sheets & Slack credentials.  
4. Activate the workflow and test.  

⚠️ Note: Parsing logic is specific and may not match your invoices.  
👉 For custom setup, reach out to me.

---

## 👥 CRM Lead Auto-Enrichment
**Description:** Captures new leads from a form/email, enriches them with public data APIs, stores in Google Sheets/CRM, and alerts sales via Slack.  
**Business Value:** Gives sales teams richer lead data instantly.

**Workflow file:** [crm-lead-enrichment.json](./crm-lead-enrichment.json)

### 🚀 How to Use
1. Import into n8n.  
2. Connect your form/email + Google Sheets.  
3. Add your API key for enrichment (e.g. Clearbit).  
4. Test with a sample lead.  

⚠️ Note: API setup is required and not included in this template.  
👉 Contact me for full integration.

---

## 📅 Social Media Auto-Scheduler
**Description:** Pulls upcoming posts from Google Sheets, formats them, and auto-schedules posts to Twitter/LinkedIn.  
**Business Value:** Saves ~5 hours/week for marketing teams and ensures consistent posting.

**Workflow file:** [social-media-scheduler.json](./social-media-scheduler.json)

### 🚀 How to Use
1. Import workflow JSON.  
2. Connect Google Sheets + social media accounts.  
3. Adjust posting format.  
4. Activate and watch posts go live.  

⚠️ Note: Requires correct API tokens for social platforms.  
👉 I can help with setup & compliance.

---

## 💾 Weekly Data Backup Automation
**Description:** Runs weekly to fetch files from Google Drive, compresses them, and uploads to AWS S3 (or another storage).  
**Business Value:** Prevents data loss with zero manual effort.

**Workflow file:** [data-backup-automation.json](./data-backup-automation.json)

### 🚀 How to Use
1. Import JSON file.  
2. Connect Google Drive + AWS S3.  
3. Adjust backup schedule.  

⚠️ Note: You must configure secure credentials for cloud storage.  
👉 Reach out for enterprise-grade setup.

---

## 💬 Customer Feedback Sentiment Analyzer
**Description:** Collects customer feedback from Google Forms, uses AI sentiment analysis, and stores results in Sheets with weekly Slack summaries.  
**Business Value:** Gives product teams instant insight into customer mood.

**Workflow file:** [customer-feedback-analyzer.json](./customer-feedback-analyzer.json)

### 🚀 How to Use
1. Import JSON into n8n.  
2. Connect Google Forms/Sheets.  
3. Add your AI provider credentials (e.g. OpenAI).  
4. Run a test with sample feedback.  

⚠️ Note: Sentiment analysis requires API setup.  
👉 I offer support to make it production-ready.

---

## 📊 Invoice-to-Cashflow Automation
**Description:** Advanced workflow that takes invoices from email, extracts details, stores them in Google Sheets, updates a financial dashboard, and generates cashflow projections.  
**Business Value:** Saves **~15 hours/month** and gives **real-time cashflow visibility** – something most businesses pay accountants for.

**Workflow file:** [invoice-to-cashflow.json](./invoice-to-cashflow.json)

### 🚀 How to Use
1. Import JSON into n8n.  
2. Connect your email inbox, Google Sheets, and dashboarding tool (Looker, Data Studio, etc).  
3. Adjust cashflow formulas to fit your business.  
4. Activate and test with a real invoice.  

⚠️ Note: Projection logic is **template only** – customization is required.  
👉 Contact me for a full financial-grade setup.


---

## 🤝 Sponsor Inquiry Automation
**Description:** Workflow that captures sponsorship inquiries via a form, extracts the budget value from text, decides whether to accept or decline based on a threshold, sends a personalized email, and logs the request in Google Sheets.  
**Business Value:** Saves time by automating sponsor request handling, ensures consistent communication, and keeps a centralized record of all inquiries.

**Workflow file:** [sponsor-inquiry.json](./sponsor-inquiry.json)

### 🚀 How to Use
1. Import JSON into n8n.  
2. Connect Gmail and Google Sheets credentials.  
3. Replace placeholder email text with your own templates.  
4. Activate and test with a form submission.  

⚠️ Note: Decline email contains placeholder wording — update before production use.  
👉 Extendable to send Slack/Discord notifications or push data into a CRM.  

---

## 👨‍💻 Author

**Zalan Lykos**  

📎 [LinkedIn](https://www.linkedin.com/in/zalanlykos) • [GitHub](https://github.com/ZalanLykos)
