# **AncestryDNA FAQ Agent**


https://github.com/user-attachments/assets/0e772304-d4ef-448f-afa9-68089868dfb4


This project is a question-answering agent built using **Langflow** that provides detailed responses to frequently asked questions about AncestryDNA's services. The agent is powered by an extensive knowledge base derived directly from the official AncestryDNA FAQ.

## **Features**

* **FAQ Agent:** A single, focused agent designed to accurately answer questions based on a specific knowledge source.  
* **Knowledge Base / RAG:** The agent's knowledge is Vector Database populated with AncestryDNA's publicly available Frequently Asked Questions.  
* **Langflow Integration:** The entire project is constructed as a Langflow chart, allowing for a visual, no-code/low-code approach to building and managing the agent's logic.  

## **Flow Overview**

The Langflow chart for this project is designed for simplicity and efficiency. The core components include:

* File Upload component for **AncestryDNA Frequently Asked Questions.pdf** primary knowledge source for the Agent

* A **Vector Store** Astra DB containing the FAQ data from AncestryDNA. This is the agent's primary knowledge source.  

* An **Agent** component that acts as the central orchestrator.  

* An **LLM** llama 3.2 that acts as the agent's reasoning engine.

The agent takes a user's question, performs a vector search against the FAQ knowledge base, and synthesizes a relevant answer.
