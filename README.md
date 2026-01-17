# RAG In-Depth: Exploring Retrieval-Augmented Generation

A comprehensive exploration of Retrieval-Augmented Generation (RAG) systems using **LangChain** and **LangGraph**, covering the complete pipeline from data ingestion to vector storage and retrieval.

## 📋 Project Overview

This project provides hands-on implementations and explorations of RAG components:
- **Data Ingestion & Parsing** - Multiple file format support
- **Vector Embeddings** - Leveraging HuggingFace and OpenAI models
- **Vector Databases** - ChromaDB and FAISS implementations
- **RAG Pipeline** - End-to-end retrieval and generation workflows

## 📁 Project Structure

```
ExploringRAGs/
├── 0-DataIngestParsing/          # Data ingestion and parsing modules
│   ├── 1-dataingestion.ipynb      # Core data ingestion techniques
│   ├── 2-dataparsingpdf.ipynb     # PDF parsing
│   ├── 3-dataparsingdoc.ipynb     # Document parsing
│   ├── 4-csvexcelparsing.ipynb    # CSV & Excel parsing
│   ├── 5-jsonparsing.ipynb        # JSON parsing
│   └── 6-sqlparsing.ipynb         # SQL database parsing
│
├── 1-VectorEmbeddingAndDatabases/ # Embedding generation
│   ├── embedding.ipynb             # Embedding fundamentals
│   ├── huggingfaceembeddings.ipynb # HuggingFace embeddings
│   └── openaiembeddings.ipynb      # OpenAI embeddings
│
├── 2-VectorStore/                 # Vector database implementations
│   ├── 1-chromadb.ipynb           # ChromaDB setup and usage
│   └── 2-faiss.ipynb              # FAISS implementation
│
├── main.py                         # Main application entry point
├── pyproject.toml                 # Project dependencies
├── uv.lock                        # Locked dependencies
└── README.md                      # This file
```

## 🚀 Quick Start

### Prerequisites
- Python 3.10+
- `uv` package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/nameisahmedh/RAG-indepth.git
   cd RAG-indepth
   ```

2. **Install dependencies**
   ```bash
   uv sync
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Add your API keys:
   # OPENAI_API_KEY=your_key_here
   # GROQ_API_KEY=your_key_here
   ```

## 📚 Module Breakdown

### Phase 0: Data Ingestion & Parsing
Learn how to ingest and parse data from multiple sources:
- **PDF Documents** - Extract text and metadata from PDFs
- **Word Documents** - Parse .docx files
- **Spreadsheets** - Handle CSV and Excel formats
- **JSON Data** - Parse structured JSON files
- **Databases** - Query and extract from SQL databases

### Phase 1: Vector Embeddings
Understand embeddings and generate vectors for your data:
- **Embedding Fundamentals** - How embeddings work and why they matter
- **HuggingFace Embeddings** - Free, open-source embedding models
- **OpenAI Embeddings** - High-quality embeddings via OpenAI API

### Phase 2: Vector Stores
Explore vector database implementations:
- **ChromaDB** - Lightweight, in-memory vector store
- **FAISS** - Facebook's scalable similarity search library

## 🔧 Technologies Used

- **LangChain** - LLM orchestration framework
- **LangGraph** - Graph-based workflow automation
- **ChromaDB** - Vector database
- **FAISS** - Vector similarity search
- **HuggingFace Transformers** - Open-source embeddings
- **OpenAI API** - Commercial embeddings and LLMs

## 📝 Usage Examples

### Running Notebooks
```bash
jupyter notebook
```
Navigate to any `.ipynb` file to explore specific RAG components.

### Running Main Application
```bash
python main.py
```

## 🔐 Security Notes

⚠️ **Never commit API keys or secrets!** Use environment variables:
- Store sensitive data in `.env` file
- `.env` is already in `.gitignore`
- Load variables: `from dotenv import load_dotenv`

## 📖 Learning Path

1. Start with **0-DataIngestParsing** to understand data preparation
2. Move to **1-VectorEmbeddingAndDatabases** to learn embeddings
3. Explore **2-VectorStore** for vector storage solutions
4. Review `main.py` for integrated pipeline example

## 🚧 Coming Soon

- [ ] Advanced RAG techniques (re-ranking, fusion)
- [ ] Multi-modal embeddings
- [ ] Production-ready deployment guide
- [ ] Performance benchmarking
- [ ] Complete end-to-end RAG application
- [ ] Testing and evaluation frameworks

## 📞 Contact & Support

For questions or issues, please create a GitHub issue.

---

**Happy exploring! 🚀**