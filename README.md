# Document Retrieval and Question Answering with LangChain

This repository demonstrates a Python-based approach to document retrieval and question answering using LangChain, integrating various tools and techniques for efficient text processing and AI-driven responses.

## Features

- **Document Loading**: Load data from URLs, PDFs, and text files using LangChain's document loaders.
- **Text Embeddings**: Utilize Hugging Face embeddings to convert text into vector representations.
- **Vector Indexing**: Employ FAISS for creating vector indexes of documents for fast similarity search.
- **Question Answering**: Implement retrieval-based question answering using LangChain's integrated tools and Google's Generative AI for generating responses.

## Installation

Ensure Python 3.8 or higher is installed. Install dependencies using pip:

## bash
pip install langchain langchain-community unstructured sentence-transformers faiss-cpu langchain-google-genai

## Usage
Loading Data: Define your sources (URLs, PDF paths, text file paths) in the script and execute to load data into a unified format.

Creating Vector Index: Convert loaded text data into embeddings and build a FAISS vector index for efficient querying.

Question Answering: Set up your Google API key and initialize LangChain to perform retrieval-based question answering using Google's Generative AI.

# Example
python
Copy code
# Example query and response
response = qa.run({"query": "Who is Santiago? Explain his journey briefly."})
print(response.strip())
Configuration
Replace google_api_key with your actual Google API key in the script for using Google's Generative AI.
