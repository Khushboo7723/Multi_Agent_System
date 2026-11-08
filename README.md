Multi-Agent AI Research System

An Intelligent AI-Powered Research Automation System using LangChain, OpenAI, Tavily, and Python

Project Overview

The Multi-Agent AI Research System is an AI-powered research automation project that uses multiple specialized AI agents to perform research, gather information, extract detailed content from web pages, generate structured research reports, and evaluate the final output.

The system follows a multi-agent workflow where each agent performs a specific task, making the research process more organized, efficient, and automated.

Instead of manually searching multiple websites and preparing reports, this system automates the complete research workflow using Large Language Models (LLMs) and web search tools.

Project Objectives

- Automate the online research process using AI agents.
- Collect recent and relevant information from the web.
- Extract detailed content from selected web pages.
- Generate structured and professional research reports.
- Evaluate the generated reports using an AI critic.
- Demonstrate practical implementation of multi-agent AI workflows.

Key Features

- AI-Powered Web Search: Searches the web for relevant and reliable information using Tavily.
- Intelligent Content Extraction: Scrapes web pages and extracts readable text using BeautifulSoup.
- Multi-Agent Architecture: Uses specialized agents for searching and reading information.
- Automated Report Generation: Generates detailed research reports using an OpenAI language model.
- AI-Based Report Evaluation: A critic agent reviews the generated report and provides a score, strengths, and areas for improvement.
- Automated Workflow: Executes the complete research process through a single Python pipeline.

System Architecture

The project consists of four major stages:

1. Search Agent

- Searches the web for recent and relevant information.
- Uses the Tavily Search API.
- Collects website titles, URLs, and content snippets.

2. Reader Agent

- Identifies relevant URLs from search results.
- Scrapes selected web pages.
- Extracts detailed textual information using BeautifulSoup.

3. Writer Agent

- Combines search results and scraped content.
- Uses an OpenAI LLM to generate a structured research report.
- Organizes the report into introduction, key findings, conclusion, and sources.

4. Critic Agent

- Evaluates the generated research report.
- Provides a score out of 10.
- Identifies strengths and areas for improvement.
- Generates a final one-line verdict.

Project Workflow

       User Enters Research Topic
                  |
                  v
          Search Agent
                  |
                  v
         Tavily Web Search
                  |
                  v
           Reader Agent
                  |
                  v
        Web Page Scraping
                  |
                  v
           Writer Agent
                  |
                  v
       Research Report Generation
                  |
                  v
           Critic Agent
                  |
                  v
        Report Evaluation
                  |
                  v
          Final Output

Technologies & Tools Used

Technology| Purpose
Python| Core programming language
LangChain| Building AI agents and LLM chains
LangGraph| Agent execution and workflow orchestration through LangChain
OpenAI API| Language model integration
Tavily API| Web search functionality
BeautifulSoup| Web scraping and content extraction
Requests| Sending HTTP requests
Python-dotenv| Managing environment variables
Rich| Terminal output formatting

Project Structure

MultiAgentSystem/
│
├── agents.py          # AI agents and LLM chains
├── pipeline.py        # Main research workflow
├── tools.py           # Web search and scraping tools
├── requirements.txt   # Project dependencies
├── .env               # API keys (not uploaded)
├── .gitignore         # Excludes sensitive and temporary files
└── README.md          # Project documentation

Installation & Setup

Step 1: Clone the Repository

git clone https://github.com/Khushboo7723/MultiAgentSystem.git

Step 2: Navigate to the Project Directory

cd MultiAgentSystem

Step 3: Create a Virtual Environment

python -m venv .venv

Step 4: Activate the Virtual Environment

For Windows:

.venv\Scripts\activate

Step 5: Install Required Dependencies

pip install -r requirements.txt

Step 6: Configure Environment Variables

Create a ".env" file in the project root directory and add your API keys:

OPENAI_API_KEY=openai_api_key
TAVILY_API_KEY=tavily_api_key

How to Run the Project

After completing the installation and API configuration, execute the following command:

python pipeline.py

Enter your desired research topic when prompted:

Enter a research topic: Artificial Intelligence in Healthcare

The system will automatically:

1. Search for relevant information.
2. Extract detailed content from web pages.
3. Generate a structured research report.
4. Evaluate the report using the critic agent.
5. Display the final report and evaluation in the terminal.

Sample Report Structure

The generated research report follows this structure:

- Introduction
- Key Findings
- Conclusion
- Sources

The critic agent provides:

- Score out of 10
- Strengths
- Areas to Improve
- One-line Verdict

API Requirements

To run this project, you need:

- OpenAI API Key: For accessing the language model.
- Tavily API Key: For web search functionality.

API keys should be stored securely in the ".env" file.

Future Improvements

- Integrate multiple specialized research agents.
- Add support for multiple website sources.
- Improve source verification and factual accuracy.
- Implement advanced report evaluation metrics.
- Add a Streamlit-based interactive user interface.
- Export generated research reports into PDF format.
- Introduce memory to maintain research context across tasks.

Learning Outcomes

Through this project, I gained practical experience in:

- Multi-Agent AI System Development.
- Large Language Models (LLMs).
- LangChain Framework.
- Prompt Engineering.
- API Integration.
- Web Search and Web Scraping.
- Automated Report Generation.
- AI-Based Evaluation.
- Python Project Development.

Author

Khushboo Patel

B.Tech – Artificial Intelligence and Data Science

Interested in Artificial Intelligence, Machine Learning, Data Science, and Generative AI.
