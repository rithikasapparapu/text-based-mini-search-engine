# Mini Search Engine for Lyrics Dataset

## Project Overview

This project implements a simple search engine for a small dataset of song lyrics. The search engine utilizes various information retrieval techniques, including tokenization, indexing, and ranked retrieval models. The goal of the project is to retrieve and rank relevant song lyrics based on user queries.

## Features

### Tokenization:
- **Stemming**: Reduces words to their root form to improve matching.
- **Case-folding**: Converts all text to lowercase for consistency.
- **Stop-word Removal**: Filters out common words (e.g., "the", "and") that do not contribute meaningfully to search.

### Indexing:
- Builds an **inverted index** to store and retrieve song lyrics efficiently based on search queries.

### Retrieval Models:
- **Vector Space Model (VSM)**: Ranks documents (song lyrics) by their vector representations in a high-dimensional space.
- **BM25**: An advanced ranking function that uses Term Frequency (TF), Inverse Document Frequency (IDF), and document length normalization.
- **Boolean Retrieval**: A model that retrieves documents based on the presence or absence of query terms using Boolean operators (AND, OR).
- **ColBERT**: A deep learning-based retrieval method using BERT embeddings for more advanced ranking.

The project implements and compares the performance of the above retrieval models, providing insights into their relative strengths and weaknesses for lyrics search.

## Dataset

We use the **Genius Lyrics Dataset**, which is a subset of 200 song lyrics. The dataset is stored in a JSON Lines file (`lyrics_200.jl`), where each line contains the lyrics of one song.
