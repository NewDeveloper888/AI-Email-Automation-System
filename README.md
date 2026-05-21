# 📧 AI Email Automation System

> Built By Mahmoud Yasser

An AI-powered email automation workflow built using n8n, Google Gemini AI, Gmail API, and Telegram Bot.

This system automatically receives emails, analyzes their content using AI, classifies them into categories, generates smart responses, and alerts the team for high-priority emails.

---

# 🚀 Features

- 📥 Automatic Gmail email monitoring
- 🤖 AI-powered email classification
- 🧠 Smart intent detection using Google Gemini
- 🏷️ Automatic email labeling
- ✉️ AI-generated email replies
- 🚨 Telegram alerts for urgent emails
- 💰 Finance email detection
- 📢 Promotion email filtering
- ⚡ Priority escalation system
- 🔄 Fully automated n8n workflow

---

# 🏗️ Architecture

```text
Incoming Email
      ↓
Gmail Trigger
      ↓
AI Text Classifier
      ↓
Category Detection
      ↓
Route to Specialized Agent
      ↓
Generate AI Response
      ↓
Decision Engine
   ↙           ↘
Draft Reply    Telegram Alert
```

---

# 🧩 Workflow Modules

## 1. Watch & Classify

Responsible for:
- Monitoring Gmail inbox
- Extracting email content
- Sending content to AI classifier

### Components
- Gmail Trigger
- Text Classifier
- Google Gemini Chat Model

---

## 2. AI Agents

Each category has a dedicated AI Agent.

| Agent | Responsibility |
|---|---|
| Customer Agent | Customer support emails |
| Priority Agent | Urgent & critical emails |
| Promotion Agent | Marketing/promotional emails |
| Finance Agent | Billing & payment issues |

---

## 3. Notification System

Handles:
- Draft email creation
- Telegram escalation alerts

### Channels
- Gmail Drafts
- Telegram Bot

---

# 🧠 AI Classification Categories

| Category | Description |
|---|---|
| Support | Customer questions/issues |
| Priority | Urgent or critical emails |
| Promotions | Marketing emails |
| Finance | Payments, invoices, refunds |

---

# ⚙️ Tech Stack

| Technology | Usage |
|---|---|
| n8n | Workflow Automation |
| Google Gemini AI | AI Understanding |
| Gmail API | Email Integration |
| Telegram Bot API | Instant Notifications |
| AI Agents | Smart Response Generation |

---

# 📦 Installation

## 1. Clone Repository

```bash
git clone https://github.com/your-repo/email-ai-automation.git
```

---

## 2. Install n8n

```bash
npm install n8n -g
```

---

## 3. Start n8n

```bash
n8n start
```

---

## 4. Configure Credentials

Add the following credentials inside n8n:

- Gmail API Credentials
- Google Gemini API Key
- Telegram Bot Token

---

# 🔥 Example Workflow

## Scenario 1 — Support Email

### Input

```text
Need help resetting my password.
```

### AI Classification

```text
Support
```

### Action

- Add "support" label
- Generate reply draft

---

## Scenario 2 — Critical Finance Email

### Input

```text
Payment system is failing urgently.
```

### AI Classification

```text
Finance + Priority
```

### Action

- Create draft response
- Send Telegram alert

---

# 📲 Telegram Alert Example

```text
🚨 HIGH PRIORITY EMAIL

From: client@company.com
Category: Finance
Urgency: Critical
Issue: Payment system failure
```

---

# 📈 Future Improvements

- CRM Integration
- Slack Notifications
- WhatsApp Alerts
- Sentiment Analysis
- Multi-language Support
- Database Logging
- Auto-reply Approval System

---

# 👨‍💻 Author

## Mahmoud Yasser

AI Automation Engineer & n8n Workflow Developer

---

# 📄 License

MIT License
