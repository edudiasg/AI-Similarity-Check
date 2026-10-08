---
title: Embedding
emoji: 🖼️
colorFrom: yellow
colorTo: red
sdk: static
app_file: index.html
pinned: false
short_description: Vector Similarity Check
---

# AI Similarity Check

Compare the semantic meaning of two phrases directly in your browser using Transformers.js and the ONNX version of `all-MiniLM-L6-v2`.

**[Try the live demo on Hugging Face](https://huggingface.co/spaces/edudiasg/embedding)**

## How to use

1. Enter two phrases, preferably in English.
2. Click **Compare phrases**.
3. Read the cosine similarity score: values closer to **1** indicate more similar embeddings.

The score is not a probability or a percentage of correctness. The first comparison downloads the model and may take a little while.

## Technology

- HTML, CSS, and JavaScript
- Transformers.js
- Model: [Xenova/all-MiniLM-L6-v2](https://huggingface.co/Xenova/all-MiniLM-L6-v2)
- Hugging Face Static Spaces

Model inference runs in the browser without a Python backend or an API key.

## Deployment

Changes pushed to `main` trigger the GitHub Actions workflow that uploads the application to [the Hugging Face Space](https://huggingface.co/spaces/edudiasg/embedding).

To sync manually, open **Actions → Sync to Hugging Face Hub → Run workflow**.

The workflow requires a repository secret named `HF_TOKEN` with write access to the destination Space.
