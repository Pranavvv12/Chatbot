# Chatbot-llama2-model
# Llama-Based QA System with FAISS

This project implements a question-answering (QA) system using the Llama model and the FAISS vector store. The application is designed to ingest PDF documents, create embeddings, and provide responses to user queries based on the content of those documents.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)


## Overview

The system consists of two main components:
1. **Ingest.py**: Responsible for loading PDF documents, creating embeddings, and saving them to a FAISS vector store.
2. **Model.py**: Loads the Llama model, sets up a retrieval QA chain, and processes user queries.

## Prerequisites

- Python 3.7 or later
- Google Colab or a local environment with access to Google Drive
- Basic knowledge of Python programming and machine learning concepts

## Installation

You can install the required libraries by running the following command in your Google Colab or local environment:

```bash
pip install langchain chainlit transformers sentence-transformers faiss-cpu huggingface_hub

