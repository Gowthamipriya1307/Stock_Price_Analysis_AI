# AI Crew for Stock Analysis 🧠📊

## Introduction

This is a GenAI-based project that automates end-to-end stock research and investment analysis using the CrewAI framework. I designed this multi-agent system to simulate how financial analysts, researchers, and advisors collaborate to analyze a company and generate insights.

Built as a learning project for exploring Retrieval-Augmented Generation (RAG), agent collaboration, and financial data tools — integrating LLMs like GPT-4 or local models like Ollama.

---

## Table of Contents
- [Overview of CrewAI Framework](#crewai-framework)
- [How to Run](#how-to-run)
- [Architecture & Files](#architecture--files)
- [Using GPT-3.5 (Optional)](#using-gpt-35-optional)
- [Running with Local LLMs (Ollama)](#running-with-local-llms-ollama)
- [License & Acknowledgements](#license--acknowledgements)

---

## CrewAI Framework

CrewAI is a multi-agent framework where role-based LLM agents coordinate with each other to complete a complex task. In this use case, I've configured agents like:

- **Financial Analyst** → Reviews 10-K, 10-Q filings
- **Market Researcher** → Scrapes real-time insights
- **Investment Advisor** → Recommends action

They interact to produce a summary stock report.

---

## How to Run

### Requirements

- Python 3.9+
- Access to [OpenAI GPT-4 API](https://platform.openai.com/api-keys)
- Keys from:
  - [Browserless](https://www.browserless.io/)
  - [Serper.dev](https://serper.dev/)
  - [SEC API](https://sec-api.io)

### Steps

```bash
# Clone the repo
git clone https://github.com/YourGitHubUsername/ai-crew-stock-analysis.git
cd ai-crew-stock-analysis

# Set up environment
cp .env.example .env
# Add your API keys inside .env

# Install dependencies
poetry install --no-root

# Run the script
poetry run python main.py
