# Medical Bot 

This project creates an advanced question-answering system tailored for medical inquiries. It harnesses the power of large language models, specifically Llama 2, to process and respond to user queries. The system's knowledge is derived from a collection of PDF documents, which are efficiently indexed and retrieved using vector store technology.

Key technologies employed in this project include:
- Llama 2: A state-of-the-art language model for generating accurate and contextual responses
- LangChain: A framework for developing applications powered by language models
- Chainlit: A tool for creating interactive chat interfaces
- FAISS: A library for efficient similarity search and clustering of dense vectors

This combination allows for intelligent document retrieval and natural language understanding, enabling the bot to provide informed answers to medical questions based on the ingested documentation.

## Setup
 1. Clone the repository:
 ```
 git clone https://github.com/yourusername/Medical-bot.git
 cd Medical-bot
```
2. Install the required packages:
   ```
   pip install langchain
   pip install langchain-core
   pip install langchain-huggingface
   pip install langchain-community
   pip install chainlit
   pip install PyPDF
   pip install torch
   pip install accelerate
   pip install bitsandbytes
   pip install ctransformers
   pip install sentence-transformers
   pip install faiss-cpu
   ```
3. Download the Llama 2 model:
   - Obtain the `llama-2-7b-chat.ggmlv3.q8_0.bin` file from a trusted source.
   - Place it in the root directory of the project.
     
4. Prepare your data:
   - Place your PDF documents in the `data/` directory.
  
## Usage
 1. Ingest the documents and create the vector store:
      ```
      python app.py
      ```
 2. Start the chat interface:
     ```
     chainlit run model.py -w
     ```
 3. Interact with the bot through the provided chat interface.

## Project Structure
 - `ingest.py`: Script for processing PDF documents and creating the vector store.
 - `model.py`: Defines the QA model and chat interface.
 - `data/`: Directory to store input PDF documents.
 - `vectorstore/db_faiss`: Directory where the FAISS vector store is saved.

## Dependencies
Main libraries used in this project:
  - langchain
  - PyTorch
  - Hugging Face Transformers
  - FAISS
  - Chainlit
  

