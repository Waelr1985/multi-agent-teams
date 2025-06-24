# LangGraph Multi-Agent Workflow Guide.
# 🌐 Building Complex Multi-Agent Teams and Workflows using LangGraph

This repository showcases progressively complex multi-agent workflows built using **LangGraph** and **LangChain**. The examples begin with simple chains and evolve into full-fledged, asynchronous multi-agent systems capable of executing intricate tasks like travel planning and web research.

---

## 📘 Project Overview

The project is a step-by-step tutorial demonstrating:

- Building agents with custom system prompts and tools
- Connecting agents into workflows using LangGraph
- Orchestrating asynchronous agents and file generation tasks

---

## 🧱 Modules Breakdown

### 🔹 Part 1 – LangChain Basics (`langchain_basics.py`)
- Learn LangChain fundamentals
- Create prompt templates and simple translation chains

### 🔹 Part 2 – Agent Tools (`tools/`)
- Implement tools like:
  - Image generation
  - Weather data retrieval
  - PDF export
  - Asynchronous web scraping

### 🔹 Part 3 – Simple LangGraph (`simple_langgraph.py`)
- Create a single agent workflow
- Loop agent with a tool executor until completion

### 🔹 Part 4 – Multi-Agent Setup (`multi_agent.py`)
- Introduce a team of agents (e.g., travel agent, designer)
- Add PDF generation capabilities

### 🔹 Part 5 – Advanced Multi-Agent Workflow (`multi_agent.py`)
- Expand the agent team into a fully coordinated system
- Build end-to-end travel itineraries with images and PDF output

### 🔹 Final – Web Research Workflow (`web_research.py`)
- Incorporate asynchronous tools
- Fetch and summarize online content
- Output a markdown-based article

---

## 🗂️ Repository Contents

| File / Folder                  | Description |
|-------------------------------|-------------|
| `langchain_basics.py`         | Basic LangChain usage and expression chains |
| `simple_langgraph.py`         | Simple looping agent using LangGraph |
| `multi_agent.py`              | Multi-agent team with a supervisor and PDF output |
| `web_research.py`             | Asynchronous agents for web search and content writing |
| `tools/`                      | Utilities for image creation, weather, PDFs, web scraping |
| `setup_environment.py`        | Loads API keys and sets LangChain project name |
| `multi_agent_prompts.py`      | System prompts for multi-agent workflows |
| `web_research_prompts.py`     | Prompts for the web research workflow |

---

## 🧠 Key Learnings

Through these examples, you'll learn how to:

1. 🧩 **Define modular agents** using system prompts and tools.
2. 🔄 **Create agent workflows** using LangGraph’s `StateGraph` to manage message passing.
3. ⚙️ **Build asynchronous pipelines** to integrate web data, analyze content, and generate files.

---

## 🚀 Get Started

To run any script:
```bash
python path/to/script.py
```

Make sure to configure your environment using:
```bash
python setup_environment.py
```

Set API keys for any external services (e.g., OpenAI, weather, Tavily).

---

## 🧰 Requirements

- Python 3.9+
- LangChain
- LangGraph
- Additional APIs (OpenAI, Tavily, etc.)

---

## 📄 License

This project is provided for educational purposes and experimentation. Check individual dependencies for their licenses.

---

Feel free to contribute, explore, and build your own agentic workflows with LangGraph!
