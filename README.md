# AI Digital Marketing RAG Assistant using n8n

## Overview

This project is an AI-powered Retrieval-Augmented Generation (RAG) assistant built using n8n. It automatically indexes Digital Marketing documents stored in Google Drive into a Pinecone vector database and allows users to ask questions through an AI chatbot.

The assistant retrieves relevant information from the uploaded documents and generates responses using Google Gemini, ensuring answers are based on the knowledge base rather than general AI knowledge.

---

## Features

- Automatically monitors a Google Drive folder for new or updated PDF files.
- Downloads documents from Google Drive.
- Generates vector embeddings using Google Gemini Embeddings.
- Stores document embeddings in Pinecone Vector Database.
- AI chatbot powered by Google Gemini.
- Retrieval-Augmented Generation (RAG) architecture.
- Uses conversation memory for improved interactions.
- Answers only from the uploaded Digital Marketing knowledge base.
- Prevents hallucinations by restricting responses to retrieved context.

---

## Workflow

### Document Indexing

Google Drive Trigger (New/Updated File)
⬇
Download PDF from Google Drive
⬇
Default Data Loader
⬇
Google Gemini Embeddings
⬇
Pinecone Vector Store

---

### Question Answering

Chat Trigger
⬇
AI Agent
⬇
Vector Store Retrieval (Pinecone)
⬇
Google Gemini
⬇
Answer returned to the user

---

## Technologies Used

- n8n
- Google Drive API
- Google Gemini
- Google Gemini Embeddings
- Pinecone Vector Database
- AI Agent (LangChain Nodes)
- Retrieval-Augmented Generation (RAG)

---

## Use Case

This workflow enables businesses, students, and professionals to build an AI knowledge assistant that can answer questions from their own Digital Marketing documents instead of relying on general AI knowledge.

Example applications include:

- Digital Marketing knowledge assistant
- Internal company knowledge base
- Employee training chatbot
- Educational document chatbot
- Course material assistant

---

## Workflow Components

- Google Drive Trigger
- Google Drive Download
- Default Data Loader
- Google Gemini Embeddings
- Pinecone Vector Store
- Chat Trigger
- AI Agent
- Memory Buffer
- Vector Store Tool
- Google Gemini Chat Model

---

## AI Guardrails

The AI Agent is configured to:

- Answer only using retrieved knowledge.
- Avoid hallucinations.
- Refuse questions outside the uploaded documents.
- Cite document information when available.
- Provide beginner-friendly explanations.

---

## Future Improvements

- Support multiple document formats (PDF, DOCX, TXT)
- Source citations with page numbers
- Web interface for end users
- Authentication and user management
- Multi-knowledge-base support
- Conversation history
- Deployment on cloud infrastructure

---

## Author

Ruhi

AI Automation | n8n Developer | Digital Marketing Automation
