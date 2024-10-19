# Chatbot-llama2-model
# Llama-Based QA System with FAISS

This project implements a question-answering (QA) system using the Llama model and the FAISS vector store. The application is designed to ingest PDF documents, create embeddings, and provide responses to user queries based on the content of those documents.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Running the Code](#runningtheCode)

## Llama Model

The Llama model used in this project can be found on Hugging Face. You can access it using the following link:

[Download Llama Model](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/blob/main/llama-2-7b-chat.ggmlv3.q8_0.bin)

## Disclaimer

As of now, this repository contains only medical-related content. Users are encouraged to modify and customize the content as needed. If you remove or alter the existing PDF documents, you are free to provide your respective PDF contents to tailor the application to your specific requirements. 


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
```

## Getting Started

To get started with the Llama2 Medical Bot, you need to:

1. Set up your environment and install the required packages as described in the Installation section.

2. Configure your project by updating the `DB_FAISS_PATH` variable and any other custom configurations in the code.

3. Prepare the language model and data as per the Langchain documentation.

4. Start the bot by running the provided Python script or integrating it into your application.

## Usage

The Llama2 Medical Bot can be used for answering medical-related queries. To use the bot, you can follow these steps:

1. Start the bot by running your application or using the provided Python script.

2. Send a medical-related query to the bot.

3. The bot will provide a response based on the information available in its database.

4. If sources are found, they will be provided alongside the answer.

5. The bot can be customized to return specific information based on the query and context provided.

## Running the Code

Step 1: Create Vector Store with `ingest.py`

The first step is to ingest your PDF files and create the FAISS vector store.

To run `ingest.py`:

```bash
python ingest.py
```

Step 2: Start the QA Bot with `model.py`

To run model.py:

```bash
python model.py
```



