# Building complex multi-agent teams and setups using LangGraph.

This repository contains the finished code for the "Building complex multi-agent teams and setups using LangGraph".

It is a collection of example code that walks through building increasingly complex multi-agent workflows with **LangGraph** and **LangChain**.


## Introduction



- In part 1, we'll get started with the basics of LangChain, learning how to create prompt templates and Chains, working with the LangChain syntax to easily string together our LLM calls.
- In the next part we'll learn how to write tools so that we can make our future agents powerful by giving them functions they can call. We will use the newest LangChain syntax for this and create both an image generation tool and a weather tool.
- Part 3 is where we will learn the basics of LangGraph, covering the underlying concepts and exactly how it works. We will learn by setting up our first agent and graph which can return a visual representation of the current weather in any city you name.
- In part 4 we'll look at how we can take this all to yet the next level, discussing how we can use all of this to create a whole team of agents working together for us. We'll also write a tool that can output PDF files in preparation for our multi-agent setup.
- Part 5 is where the rubber really hits the road and we will create a powerful multi-agent setup in LangGraph using a team, team manager, many agents, conditional paths, and more. We will create a team that can work together independently and create travel itineraries for us, providing them in PDF format with an inserted image and a full travel plan.
- In the final part we'll have a look at writing asynchronous tools for our agents and then create a web research and article writing graph that can visit many web pages at the same time and then write an article about our desired topic for us.

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


