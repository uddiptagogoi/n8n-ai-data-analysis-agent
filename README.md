# 🤖 AI Data Analysis Agent with n8n

An AI-powered data analysis agent built with **n8n, OpenRouter and Google Sheets**.

The idea behind this project was simple: instead of manually going through a spreadsheet every time I want to answer a business question, I wanted to build an agent that could understand the question, work with the data, and return the result in plain English.

## What does it do?

The agent allows users to ask questions about data using natural language.

For example:

* "What is the total revenue?"
* "Which product has the highest sales?"
* "Show me the best-performing category."
* "What are the main trends in the data?"
* "Compare sales across different regions."

The workflow uses **n8n** to connect the different components, **Google Sheets** as the data source, and **OpenRouter** to handle the AI reasoning.

## How it works

```text
User Question
      ↓
     n8n
      ↓
OpenRouter / LLM
      ↓
Understand the user's question
      ↓
Google Sheets
      ↓
Read and process the data
      ↓
LLM interprets the result
      ↓
Natural-language response
```

The goal is to make data analysis feel more like having a conversation with your dataset instead of manually searching through rows and columns.

## 🛠️ Tech Stack

* **n8n** – Workflow automation and agent orchestration
* **OpenRouter** – Access to LLMs for understanding and reasoning
* **Google Sheets** – Data source
* **AI Agent / LLM** – Natural-language data analysis
* **JSON** – Workflow configuration

## 🔍 Why I built this

I built this project to explore how AI agents can be used for practical data analysis tasks.

As a data analyst, I often work with spreadsheets and spend time cleaning data, finding patterns, calculating KPIs and answering business questions. This project explores how some of those repetitive interactions can be automated using an AI-powered workflow.

It also gave me hands-on experience connecting an LLM with external tools and making the model work with real data rather than just generating text.

## ✨ Key Features

* Ask data questions using natural language
* Connect directly to Google Sheets
* Use an LLM to understand user questions
* Automate the data-analysis workflow with n8n
* Return results in an easy-to-understand format
* Reduce the need for manually searching through spreadsheets

## 📁 Project Structure

```text
n8n-ai-data-analysis-agent/
│
├── workflow/
│   └── ai-data-analysis-agent.json
│
├── screenshots/
│   ├── n8n-workflow.png
│   ├── google-sheet.png
│   └── analysis-output.png
│
├── sample-data/
│   └── sample-data.csv
│
└── README.md
```

> The exact folder structure may vary depending on how the n8n workflow and supporting files are stored in the repository.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/uddiptagogoi/n8n-ai-data-analysis-agent.git
cd n8n-ai-data-analysis-agent
```

### 2. Set up n8n

You can run n8n locally or use an n8n instance.

Import the workflow JSON file into your n8n environment.

### 3. Configure OpenRouter

Create an OpenRouter API key and configure it in n8n.

Do **not** commit API keys or other credentials to GitHub.

### 4. Connect Google Sheets

Connect your Google account in n8n and provide access to the spreadsheet that contains your dataset.

### 5. Run the workflow

Send a question to the agent and let the workflow process the request.

For example:

```text
Which region generated the highest revenue?
```

The agent uses the available spreadsheet data and returns the analysis as a natural-language response.

## 💡 Example Use Cases

This type of workflow could be useful for:

* Sales analysis
* Marketing performance analysis
* Customer data analysis
* KPI reporting
* Spreadsheet-based business reporting
* Quick exploratory data analysis
* Automated business insights

## 🔐 Security

API keys, Google credentials and other sensitive information should **never** be stored directly in the repository.

Use n8n's credential management system or environment variables to manage secrets.

## 🔮 Future Improvements

Some improvements I would like to explore:

* Add support for CSV and Excel files
* Add automatic data cleaning
* Generate charts and visualizations automatically
* Add more advanced statistical analysis
* Add memory for follow-up questions
* Add support for multiple data sources
* Build a simple web interface for interacting with the agent

## 👨‍💻 About

This project is part of my work exploring **Data Analytics, AI Agents and workflow automation**.

I'm particularly interested in how AI can be combined with traditional data tools to make everyday analysis faster and easier.

**GitHub:** https://github.com/uddiptagogoi

---

⭐ If you find the project interesting, feel free to explore the workflow and share your feedback.
