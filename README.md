# Deep-Research-using-Open-AI

![image](https://github.com/user-attachments/assets/240935ed-3947-4c77-888e-a17d6ad1a37f)
![image](https://github.com/user-attachments/assets/133ca6af-fd7b-4ae7-9773-fbd622f368bf)

# 🧠 Agentic AI Deep Research Assistant

A modular, end-to-end agent-based research automation system powered by LLMs. This assistant autonomously plans web searches, summarizes findings, writes detailed reports, and emails the result — all from a single user query.

## 📦 Features

- 🗺️ **Planner Agent**: Breaks the query into structured web searches with reasoning.
- 🔍 **Search Agent**: Performs web searches and summarizes results concisely.
- 📝 **Writer Agent**: Synthesizes findings into a well-formatted markdown report.
- 📧 **Email Agent**: Converts reports to HTML and sends via SendGrid.
- 🌐 **Gradio UI**: Clean interface to enter queries and track research progress.
- 🧵 **Trace Logging**: Generates OpenAI trace links for debugging and transparency.

---

## 🚀 Getting Started

### 1. Clone the repository


git clone https://github.com/your-username/agentic-ai-research.git
cd agentic-ai-research
2. Install dependencies

pip install -r requirements.txt
3. Configure environment variables
Create a .env file in the root directory:

env
Copy
Edit
OPENAI_API_KEY=your_openai_key
SENDGRID_API_KEY=your_sendgrid_key
4. Launch the app
bash
Copy
Edit
python deep_research.py
🧠 Agent Architecture
Agent Name	Purpose
PlannerAgent	Generates 5 web search terms based on the input query
SearchAgent	Performs search + summarization for each generated term
WriterAgent	Creates a detailed markdown report with outline and summary
EmailAgent	Formats the report in HTML and sends it via email

📂 Code Structure
File	Description
deep_research.py	Main UI and app launcher using Gradio
research_manager.py	Controls the full agentic workflow
planner_agent.py	Query decomposition into web search plan
search_agent.py	Executes searches and extracts summaries
writer_agent.py	Converts search findings into a full report
email_agent.py	Sends reports via SendGrid email service

💡 Example Query

What are the ethical concerns and regulatory frameworks around AI in healthcare?
You’ll receive a ~1000 word markdown report with:

A short summary

Full report content

Follow-up research questions

Delivered directly via email

🔐 Security Note
All API keys must be stored in the .env file. Do not commit your credentials.

🔧 Future Enhancements
 Allow user to specify recipient email

 Add PDF export support

 Save report history to a local or cloud database

👨‍💻 Author
Built by Anish Nehete
Inspired by Ed Donner
Check out his Agentic AI course :)
