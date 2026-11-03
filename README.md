# multi-agent-research-system
# 🔬 ResearchMind – Multi-Agent AI Research System

An AI-powered multi-agent research system that automates web research, content extraction, report generation, and quality evaluation using multiple specialized AI agents.

## 📌 Overview

ResearchMind is a multi-agent AI research application built with Python and LangChain.

Instead of manually searching multiple websites, reading articles, and preparing research reports, ResearchMind automates the entire workflow using specialized AI agents.

The system follows a four-stage research pipeline:

1. **Search Agent:** Searches the web for recent and relevant information using Tavily.
2. **Reader Agent:** Extracts useful information from selected web pages.
3. **Writer Agent:** Generates a structured research report using an OpenAI language model.
4. **Critic Agent:** Evaluates the generated report and provides a score, strengths, and improvement suggestions.

The application provides an interactive interface built with Streamlit.

## ✨ Features

* Automated web research.
* Multi-agent architecture.
* Real-time web search using Tavily.
* Web scraping and content extraction.
* AI-powered research report generation.
* Automated report evaluation and scoring.
* Interactive Streamlit dashboard.
* Downloadable research reports in Markdown format.
* Environment-based API key management.

## 🛠️ Technologies Used

| Technology    | Purpose                            |
| ------------- | ---------------------------------- |
| Python        | Core programming language          |
| LangChain     | Agent orchestration and LLM chains |
| OpenAI        | Language model for AI agents       |
| GPT-4o-mini   | AI model                           |
| Tavily        | Web search API                     |
| BeautifulSoup | Web scraping                       |
| Requests      | HTTP requests                      |
| Streamlit     | Interactive user interface         |
| Python-dotenv | Environment variable management    |

## 🏗️ System Architecture

The project follows a sequential multi-agent architecture.

**Research Workflow:**

User Input (Research Topic)
↓
Search Agent
↓
Reader Agent
↓
Writer Agent
↓
Critic Agent
↓
Final Research Report + Evaluation

### Agent Responsibilities

**1. Search Agent**

* Searches the internet for relevant information.
* Retrieves website titles, URLs, and content snippets.
* Uses Tavily Search API.

**2. Reader Agent**

* Selects relevant resources.
* Scrapes web pages.
* Extracts readable content using BeautifulSoup.

**3. Writer Agent**

* Processes collected research information.
* Generates a structured research report.
* Organizes findings into introduction, key findings, conclusion, and sources.

**4. Critic Agent**

* Reviews the generated report.
* Assigns a score out of 10.
* Identifies strengths and weaknesses.
* Suggests improvements.

## 📂 Project Structure

```text
Multi-agent-research-system/
│
├── app.py              # Streamlit application
├── agents.py           # AI agent and LLM configurations
├── pipeline.py         # Research pipeline execution
├── tools.py            # Web search and scraping tools
├── requirements.txt    # Python dependencies
├── .env                # API keys (not committed)
├── .gitignore          # Git ignored files
└── README.md           # Project documentation
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Navigate to the Project Directory

```bash
cd Multi-agent-research-system
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Configure API Keys

Create a `.env` file in the root directory.

Add your API keys:

```env
OPENAI_API_KEY=your_openai_api_key
TAVILY_API_KEY=your_tavily_api_key
```

**Important:** Never upload your actual API keys or `.env` file to GitHub.

### 6. Run the Application

To launch the Streamlit interface:

```bash
streamlit run app.py
```

The application will open in your browser.

## 🚀 Usage

1. Launch the application.
2. Enter a research topic.
3. Click the **Run Research Pipeline** button.
4. Let the Search Agent collect information.
5. Let the Reader Agent extract relevant content.
6. The Writer Agent generates the research report.
7. The Critic Agent evaluates the report.
8. View and download your final research report.

## 🔐 Environment Variables

| Variable       | Description                          |
| -------------- | ------------------------------------ |
| OPENAI_API_KEY | Authentication for OpenAI API        |
| TAVILY_API_KEY | Authentication for Tavily Search API |

## 🔮 Future Improvements

* Implement parallel agent execution.
* Add memory for previous research sessions.
* Integrate a vector database for long-term knowledge storage.
* Implement RAG (Retrieval-Augmented Generation).
* Add source credibility verification.
* Improve report evaluation with dedicated evaluation metrics.
* Add PDF export functionality.
* Introduce more specialized research agents.

## 🎯 Project Objective

The primary objective of ResearchMind is to demonstrate how multiple specialized AI agents can collaborate to automate complex research tasks.

The project explores the practical application of:

* Agentic AI
* Large Language Models (LLMs)
* Multi-Agent Systems
* LangChain
* Web Search Automation
* Web Scraping
* AI-powered Content Generation

## 👨‍💻 Author

**Himangshu**

Computer Applications Student | Python Developer | AI/ML Enthusiast

---

⭐ If you find this project interesting, consider giving the repository a star!

**Note:** This project requires valid OpenAI and Tavily API keys to run.
