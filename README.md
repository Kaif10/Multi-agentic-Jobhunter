# Multi-agentic-Jobhunter

AI Job Hunt Agents 🤖💼
This project is a multi-agent AI system built in a Python notebook that automates key parts of the job application process. It uses a team of specialized AI agents to write tailored cover letters, craft professional networking messages, and provide strategic reviews of your CV against a specific job description.

Note: You can create a quick screen recording of the app and convert it to a GIF using a free online tool like ezgif.com.

✨ Features
This system is composed of three specialist agents, an orchestrator, and a reviewer, all accessible through a simple Gradio web UI.

Cover Letter Agent: Creates a compelling, professional cover letter tailored to the job description and your CV. It analyzes the role's key requirements and maps them to your strongest qualifications, outputting a downloadable PDF.

Networking Agent: Generates two robust, ready-to-send outreach messages: a concise LinkedIn DM and a slightly more formal cold email. The agent is designed with a multi-layered safety net (guided retries and high-quality fallbacks) to ensure a usable output every time.

CV Review Agent: Acts as an expert recruiter, providing a strategic analysis of your CV's alignment with the role. It returns a structured JSON object with a verdict (Strong Fit, Good Fit, etc.), a confidence score, keyword optimization tips, and prioritized, actionable edits.

🚀 How It Works
The system uses a modular, multi-agent architecture where each component has a specific responsibility. This makes the system robust, maintainable, and easy to extend.

A simple diagram showing the UI, Orchestrator, and the three specialist agents.

UI (Gradio): The user uploads their CV, provides a job URL, and selects a task.

Orchestrator: The central "project manager." It scrapes the necessary data and routes the request to the appropriate agent.

Specialist Agents: The selected agent performs its task (e.g., writing a cover letter).

Review Coordinator: Manages the feedback loop, allowing the user to request revisions until they are satisfied with the output.

🛠️ Getting Started
To run this project, you'll need Python and an OpenAI API key.

1. Clone the Repository
git clone [https://github.com/your-username/job-hunt-agents.git](https://github.com/your-username/job-hunt-agents.git)
cd job-hunt-agents

2. Install Dependencies
The project uses a few key Python libraries. You can install them using pip:

pip install openai beautifulsoup4 requests reportlab pdfminer.six gradio

3. Configure Your API Key
When you run the notebook for the first time, it will prompt you to enter your OpenAI API key.

Enter your OpenAI API key: [your_key_here]

Alternatively, you can set it as an environment variable.

4. Run the Notebook
Open the main.ipynb file in Jupyter Notebook or JupyterLab and run the cells sequentially. The Gradio UI will launch at the end, providing a public URL you can use to interact with the application.

💡 Future Ideas
This project is a great
