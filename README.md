# Contextual Text Similarity with Sentence-BERT

This project demonstrates how to compute contextual text similarity using the **Sentence-BERT** model. The goal is to calculate the similarity between text pairs and find the most contextually similar sentences to a user-provided input sentence from a dataset.

## Features

- Uses **Sentence-BERT** (`all-MiniLM-L6-v2`) to compute embeddings for sentences.
- Calculates **cosine similarity** between embeddings to measure text similarity.
- Loads and evaluates text similarity using the **STS Benchmark dataset**.
- Finds the **top 5 most similar sentences** from the dataset for a given user input.

## Example

**Input:**
