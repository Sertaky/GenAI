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

1- Pretrained Language Model: Llama 2 for conversational intelligence.

2- Vector Database: Pinecone for storing and retrieving embeddings.

3- LangChain Framework: To chain model responses with retrieval mechanisms.

=================================================================================================================================================

# 2_Falcon_7b_with_LangChain_test

This project demonstrates the usage of the Falcon-7B model with LangChain to generate high-quality text. Falcon-7B is a powerful large language model designed for natural language processing tasks. This notebook shows how to set up and use the model for text generation tasks using HuggingFace and LangChain.

## Features
- **Falcon-7B Integration**: Utilizes the `tiiuae/falcon-7b-instruct` model for text generation.
- **LangChain Support**: Leverages LangChain to structure and manage interactions with the language model.
- **Customizable Parameters**: Allows configuration of text generation parameters such as `max_length`, `top_k`, and more.

## Requirements

Before running the notebook, ensure you have the following:

- Python 3.8 or higher
- A GPU-enabled system for optimal performance
- Libraries:
  - `transformers`
  - `einops`
  - `accelerate`
  - `langchain`
  - `bitsandbytes`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Sertakye/2_Falcon_7b_with_LangChain_test.git
   cd 2_Falcon_7b_with_LangChain_test
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Check GPU availability:
   ```bash
   !nvidia-smi
   ```

## Usage

1. **Load the Model**:
   The notebook initializes the Falcon-7B model using HuggingFace's pipeline:
   ```python
   from transformers import AutoTokenizer, pipeline

   model = "tiiuae/falcon-7b-instruct"
   tokenizer = AutoTokenizer.from_pretrained(model)
   pipeline = pipeline(
       "text-generation",
       model=model,
       tokenizer=tokenizer,
       torch_dtype=torch.bfloat16,
       trust_remote_code=True,
       device_map="auto",
       max_length=200,
       do_sample=True,
       top_k=10,
       num_return_sequences=1
   )
   ```

2. **Run the Notebook**:
   Launch the notebook and execute the cells sequentially to load the model and generate text.

3. **Generate Text**:
   Use the configured pipeline to input a prompt and receive generated text:
   ```python
   result = pipeline("Your input prompt here")
   print(result)
   ```

## Example Output
- **Input**: "What are the applications of Falcon-7B?"
- **Output**: "Falcon-7B can be used in a wide range of applications including chatbots, content creation, code generation, and more."

========================================================================================================================================================================


