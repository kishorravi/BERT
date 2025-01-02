# IMDb Sentiment Analysis with BERT

## Authors

- [@Mr_Kishor_Ravikumar](mailto:ece.kishor@gmail.com)

## Overview

IMDb Sentiment Analysis using **BERT** (Bidirectional Encoder Representations from Transformers) demonstrates the power of state-of-the-art natural language processing (NLP) models. This project leverages a pretrained BERT model to classify IMDb movie reviews as either positive or negative sentiments. The model is fine-tuned and evaluated on a subset of the IMDb dataset.

## Key Features

- **Pretrained Model**: Uses the `bert-base-uncased` model from Hugging Face Transformers.
- **Dataset**: IMDb movie reviews, a benchmark dataset for sentiment analysis.
- **Metrics Evaluated**:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - Cohen's Kappa
- **Batch Processing**: Efficient data handling using PyTorch's `DataLoader`.

## Dataset

The **IMDb dataset** is a well-known collection of movie reviews with binary sentiment labels (positive or negative). For this project, 10% of the test set is used for evaluation:

```python
dataset = load_dataset('imdb', split='test[:10%]')
