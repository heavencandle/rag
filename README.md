# RAG Implementation with LangChain

This repository contains implementations of Retrieval-Augmented Generation (RAG) using LangChain, with two approaches: off-the-shelf and custom logic with LangChain Execution Layer (LCEL).

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/heavencandle/rag
    cd rag
    ```

2. Create a virtual environment and activate it:

    ```bash
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

### RAG Off-The-Shelf

The `rag_off_the_shelf.py` script uses LangChain's off-the-shelf RAG implementation.

1. Load, split, and embed documents.
2. Store embeddings in Chroma vector store.
3. Use the `RetrievalQA` chain with the "refine" chain type.

To run this script:

```bash
python rag_off_the_shelf.py
