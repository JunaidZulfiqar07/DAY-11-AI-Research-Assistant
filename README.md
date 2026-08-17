# 🤖 AI Research Assistant

### Day 11 — 30 Days AI Automation Challenge

An AI-powered research assistant that automatically researches a user's question using the **Tavily Search API**, analyzes the collected information with AI, and generates a structured research report with key findings, insights, opportunities, challenges, conclusions, and source references.

🌐 **Live Demo:** https://junaidzulfiqar07.github.io/AI-RESEARCH-ASSISTANT/

📅 **Live Demo Available Until:** August 24, 2026

---

## 📌 Project Overview

Researching a topic manually often requires visiting multiple websites, collecting information, comparing sources, and organizing the findings.

The **AI Research Assistant** automates this entire process.

The user simply enters a research question. The system generates focused search queries, searches the web using the **Tavily Search API**, collects relevant information, analyzes the results using AI, and presents the final research report through a clean and responsive web interface.

This project was built as **Day 11 of my 30 Days AI Automation Challenge**.

---

## ✨ Features

* 🔎 Research any topic using a simple search interface
* 🧠 AI-powered research planning
* 🌐 Automated web research
* 🔍 Multiple focused search queries
* 🤖 AI-powered research analysis
* 📝 Automatic research report generation
* 📋 Executive summary
* 🔎 Key findings
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
   AI Research Planner
          ↓
    Generate 3 Queries
          ↓
   Tavily Search API
          ↓
   Collect Web Results
          ↓
   AI Research Analyst
          ↓
    Structure Report
          ↓
    Google Sheets
          ↓
   Respond to Webhook
          ↓
     Research Report
```

---

## 🧩 n8n Workflow

The backend automation is built using **n8n**.

### Workflow Components

### 1. Webhook

Receives the research question from the frontend.

Example:

```json
{
  "question": "What are the latest applications of AI in healthcare?"
}
```

### 2. Edit Fields

Extracts and prepares the user's research question for processing.

### 3. AI Research Planner

Analyzes the research question and generates **three focused search queries** covering different aspects of the topic.

### 4. Code Node

Processes the generated queries and converts them into separate items for web searching.

### 5. Tavily Search API

Searches the web for relevant and recent information based on the generated queries.

### 6. Research Results Processing

Collects and organizes the search results returned by Tavily.

### 7. AI Research Analyst

Analyzes the collected web information and generates a structured research report.

### 8. Code Node

Formats the AI Research Analyst output into a clean JSON structure.

### 9. Google Sheets

Stores the completed research requests and generated reports for future reference.

### 10. Respond to Webhook

Sends the final structured research report back to the frontend.

---

## 🧠 AI Research Planner

The Research Planner converts one research question into multiple focused search queries.

### Example

**Research Question:**

```text
What are the latest applications of AI in healthcare?
```

**Generated Search Queries:**

```text
1. Latest applications of AI in healthcare
2. Recent developments and use cases of AI in healthcare
3. Challenges and future trends of AI in healthcare
```

This approach allows the system to gather information from multiple perspectives instead of relying on a single search query.

---

## 🌐 Tavily Search API

The project uses the **Tavily Search API** for automated web research.

Tavily provides the workflow with relevant web results that are then passed to the AI Research Analyst.

The search process includes:

* Multiple search queries
* Relevant web pages
* Search result titles
* Source URLs
* Extracted content
* Recent information when available

The collected information is then analyzed by the AI model.

---

## 🤖 AI Research Analyst

The AI Research Analyst processes the collected web research and generates:

```text
Executive Summary
Key Findings
Important Insights
Opportunities & Benefits
Challenges & Limitations
Conclusion
Sources
```

### Research Rules

The analyst is instructed to:

* Use information from the provided research results
* Avoid inventing facts
* Avoid creating fake sources
* Compare relevant information
* Remove unnecessary duplication
* Generate clear and professional results
* Return structured JSON
* Include source titles and URLs

---

## 📊 Research History

Completed research requests can be stored in **Google Sheets**.

### Stored Information

| Field             | Description                |
| ----------------- | -------------------------- |
| Date              | Research date and time     |
| Research Question | User's original question   |
| Executive Summary | AI-generated summary       |
| Key Findings      | Main research findings     |
| Insights          | Important insights         |
| Opportunities     | Benefits and opportunities |
| Challenges        | Limitations and challenges |
| Conclusion        | Final conclusion           |
| Sources           | Research source URLs       |

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

* **Tavily Search API**

### Data Storage

* Google Sheets

### Deployment

* GitHub
* GitHub Pages

---

## 📂 Project Structure

```text
DAY-11-AI-Research-Assistant/
│
├── index.html
├── README.md
└── LICENSE
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/JunaidZulfiqar07/DAY-11-AI-Research-Assistant.git
```

### 2. Open the Project

```bash
cd DAY-11-AI-Research-Assistant
```

### 3. Configure the n8n Webhook

Open `index.html` and configure your n8n production webhook:

```javascript
const WEBHOOK_URL =
  "YOUR_N8N_PRODUCTION_WEBHOOK";
