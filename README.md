# AI From Scratch

[![Python](https://img.shields.io/badge/Python-3.14+-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NavneetSinghArora/AI-From-Scratch/blob/main/src/vector-embeddings.ipynb)
[![Hugging Face](https://img.shields.io/badge/🤗%20Hugging%20Face-Models-FFD21E)](https://huggingface.co/sentence-transformers)
[![uv](https://img.shields.io/badge/uv-package%20manager-DE5FE9)](https://docs.astral.sh/uv/)
[![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE)

A hands-on learning repository for exploring AI and Machine Learning concepts through practical Jupyter notebooks. Each notebook is self-contained, runnable locally or directly in Google Colab, and focused on building intuition from the ground up.

## Notebooks

| Notebook | Description | Open |
|---|---|---|
| [Vector Embeddings](src/vector-embeddings.ipynb) | Dense vector embeddings with SBERT, cosine similarity, and 2D PCA visualisation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NavneetSinghArora/AI-From-Scratch/blob/main/src/vector-embeddings.ipynb) |

## Setup

### Prerequisites

- Python 3.14+
- [`uv`](https://docs.astral.sh/uv/) — used for dependency and environment management

### Local installation

```bash
git clone https://github.com/NavneetSinghArora/AI-From-Scratch.git
cd AI-From-Scratch

# Create virtual environment and install dependencies
uv sync

# Install notebook-specific dependencies
uv pip install sentence-transformers
```

### Environment variables

Create a `.env` file in the project root:

```bash
HF_TOKEN=your_huggingface_token_here
```

A Hugging Face token is optional for public models but recommended. Get one at [huggingface.co/settings/tokens](https://huggingface.co/settings/tokens).

### Running in Google Colab

Each notebook has an **Open in Colab** badge. Before running:

1. Go to **Tools > Secrets** in the Colab menu
2. Add a secret named `HF_TOKEN` with your Hugging Face token
3. Run all cells

## Repository Structure

```
AI-From-Scratch/
├── src/
│   └── vector-embeddings.ipynb   # SBERT embeddings & similarity visualisation
├── .env                           # Local secrets (not committed)
├── pyproject.toml
└── README.md
```

## References

- [Sentence Transformers (SBERT)](https://sbert.net/)
- [Pretrained SBERT models](https://sbert.net/docs/sentence_transformer/pretrained_models.html)
- [all-MiniLM-L6-v2 on Hugging Face](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2)
