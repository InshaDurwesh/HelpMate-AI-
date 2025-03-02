# HelpMateAI: Building an Effective Search System

## Project Overview
HelpMateAI is an advanced generative search system designed to process and extract accurate, context-rich answers from long-form policy documents. Using Retrieval-Augmented Generation (RAG) techniques, the project optimizes document processing, embedding generation, semantic search, and response quality.

## Features
- **Document Processing:** Efficiently reads and preprocesses long insurance policy documents.
- **Chunking and Embeddings:** Uses optimized chunking strategies and SentenceTransformer models for high-quality embeddings.
- **Vector Database:** Stores embeddings in ChromaDB for fast and scalable search.
- **Semantic Search:** Embeds user queries and matches against document embeddings with caching for efficiency.
- **Re-Ranking:** Enhances result relevance using cross-encoder models.
- **Generative Response:** Uses GPT-3.5 with well-engineered prompts to generate accurate answers with citations.

## System Architecture
1. **Embedding Layer:** Processes and chunks documents, generating embeddings using models like SentenceTransformers.
2. **Search Layer:** Embeds queries, searches ChromaDB, implements caching, and re-ranks results.
3. **Generation Layer:** Uses top-ranked results and GPT-3.5 to generate final responses.

## Prerequisites
- Python 3.7+
- `pdfplumber` for PDF processing
- ChromaDB for vector storage
- HuggingFace models for embeddings and re-ranking
- OpenAI API key stored in a text file named `OpenAI_API_Key`

## Future Enhancements
- Explore advanced embedding models and dynamic chunking techniques.
- Improve scalability and adaptability for diverse document types.
- Integrate more efficient caching and indexing strategies.

## License
This project is licensed under the MIT License.

