# AI-Automated Strategy Recommendation System

## 📌 Project Overview

This project is an AI-powered automation workflow built using **n8n**. It collects client business requirements through a Typeform, validates the input, generates a customized automation strategy using an AI model (Gemini), and sends the result to the client via email.

The project demonstrates practical knowledge of:

- Workflow automation (n8n)
- AI integration
- Conditional logic
- Error handling
- Cloud deployment understanding

---

## 🔗 Live Typeform (For Testing)

Test the workflow by filling the Typeform below:

👉 **Typeform Link:**\
[https://example.typeform.com/to/automation-strategy](https://example.typeform.com/to/automation-strategy)



---

## 🧪 Sample Input

```
Client Name: ABC Retail
Industry: E-commerce
Business Goal: Automate client onboarding
Target Audience: Small online sellers
Budget Level: 5k – 10k
Timeline: 1–2 months
Email: test@example.com
Service Required: AI-Driven Automation Strategy (Jugaad)
```

---

## ▶️ How to Run This Project on Your Own System

### Option 1: Run Locally Using Docker 

```bash
docker run -it --rm \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
```

Then open in browser:

```
http://localhost:5678
```

Steps:

1. Import `AI Automated Strategy Recommendation System.json`
2. Import `Error.json`
3. Configure credentials (Typeform, Gemini, Gmail)
4. Activate both workflows

---

### Option 2: Run on n8n Cloud

1. Create an account at [https://n8n.io](https://n8n.io)
2. Import the workflow JSON files
3. Configure credentials
4. Activate workflows

---

## 🔐 Credentials Setup (Required)

Credentials are not included in this repository for security reasons.

### Typeform

- Create a Typeform account
- Generate an API token
- Add credentials in n8n → Typeform Trigger

Docs: [https://developer.typeform.com/](https://developer.typeform.com/)

### Gemini AI

- Create an API key from Google AI Studio
- Add Gemini credentials in n8n

Docs: [https://ai.google.dev/](https://ai.google.dev/)

### Gmail

- Configure Gmail OAuth credentials in n8n
- Authorize your Google account

Docs: [https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.gmail/](https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.gmail/)

---

## ☁️ Cloud Deployment Note

For learning and demonstration purposes, this workflow was also deployed on **Render** using the official n8n Docker image.

This was done to demonstrate cloud deployment understanding. In production environments, **n8n Cloud** or an always-on VM (AWS / GCP / Oracle Cloud) would be preferred.

---

## 📁 Repository Contents

```
/workflows
  ├── AI Automated Strategy Recommendation System.json
  └── Error.json


```
