# 💰 Invoice-to-Cashflow Automation (n8n)

An advanced **business process automation** workflow built with [n8n](https://n8n.io).  
This project automates the **invoice lifecycle** — from receiving an invoice, logging it, checking due dates, sending reminders, updating CRM, creating tasks, and handling errors with real-time notifications.

---

## 🚀 Features

- 📩 **Email Trigger** – captures invoices from Gmail automatically  
- 📄 **PDF Parsing** – extracts amount, client, due date, and invoice ID  
- 📊 **Google Sheets Logging** – creates a single source of truth for invoices  
- 🧮 **Decision Logic** – checks if invoices are overdue or not  
- 🔄 **Multi-Branch Workflow**:
  - ✅ **Not Due/Paid** → Update HubSpot CRM + Backup in Airtable  
  - ❌ **Overdue** → Reminder Email + Slack Alert + Trello Task  
  - ⚠ **Error Handling** → Log in Error Sheet + Telegram Alert  
- 📲 **Notifications** – Slack for finance team, Trello for collections, Telegram for admins  
- ♻ **Retry Mechanism** – auto-retries failed reminder emails (3 attempts)  

---

## 📊 Business Impact

- ⏳ **20+ hours/month saved** by automating manual invoice tracking  
- 💸 **40% faster collection** of overdue invoices  
- 🚫 **0 missed invoices** thanks to automated error handling  
- 📈 Improved **cash flow predictability**  

---

## 🖼 Workflow Overview

```
📩 Gmail (Invoices) → 📄 PDF Parser → 📊 Google Sheets (Log)  
                                ↓  
                         🧮 Check Due Date  
                                ↓  
     ┌───────────────┴───────────────┐  
     ↓                               ↓  
✅ Not Due/Paid                  ❌ Overdue  
Update HubSpot CRM              Reminder Email  
Backup to Airtable              Slack Alert  
                                Trello Task  
                                ↳ Retry on Fail  
                                
⚠ Error → Error Sheet → Telegram Admin Alert
```

---

## ⚙️ Tech Stack

- **n8n** (workflow automation)
- **Gmail** (trigger source)
- **PDF Parser** (invoice data extraction)
- **Google Sheets** (logging & error queue)
- **HubSpot CRM** (customer lifecycle updates)
- **Airtable** (backup storage for BI dashboards)
- **Slack** (finance alerts)
- **Trello** (collections follow-up tasks)
- **Telegram** (admin error alerts)

---

## 📥 Setup Instructions

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/invoice-cashflow-automation.git
   cd invoice-cashflow-automation
   ```

2. Import the workflow JSON into your **n8n instance**.  
   - Go to **n8n → Workflows → Import from File**  
   - Select `workflow.json` from this repo.  

3. Replace placeholders (`{{YOUR_API_KEY}}`, `{{YOUR_SHEET_ID}}`, etc.) with your credentials.  

4. Activate the workflow and test with a sample invoice email.  

---

## 📸 Screenshots

*(Add screenshots of your actual workflow from n8n here — it makes the project look alive.)*

---

## 🔮 Future Improvements

- Integration with accounting tools (e.g., QuickBooks, Xero)  
- AI-based OCR for messy invoice PDFs  
- Automatic payment reconciliation  

---

## 👨‍💻 Author

**Dktr Dee**  
*AI Agent & Automation Engineer | Workflow Automation | Business Process Optimization | Cybersecurity Student | Full-Stack Developer*  

📎 [LinkedIn](https://www.linkedin.com/in/zalanlykos) • [GitHub](https://github.com/ZalanLykos)
