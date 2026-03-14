# LangChain Watsonx RAG QA Bot

A Retrieval-Augmented Generation (RAG) Question Answering Bot built using LangChain, IBM Watsonx LLM, and Chroma Vector Database. This application allows users to upload a PDF document and ask questions about its content. The system retrieves relevant document sections and generates answers using an LLM.

## Features

- Upload PDF documents
- Ask questions about the document
- Automatic document chunking
- Semantic search using embeddings
- Retrieval-Augmented Generation (RAG)
- Interactive UI using Gradio

## Technologies Used

- LangChain – Framework for building LLM applications
- IBM Watsonx.ai – LLM and embedding models
- Granite LLM – Used to generate answers
- Slate 125M Embedding Model – Used for document embeddings
- ChromaDB – Vector database for storing embeddings
- Gradio – Web interface for the QA bot
- PyPDF – PDF document loader

## Project Architecture

PDF Document
↓
Document Loader
↓
Text Splitter
↓
Embedding Model (Slate 125M)
↓
Vector Database (ChromaDB)
↓
Retriever
↓
Granite LLM
↓
Generated Answer

## Project Structure

langchain-watsonx-rag-qa-bot
│
├── qabot.py
├── requirements.txt
├── embedding.png
└── README.md

## Installation

Clone the repository:

git clone https://github.com/MuhammadKhubaib1/langchain-watsonx-rag-qa-bot.git
cd langchain-watsonx-rag-qa-bot

Install dependencies:

pip install -r requirements.txt

## Run the Application

python qabot.py

The Gradio interface will start and you can:

1. Upload a PDF document
2. Enter a question
3. Receive an AI-generated answer based on the document

## Future Improvements

- Support multiple document uploads
- Add conversation memory
- Deploy the app as a web service
- Implement hybrid search or reranking

## Author

Muhammad Khubaib
