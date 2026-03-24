# Haneen-AI-Customer-Service-Chatbot-using-FlowiseAI


Project Overview:

A Retrieval-Augmented Generation (RAG) chatbot designed for Haneen Company. It uses local LLMs to provide accurate, context-aware customer support based on a private knowledge base.

Tech Stack:

  - Orchestration: FlowiseAI

  - LLM: Llama 3 (via Ollama)

  - Embeddings: all-minilm

  - Vector Store:In-Memory

  - Environment: Run on MacBook Air using Docker.



System Architecture:

  - Data Ingestion: knowledge.txt processed via RecursiveCharacterText Splitter.

  - Vectorization: Text chunks converted to embeddings using all-minilm.

  - Retrieval: Similarity search to find relevant context for user queries.

  - Generation: Llama 3 generates concise answers strictly from the retrieved context.


  
How to Run:

 - Install Ollama, pull Llama 3 and all-minilm: 

    ollama pull llama3. 

    ollama pull all-minilm.

  - Run Flowise via Docker.

  - Import the JSON workflow file (provided in this repo).

  - Upload knowledge.txt
