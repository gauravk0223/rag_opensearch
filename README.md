# Retrieval Augmented Generation (RAG) Pipeline with LangChain and OpenSearch

This repository implements a **Retrieval Augmented Generation (RAG) pipeline** using [LangChain] and [OpenSearch](https://opensearch.org/). The pipeline enables efficient document ingestion, semantic chunking, vector storage, and intelligent retrieval for advanced NLP applications.

---

## 🚀 Key Features

- **PDF Loader:** Easily ingest and process PDF documents for downstream NLP tasks.
- **Semantic Chunking:** Breaks documents into meaningful chunks for improved retrieval accuracy.
- **OpenSearch Vector Store:** Utilizes OpenSearch as a scalable vector database for storing and searching document embeddings.
- **HNSW Indexing:** Implements Hierarchical Navigable Small World (HNSW) algorithm for fast and accurate vector similarity search.
- **LangChain Prompt Integration:** Leverages prompts from the LangChain hub for flexible and customizable language model interactions.

---

## 🛠️ Getting Started

### 1. Clone the Repository
git clone https://github.com/gauravk0223/rag_opensearch.git

### 2. pip install -r requirements.txt  (Make sure you have Python 3.13 installed)

### 3. Run OpenSearch Locally with Docker
    docker pull opensearchproject/opensearch:latest
    docker run -it -p 9200:9200 -p 9600:9600 -e OPENSEARCH_INITIAL_ADMIN_PASSWORD=<password> -e "discovery.type=single-node"  --name opensearch-node opensearchproject/opensearch:latest
