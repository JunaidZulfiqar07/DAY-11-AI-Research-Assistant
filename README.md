# 🤖 AI Research Assistant

### Day 11 — 30 Days AI Automation Challenge

An AI-powered research assistant that automatically researches a user's question using web search, analyzes the collected information with AI, and generates a structured research report with key findings, insights, opportunities, challenges, conclusions, and sources.

🔴 **Live Demo:** https://junaidzulfiqar07.github.io/AI-RESEARCH-ASSISTANT/

📅 **Live Demo Available Until: August 24, 2026**

---

## 📌 Project Overview

Researching a topic manually often requires visiting multiple websites, collecting information, comparing sources, and organizing the findings.

The **AI Research Assistant** automates this process.

The user simply enters a research question. The system generates focused search queries, searches the web, collects relevant information, analyzes the results using AI, and presents the final research report through a clean web interface.

This project was built as **Day 11 of my 30 Days AI Automation Challenge**.

---

## ✨ Features

* 🔎 Research any topic using a simple search interface
* 🧠 AI-powered research planning
* 🌐 Automated web research
* 📊 Multiple focused search queries
* 🤖 AI-powered information analysis
* 📝 Automatic research report generation
* 📋 Executive summary
* 🔍 Key findings
* 💡 Important insights
* 🚀 Opportunities & benefits
* ⚠️ Challenges & limitations
* ✅ Conclusion
* 🔗 Source titles and URLs
* 📊 Research history stored in Google Sheets
* ⚡ n8n-powered automation
* 📱 Responsive web interface
* 🌐 GitHub Pages deployment

---

## 🔄 How It Works

```text
User enters research question
          ↓
       Webhook
          ↓
    Research Planner
          ↓
   Generate 3 Queries
          ↓
      Web Search
          ↓
   Collect Web Results
          ↓
    AI Research Analyst
          ↓
    Structure Research
          ↓
     Google Sheets
          ↓
    Research Report
          ↓
        User
```

---

## 🧩 n8n Workflow

The backend automation is built using **n8n**.

### Workflow Components

1. **Webhook**

   * Receives the research question from the frontend.

2. **Edit Fields**

   * Extracts and prepares the user's question.

3. **AI Research Planner**

   * Analyzes the research question.
   * Generates three focused web search queries.

4. **Code Node**

   * Converts the generated queries into separate items.

5. **Web Search**

   * Searches the web for relevant information.

6. **Research Results Processing**

   * Collects the information returned by the search API.

7. **AI Research Analyst**

   * Analyzes the collected research.
   * Generates a structured research report.

8. **Code Node**

   * Formats the AI output into a clean JSON structure.

9. **Google Sheets**

   * Stores research history and generated reports.

10. **Respond to Webhook**

    * Sends the final research report back to the frontend.

---

## 🧠 AI Research Planner

The Research Planner converts one research question into multiple focused search queries.

### Example

**Question:**

```text
What are the latest applications of AI in healthcare?
```

**Generated queries:**

```text
1. AI applications in healthcare 2026
2. Recent developments in AI healthcare
3. Challenges and future trends of AI in healthcare
```

This allows the system to collect information from different perspectives instead of relying on a single search query.

---

## 🤖 AI Research Analyst

After collecting web research, the AI Research Analyst processes the information and generates:

```text
Executive Summary
Key Findings
Important Insights
Opportunities & Benefits
Challenges & Limitations
Conclusion
Sources
```

The analyst is instructed to:

* Use information from the collected sources
* Avoid inventing facts
* Avoid creating fake sources
* Compare relevant information
* Produce clear and professional results
* Return structured JSON

---

## 📊 Research History

Every completed research request can be stored in Google Sheets.

### Stored Information

| Field             | Description                |
| ----------------- | -------------------------- |
| Date              | Research date and time     |
| Research Question | User's original question   |
| Executive Summary | AI-generated summary       |
| Key Findings      | Main findings              |
| Insights          | Important insights         |
| Opportunities     | Benefits and opportunities |
| Challenges        | Limitations and challenges |
| Conclusion        | Final conclusion           |
| Sources           | Research sources           |

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript
* Responsive Web Design

### Automation

* n8n
* Webhooks
* HTTP Requests
* JavaScript Code Nodes

### AI

* AI Research Planner
* AI Research Analyst
* LLM-based structured analysis

### Web Research

* Web Search API

### Data Storage

* Google Sheets

### Deployment

* GitHub
* GitHub Pages

---

## 📂 Project Structure

```text
AI-RESEARCH-ASSISTANT/
│
├── index.html
└── README.md
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/JunaidZulfiqar07/AI-RESEARCH-ASSISTANT.git
```

### 2. Open the Project

```bash
cd AI-RESEARCH-ASSISTANT
```

### 3. Configure the Webhook

Open `index.html` and configure the production n8n webhook:

```javascript
const WEBHOOK_URL =
  "YOUR_N8N_PRODUCTION_WEBHOOK";
```

### 4. Open the Website

You can open `index.html` directly in a browser or deploy it using GitHub Pages.

---

## 🌐 Live Demo

🚀 **Try the AI Research Assistant:**

https://junaidzulfiqar07.github.io/AI-RESEARCH-ASSISTANT/

---

## 💡 Example Research Questions

Try questions such as:

```text
What are the latest applications of AI in healthcare?

How is artificial intelligence changing education?

What are the major cybersecurity challenges in 2026?

What are the applications of robotics in manufacturing?

How is AI transforming software development?
```

---

## 🔐 Security Note

The frontend communicates with the production n8n webhook.

API keys and sensitive credentials should **never be exposed inside frontend JavaScript**.

Use n8n credentials or secure server-side configuration for API authentication.

---

## 🔮 Future Improvements

Planned improvements include:

* 📄 Export reports as PDF
* 📥 Download research reports
* 💬 Follow-up questions
* 🧠 Conversation-based research
* 📚 Source credibility scoring
* 🔍 Advanced search filters
* 📊 Research analytics dashboard
* 🗂️ Research history interface
* 🌙 Light/Dark theme options
* 🎙️ Voice-based research queries

---

## 🎯 Learning Outcomes

Through this project, I practiced:

* Building AI-powered automation workflows
* Working with n8n Webhooks
* Integrating web search APIs
* Designing AI prompts
* Generating structured AI output
* Processing JSON with JavaScript
* Connecting frontend applications with n8n
* Automating Google Sheets data storage
* Deploying web applications with GitHub Pages
* Building production-oriented AI automation systems

---

## 🏆 30 Days AI Automation Challenge

This project is part of my:

### **30 Days AI Automation Challenge 🚀**

**Day 11 — AI Research Assistant**

The goal of this challenge is to build and deploy a new AI/automation project every day while continuously improving my skills in AI, automation, APIs, n8n, web development, and real-world problem solving.

---

## 👨‍💻 Author

### Junaid Zulfiqar

**Computer Engineering Student**
UET Taxila

Building projects around:

* Artificial Intelligence
* Automation
* n8n
* AI Agents
* Web Development
* APIs
* Computer Engineering

---

## ⭐ Support

If you found this project useful, consider giving the repository a ⭐ **Star**.

It helps support the project and motivates me to continue the **30 Days AI Automation Challenge**.

---

### © 2026 Junaid Zulfiqar — All Rights Reserved
