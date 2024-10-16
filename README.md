# Multi-AI-Agent-RAG-Chatbot

## Overview
- A web application with multi AI agents co-ordinating with each other to generate completions for user queries

- An agent with RAG framework to search the vector stores for relevant answer and another agent to search wikipedia if the answer is not found in stores.

- Routing using LangGraph to appropriate functions

## Problem Objective
- To build a web application with multiple AI agents to answer user queries.

## Methodology

![App Demo](https://github.com/Pratik872/Youtube-Video-Summarizer/blob/main/readme%20resources/app%20demo.png)

The Web Application involves:
- RAG Agent - Loading the webpages and storing their embedding vectors into vector stores

- Wikipedia Agent Implementation

- Designing a prompt for LLM

- LangGraph for multi AI agent implementation

### 1 - RAG Agent
- Used `WebBaseLoader` from `Langchain` to load the web pages

- Used `Huggingface` embeddings to vector for the documents

- Stored the vectors in `Astra DB` through `Langchain`

### 2 - Wikipedia Agent Implementation
- Used `WikipediaAPIWrapper` to get response from wikipedia if the answer is not found in vector stores created
![wiki demo](https://github.com/Pratik872/Multi-AI-Agent-RAG-Chatbot/blob/main/readme%20resources/wiki%20demo.png)

### 3 - Designing a prompt for LLM
- Created a prompt template using `Langchain`

- Defined the prompt to LLM using prompt template

### 4 - Langgraph Nodes for multi-AI Agent
![nodes](https://github.com/Pratik872/Multi-AI-Agent-RAG-Chatbot/blob/main/readme%20resources/nodes.png)


### Sample Working
- RAG demo
![RAG](https://github.com/Pratik872/Multi-AI-Agent-RAG-Chatbot/blob/main/readme%20resources/demo1.png)

- Wikipedia demo
![Wiki](https://github.com/Pratik872/Multi-AI-Agent-RAG-Chatbot/blob/main/readme%20resources/demo2.png)


### Built with 🛠️
- Packages/Repo : Langchain, Jupyter, Groq, LangGraph

- Coded on : Jupter Notebook (modelling), VSCode(building application)

