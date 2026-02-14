# 🚀 Automated LinkedIn Post Generator using GenAI + n8n

This project is an AI-powered automation system that converts article links into professional LinkedIn posts automatically.

By combining **n8n**, **OpenAI models**, **Google Sheets**, and the **LinkedIn API**, the workflow reads an article URL, summarizes it, rewrites it for LinkedIn, and publishes it — completely hands-free.

Built for the **GenAI Buildathon**, this project demonstrates a real-world generative AI automation pipeline.

---

## ⭐ Project Overview

Professionals want to stay consistent on LinkedIn, but:

- Writing summaries takes time
- Converting articles into LinkedIn posts is difficult
- Posting regularly requires effort

This system automates the entire workflow.

---

## 🧠 How the System Works

### Step 1 — Google Sheets Trigger
A new article link is added to Google Sheets.

This automatically triggers the n8n workflow.

---

### Step 2 — AI Article Summarization
An OpenAI model generates a concise summary of the article.

Example prompt:

---

### Step 3 — LinkedIn Post Generation
The summary is rewritten into a professional LinkedIn post.

Example prompt:


---

### Step 4 — Auto Publishing to LinkedIn
The formatted post is published automatically using the LinkedIn API.

No manual posting required.

---

## 🏗 Architecture Diagram

Google Sheets (Article Link)
│
▼
n8n Google Sheets Trigger
│
▼
OpenAI Summarizer
│
▼
LLM Chain (LinkedIn Formatter)
│
▼
LinkedIn API Post


---

## 🛠 Tech Stack

| Component | Technology |
|----------|-----------|
| Workflow Automation | n8n |
| Language Model | OpenAI GPT |
| Input Source | Google Sheets |
| Content Generation | Prompt Engineering |
| Publishing | LinkedIn API |
| Data Mapping | JSON in n8n |

---

## 📁 Repository Structure

genai-linkedin-auto-post/
│
├── README.md
├── workflow.json
├── prompts.md
│
└── screenshots/
├── llm_architecture_overview.jpg
├── google_sheets_trigger_workflow.jpg
├── summarizer_prompt_output.jpg
├── llm_chain_node.jpg
└── auto_post_to_linkedin.jpg


---

## 📈 Features

- Reads article links automatically from Google Sheets
- Generates article summaries using LLMs
- Converts summaries into LinkedIn-style posts
- Publishes posts automatically
- Fully automated workflow
- Continuous posting support
- Extendable automation pipeline

---

## 🧪 Testing the Workflow

1. Add a link to Google Sheets
2. Workflow triggers automatically
3. Check summarizer output in n8n logs
4. Verify LinkedIn post generation
5. Confirm automatic LinkedIn posting

---

## 🎯 Use Cases

- Daily LinkedIn learning posts
- Startup founder content automation
- Personal branding automation
- Newsletter-to-LinkedIn conversion
- AI-powered content workflows

---

## 🌟 Why This Project Stands Out

This project demonstrates:

- Real GenAI application
- Automation workflow design
- API integration
- Prompt engineering
- End-to-end AI system implementation

Not just AI usage — **AI system building**.

---

## 🔮 Future Enhancements

- Multi-platform posting (Twitter/X, Instagram)
- Automatic hashtag generation
- Embedding-based article classification
- Post history tracking database
- Output confidence scoring
- Notion integration

---

## 📄 License

This project is intended for educational, portfolio, and GenAI buildathon demonstration purposes.

---

## Author
Dhanuja Anbalagan
