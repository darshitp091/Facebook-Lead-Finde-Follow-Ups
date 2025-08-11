# 📋 Instant Lead Capture & AI Follow-up Automation (n8n + Facebook + Google Sheets + Gmail + OpenRouter)

This automation captures leads from **Facebook Lead Ads**, stores them in **Google Sheets**, generates a personalized follow-up email using **OpenRouter's DeepSeek:R1 model**, and sends the email via **Gmail** — all **automatically**.

---

## 🛠 Tools Used
- **n8n** – Workflow automation platform
- **Facebook Lead Ads** – Lead generation source
- **Google Sheets** – Lead tracking
- **OpenRouter (DeepSeek:R1)** – AI email writing
- **Gmail** – Follow-up delivery

---

## 📂 Files in This Repo
- `automation.json` → The n8n workflow export file  
- `README.md` → This setup and guidance document

---

## 📈 Workflow Overview
1. **Facebook Lead Ads Trigger** → Captures new leads in real time.
2. **Google Sheets Append Row** → Logs lead details in a spreadsheet.
3. **HTTP Request (OpenRouter)** → Sends lead data to AI to create a personalized email.
4. **Gmail Send Message** → Sends the AI-generated email to the lead instantly.

---

## 🔍 Work Guidance (What Each Step Does)

### 1️⃣ Facebook Lead Ads Trigger
> When a new lead submits a Facebook form, their Name, Email, and Service Interest are captured.

### 2️⃣ Append Row in Google Sheet
> Saves lead data into Google Sheets for record-keeping and later reference.

### 3️⃣ HTTP Request – OpenRouter (DeepSeek:R1)
> Uses AI to generate a friendly, personalized email for the captured lead.

### 4️⃣ Send a Message via Gmail
> Sends the AI-generated message directly to the lead’s email address.

---

## ⚙️ Setup Guidance (Step-by-Step)

### **1. Facebook Lead Ads Trigger**
1. Go to [Meta for Developers](https://developers.facebook.com/) → Create a Facebook App.
2. In n8n, add a Facebook Lead Ads Trigger node.
3. Create new credentials → Log into your Facebook account and authorize.
4. Select your Page and the specific Lead Form.
5. Click **Execute Node** to test if it fetches lead data.

---

### **2. Google Sheets – Append Row**
1. Create a new Google Sheet with columns:
