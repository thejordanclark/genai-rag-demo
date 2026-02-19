# GenAI Bootcamp - RAG System Demo

This repository demonstrates a simple Retrieval-Augmented Generation (RAG) system for clinical trial documentation using **local models only** (no API keys required).

## Purpose
- Demonstrate RAG architecture for GxP environments
- Show document ingestion and retrieval
- Illustrate compliance considerations (data lineage, validation)
- Use only local models for data privacy

## Architecture

Documents → Chunking → Embeddings → Vector DB → Retrieval → Context

## Components

1. **Document Processor** - Loads and chunks documents
2. **Vector Store** - Stores embeddings using ChromaDB (local)
3. **RAG Engine** - Retrieves relevant context for queries
4. **UI App** - Simple Gradio interface for testing

## Technology Stack

- **Embeddings:** sentence-transformers (all-MiniLM-L6-v2) - runs locally
- **Vector DB:** ChromaDB - runs locally, no server needed
- **UI:** Gradio - simple web interface
- **No external APIs required** - everything runs on your machine

## Running the Demo

```bash
# Install dependencies
pip install -r requirements.txt

# Ingest documents
python src/document_processor.py

# Run the RAG system
python src/rag_engine.py

# Launch UI (optional)
python src/ui_app.py
```

## Compliance Features

- Data lineage tracking (what documents were used)
- Query logging (audit trail)
- Source attribution (which document provided the answer)
- Local processing (no data sent to external APIs)
- Deterministic retrieval (same query = same results)

## Sample Queries

See `demo_queries.md` for example queries to test the system.
