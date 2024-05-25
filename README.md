# Retrieval Augmented Generation (RAG) App

Hi! I'm excited to share a project I've been working on: a Retrieval Augmented Generation (RAG) application. This app leverages Langchain and OpenAI to interact with your own documents or data sources. Whether you have a collection of books, technical documentation, or any other text-based data, this application allows you to query and get meaningful, context-aware responses.

## Features

- Load and process large text datasets.
- Create a vector database using ChromaDB and OpenAI embeddings.
- Query the database for relevant information.
- Generate accurate responses based on retrieved data.
- Reference sources for transparency and reliability.

## Setup


### Prerequisites

To get started, make sure you have the following installed:
- Python 3.7 or higher
- pip (Python package installer)
- An OpenAI API key



## Preparation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Shreyansh-333/RAG-AI-Chatbot.git
   cd RAG-AI-Chatbot
   ```


2. **Install dependencies.:**  
  ```python
  pip install -r requirements.txt
  ```


3. **OpenAI API Key:**
Create a .env file in the root directory of the project and add your OpenAI API key:

  ```bash
  OPENAI_API_KEY = "your_openai_api_key"
  ```


4. **Data Source:**

Place your markdown files in the data/ directory. You can organize them into subfolders if needed.



## Create the Chroma DB.

  ```python
  python create_database.py
  ```

This will:

- Load your markdown files
- Split the documents into smaller chunks
- Generate vector embeddings for each chunk
- Save the embeddings to a ChromaDB database

![Alt text](/Screenshots/Embeddings.png)


## Query the Chroma DB.

  ```python
  python query_data.py "Your question"
  ```

This script will:

- Create a prompt using the retrieved data chunks
- Call the OpenAI API to generate a response
- Print the response along with source references

### Example

![Alt text](/Screenshots/Example.png)
![Alt text](/Screenshots/Retrieval.png)


By using retrieval augmented generation, the app ensures that the responses are both relevant and grounded in the provided data. This can be particularly useful for applications like customer support, educational tools, and more.
