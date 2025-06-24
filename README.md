# Building complex multi-agent teams and setups using LangGraph.

This repository contains the finished code for the "Building complex multi-agent teams and setups using LangGraph".

It is a collection of example code that walks through building increasingly complex multi-agent workflows with **LangGraph** and **LangChain**.


## Introduction



- **Part 1 (`langchain_basics.py`)** – Learn LangChain basics by creating prompt templates and simple chains.
- **Part 2 (`tools/` directory)** – Write agent tools such as image generation and weather lookup functions.
- **Part 3 (`simple_langgraph.py`)** – Introduce LangGraph with an agent that returns a visual of the current weather.
- **Part 4 (`multi_agent.py`)** – Build a small team of agents and add a PDF generation tool.
- **Part 5 (`multi_agent.py`)** – Expand the team into a robust workflow that produces complete travel itineraries in PDF format.
- **Final Part (`web_research.py`)** – Add asynchronous tools and create a web research workflow that writes an article.

## Repository Overview

This project demonstrates different styles of LangGraph workflows, starting with basic chains and growing to a multi-agent team.

### Key Components

- **`multi_agent.py`** – defines a full team of agents (travel agent, language assistant, visualizer, designer) overseen by a supervisor. The workflow wires these agents into a `StateGraph` so the supervisor can route control among them and finish by generating a PDF.
- **`simple_langgraph.py`** – shows a smaller example where an agent loops with a tool executor until the agent signals completion.
- **`web_research.py`** – demonstrates asynchronous agents that search the web, gather page content concurrently, and write the results to a markdown file.
- **`tools/`** – contains utilities for image creation, PDF generation, weather lookup, and asynchronous webpage retrieval.

### Overall

These scripts illustrate how to:
1. Define agents with system prompts and tools.
2. Wire agents together into LangGraph workflows that pass messages between them.
3. Extend workflows with asynchronous tasks and file output.

## Scripts

The repository includes several standalone examples that can be run individually:

- **`langchain_basics.py`** – a minimal script showing the LangChain Expression
  Language (LCEL). It creates a simple chain that translates a word to French
  and German and then checks the result using a second chain.
- **`simple_langgraph.py`** – demonstrates LangGraph fundamentals with a single
  agent that can fetch the weather and generate images using tools.
- **`multi_agent.py`** – builds a full team of agents managed by a supervisor.
  The team collaborates to produce a travel itinerary with an image and final
  PDF output.
- **`web_research.py`** – an asynchronous workflow that performs a Tavily search
  and then gathers webpage content concurrently before writing the result to a
  markdown file.
- **`setup_environment.py`** – helper for loading API keys and setting the
  LangChain project name via environment variables.
- **`multi_agent_prompts.py`** and **`web_research_prompts.py`** – store the
  system prompts used by the main workflows.

## Repository Overview

This project demonstrates different styles of LangGraph workflows, starting with basic chains and growing to a multi-agent team.

### Key Components

- **`multi_agent.py`** – defines a full team of agents (travel agent, language assistant, visualizer, designer) overseen by a supervisor. The workflow wires these agents into a `StateGraph` so the supervisor can route control among them and finish by generating a PDF.
- **`simple_langgraph.py`** – shows a smaller example where an agent loops with a tool executor until the agent signals completion.
- **`web_research.py`** – demonstrates asynchronous agents that search the web, gather page content concurrently, and write the results to a markdown file.
- **`tools/`** – contains utilities for image creation, PDF generation, weather lookup, and asynchronous webpage retrieval.

### Overall

These scripts illustrate how to:
1. Define agents with system prompts and tools.
2. Wire agents together into LangGraph workflows that pass messages between them.
3. Extend workflows with asynchronous tasks and file output.


