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

## Getting Started

To get started with the Llama2 Medical Bot, you need to:

1. Set up your environment and install the required packages as described in the Installation section.

2. Configure your project by updating the `DB_FAISS_PATH` variable and any other custom configurations in the code.

3. Prepare the language model and data as per the Langchain documentation.

4. Start the bot by running the provided Python script or integrating it into your application.


