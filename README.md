🚀 Automated LinkedIn Post Generator using GenAI + n8n

This project is an AI-powered automation system that turns any article link into a professional LinkedIn post — completely automatically.

By combining n8n, OpenAI models, Google Sheets, and the LinkedIn API, this workflow reads an article URL, summarizes it, rewrites it for LinkedIn, and publishes it — all without human intervention.

This project was built for the GenAI Buildathon to showcase a real-world, fully functional generative AI automation pipeline.

⭐ Project Overview

Professionals want to be consistent on LinkedIn, but:

Writing summaries is slow

Writing LinkedIn-style posts is harder

Posting regularly is difficult

This system solves all of these by automating the entire workflow:

🧠 How the System Works
✔ Step 1 — Add an Article Link (Google Sheets Trigger)

Whenever a new link is added to Google Sheets, n8n automatically starts the workflow.

✔ Step 2 — AI Summarizes the Article

Using OpenAI GPT models, the system generates a clean summary of the article.

Prompt Used:

Summarize this article: {{$json.ArticleLinks}}

✔ Step 3 — AI Converts Summary into LinkedIn Post

A LinkedIn-style post is generated using a second LLM in the chain.

Prompt Example:

Rewrite this summary into a professional LinkedIn post.
Add 4–5 relevant hashtags and a call to action.

✔ Step 4 — LinkedIn API Publishes Automatically

The final output is sent to LinkedIn and posted on your profile immediately.

Completely hands-free.

🏗 Architecture Diagram (Text)
Google Sheets (Article Link)
        │
        ▼
n8n Google Sheets Trigger Node
        │
        ▼
OpenAI Summarizer (LLM)
        │
        ▼
LLM Chain (LinkedIn-style Formatter)
        │
        ▼
LinkedIn Post Node (API)

🛠 Tech Stack
Component	Technology
Workflow Automation	n8n
Language Model	OpenAI GPT Models
Input Source	Google Sheets
Content Generation	Prompt Engineering + LLM Chain
Publishing	LinkedIn API
Logic	JSON mapping in n8n
📁 Repository Structure
📦 genai-linkedin-auto-post
 │
 ├── README.md                 # Full documentation
 ├── /screenshots              # Your 5 uploaded images
 │     ├── llm_architecture_overview.jpg
 │     ├── google_sheets_trigger_workflow.jpg
 │     ├── summarizer_prompt_output.jpg
 │     ├── llm_chain_node.jpg
 │     └── auto_post_to_linkedin.jpg
 │
 ├── workflow.json (Optional: Exported n8n workflow)
 └── prompts.md (Optional: Store your prompts)

📈 Features

🔗 Reads article links automatically from Google Sheets

🤖 Extracts the key insights using LLM summarization

✍️ Reformats the content as a LinkedIn-style post

🔥 Publishes directly via LinkedIn API

🌀 Fully automated workflow

⚙️ Supports continuous posting

🔄 Extendable for multi-platform publishing

🧪 Testing the Workflow
✔ Add the link to Google Sheets

→ Workflow triggers.

✔ Check Summarizer Output

→ Summary appears in execution logs.

✔ Check LLM Chain Output

→ LinkedIn-ready post appears.

✔ Final Step

→ Post is automatically published to your LinkedIn account.

🎯 Use Cases

Daily LinkedIn learning posts

Startup founders posting articles

Personal branding automation

Newsletter → LinkedIn autoposting

AI-powered content creation for teams

🌟 Why This Project Stands Out

This project shows:

✔ Real GenAI application — not just a model demo
✔ Automation skills (n8n workflows)
✔ API integration (LinkedIn)
✔ Zero-code + AI combined effectively
✔ End-to-end working solution with screenshots


🔮 Future Enhancements

Add support for Twitter/X, Instagram, Threads

Add auto-hashtag generator

Use embeddings to detect article themes

Add confidence score for AI outputs

Add Notion/Database to track posting history

📄 License

This project is open for educational, portfolio, and GenAI buildathon demonstration purposes.
