# Research Assistant Agent

An AI-powered research assistant built with **LangChain** and **GPT-4o-mini**. You enter a topic, and the agent automatically searches the web and Wikipedia, summarizes the results, and saves structured data to `research_output.txt`.

## Installation
bash
git clone https://github.com/your-username/research-agent.git
cd research-agent
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
pip install -r requirements.txt
requirements.txt


## requirements.txt

langchain
langchain-openai
langchain-anthropic
langchain-community
python-dotenv
pydantic
duckduckgo-search
wikipedia


##  Create a .env file:

OPENAI_API_KEY=your_openai_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key

## Run
python main.py


## When prompted:

What can i help you researching? → History of AI

## How it works

The script builds a LangChain agent with three tools:

- search_tool — searches the web via DuckDuckGo

- wiki_tool — fetches data from Wikipedia

- save_tool — writes results to research_output.txt