```

### 4. Configure the Backend

The n8n workflow requires:

* n8n
* AI model/API
* Tavily Search API
* Google Sheets credentials

### 5. Run the Frontend

Open `index.html` in your browser or deploy the project using GitHub Pages.

---

## 🌐 Live Demo

🚀 **Try the AI Research Assistant:**

https://junaidzulfiqar07.github.io/AI-RESEARCH-ASSISTANT/

📅 **Live Demo Available Until: August 24, 2026**

---

## 💡 Example Research Questions

Try questions such as:

```text
What are the latest applications of AI in healthcare?

How is artificial intelligence changing education?

What are the major cybersecurity challenges in 2026?

What are the applications of robotics in manufacturing?

How is AI transforming software development?

What are the latest trends in renewable energy?

How is AI being used in financial services?
```

---

## 🔐 Security Note

The frontend communicates with the production n8n webhook.

**Never expose API keys or sensitive credentials in frontend JavaScript.**

Tavily and other API credentials should be securely configured on the backend/n8n side using appropriate credentials or secure environment configuration.

---

## 🔮 Future Improvements

Planned improvements include:

* 📄 Export research reports as PDF
* 📥 Download research reports
* 💬 Follow-up research questions
* 🧠 Conversation-based research
* 📚 Source credibility scoring
* 🔍 Advanced search filters
* 📊 Research analytics dashboard
* 🗂️ Research history interface
* 🌙 Light/Dark theme options
* 🎙️ Voice-based research queries
* 📈 Automatic comparison between sources

---

## 🎯 Learning Outcomes

Through this project, I practiced:

* Building AI-powered automation workflows
* Working with n8n Webhooks
* Integrating external APIs
* Using the Tavily Search API
* Designing effective AI prompts
* Generating structured AI output
* Processing JSON with JavaScript
* Connecting frontend applications with n8n
* Automating Google Sheets data storage
* Deploying web applications with GitHub Pages
* Building production-oriented AI automation systems

---

## 🏆 30 Days AI Automation Challenge

This project is part of my:

# **30 Days AI Automation Challenge 🚀**

### Day 11 — AI Research Assistant

The goal of this challenge is to build and deploy a new AI/automation project every day while continuously improving my skills in:

* Artificial Intelligence
* Automation
* n8n
* APIs
* AI Agents
* Web Development
* Prompt Engineering
* Real-world Problem Solving

---

## 👨‍💻 Author

### Junaid Zulfiqar

**Computer Engineering Student**
**UET Taxila**

Interested in building projects around:

* 🤖 Artificial Intelligence
* ⚡ Automation
* 🔗 n8n
* 🧠 AI Agents
* 🌐 Web Development
* 🔌 APIs
* 💻 Computer Engineering

---

## ⭐ Support

If you found this project useful, consider giving the repository a ⭐ **Star**.

Your support motivates me to continue building and sharing projects throughout the **30 Days AI Automation Challenge**.

---

## 📜 License

This project is available under the **MIT License**.

---

### © 2026 Junaid Zulfiqar — All Rights Reserved
