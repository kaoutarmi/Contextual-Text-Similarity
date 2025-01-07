# Contextual Text Similarity with Sentence-BERT

This project demonstrates how to compute contextual text similarity using the **Sentence-BERT** model. The goal is to calculate the similarity between text pairs and find the most contextually similar sentences to a user-provided input sentence from a dataset.

## Features

- Uses **Sentence-BERT** (`all-MiniLM-L6-v2`) to compute embeddings for sentences.
- Calculates **cosine similarity** between embeddings to measure text similarity.
- Loads and evaluates text similarity using the **STS Benchmark dataset**.
- Finds the **top 5 most similar sentences** from the dataset for a given user input.

## Example

**Input:**
A person is playing a musical instrument

**Output:**
A person is playing a piano. (similarity: 0.7312)
A man plays a guitar. (similarity: 0.7006)
Someone is playing a piano. (similarity: 0.6983)
A man is playing a guitar. (similarity: 0.6930)
A man is playing a guitar. (similarity: 0.6930)


## Requirements

- Python 3.7+
- Libraries:
  - `sentence-transformers`
  - `datasets`
## How It Works
### Model Setup:

Loads the pre-trained all-MiniLM-L6-v2 model from the sentence-transformers library.
### Dataset Loading:

Loads the STS Benchmark dataset from Hugging Face's datasets library.
### Similarity Calculation:

Computes the cosine similarity between the embeddings of sentence pairs.
### Top 5 Similar Sentences:

Encodes the user-provided sentence and finds the 5 most similar sentences in the dataset.
## Usage
1-Clone the repository:
git clone https://github.com/yourusername/contextual-text-similarity.git
cd contextual-text-similarity
2-Run the script:
python script.py
3-Enter your input sentence when prompted.
## Applications
This project can be useful for:

Information retrieval systems.
Recommender systems for text-based content.
Enhancing chatbot contextual understanding.
