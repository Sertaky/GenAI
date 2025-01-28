# GenAI

# 1_Website Bot using Llama 2, Pinecone & LangChain

This project implements an interactive chatbot powered by Llama 2, Pinecone, and LangChain. The bot can answer queries, provide context-based information, and utilize vector-based search for enhanced responses. It leverages the capabilities of modern language models for high-quality interactions.

## Features
- **Llama 2 Integration:** Utilizes Llama 2, a powerful large language model, for detailed and accurate conversational responses.
- **Pinecone Vector Search:** Implements Pinecone to enable efficient storage and retrieval of vector embeddings for context-based Q&A.
- **LangChain Support:** Employs LangChain for seamless chaining of language models and contextual understanding.
- **Interactive Chat Interface:** A user-friendly interface to input prompts and receive responses.

## Requirements
- Python 3.8 or higher
- Dependencies (e.g., LangChain, Pinecone, OpenAI libraries)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Sertaky/GenAI.git
   cd 1_Website Bot using Llama 2, Pinecone & LangChain
2. Set up your API keys:

Obtain API keys for Pinecone and OpenAI.
Add them to your environment variables or a .env file.

3.Run the notebook or script:
 '''bash
         jupyter notebook Website_bot_using_Llama2,_Pinecone_&_LangChain.ipynb

## Usage
1- Launch the chatbot by running the notebook.
2- Enter your query in the prompt field.
3- The chatbot will provide an intelligent response based on the context.

## Architecture
The project architecture involves:

Pretrained Language Model: Llama 2 for conversational intelligence.
Vector Database: Pinecone for storing and retrieving embeddings.
LangChain Framework: To chain model responses with retrieval mechanisms.
