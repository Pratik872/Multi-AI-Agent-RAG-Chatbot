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

- Prompts would be passed to this model using Groq API

### 3 - Creating a prompt for LLM
- Created a prompt template using `Langchain`

- Defined the prompt to LLM using prompt template

### 4 - Getting transcripts for the video/website using external tools and `Langchain`
- Fetching the URL uploaded by user through streamlit

- Used this URL to get transcripts through `YoutubeLoader` and `UnstructuredURLLoader` in `Langchain` and converting those to data which needs to be passed to the LLM


### Sample Working

![Demo](https://github.com/Pratik872/Youtube-Video-Summarizer/blob/main/readme%20resources/app%20sample.png)


### Built with 🛠️
- Packages/Repo : Langchain, Jupyter, Streamlit, Groq

- Coded on : Jupter Notebook (modelling), VSCode(building application)

