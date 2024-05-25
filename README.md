# Retrieval Augmented Generation (RAG) App

Welcome to the RAG (Retrieval Augmented Generation) application project! This project demonstrates how to build an AI-powered application that interacts with your own documents or data sources using Langchain and OpenAI. This type of application is ideal for handling large text datasets, enabling you to ask questions or create custom chatbots based on your data.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Setup](#setup)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [Usage](#usage)
  - [Data Preparation](#data-preparation)
  - [Creating the Vector Database](#creating-the-vector-database)
  - [Querying the Database](#querying-the-database)
  - [Generating Responses](#generating-responses)
- [Example](#example)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project showcases how to create a Retrieval Augmented Generation (RAG) application using Langchain and OpenAI. The application can process large amounts of text data, enabling sophisticated interactions like question-answering and chatbot functionalities.

## Features

- Load and process large text datasets
- Create a vector database using ChromaDB and OpenAI embeddings
- Query the database for relevant information
- Generate accurate responses based on retrieved data
- Reference sources for transparency

## Setup

### Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.7 or higher
- pip (Python package installer)
- An OpenAI API key

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/rag-app.git
   cd rag-app

Install dependencies.

```python
pip install -r requirements.txt
```

Create the Chroma DB.

```python
python create_database.py
```

Query the Chroma DB.

```python
python query_data.py "How does Alice meet the Mad Hatter?"
```

You'll also need to set up an OpenAI account (and set the OpenAI key in your environment variable) for this to work.
