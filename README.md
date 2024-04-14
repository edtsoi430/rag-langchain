# rag-langchain

## Motivation
I enjoy learning by reading books, but nowadays I often struggle to find time to scroll through hundreds or even thousands of pages of words.

This project aims to take advantage of Retrieval-Augumented Generation (RAG), where I feed in books of interest and use LLM to generate responses to user queries. 

We'll be using:
- ChromaDB, 
- OpenAI embedding function, and
- Langchain

## Usage
I use rye to manage my project dependencies.

To use Rye to create a database (with ChromaDB):
```
rye run create-db
```

To use Rye to query ChromaDB:
```
rye run query "<your prompt goes in here>"
```

Alternatively, you could run:
```
python ./src/rag_langchain/query_data.py "<your prompt>"
```
etc.

You would also need an openAI account and set up the API key in your environment variable.

## Credits
- Special credits to https://github.com/pixegami/langchain-rag-tutorial