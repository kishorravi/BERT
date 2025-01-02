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
The IMDb dataset is a well-known collection of movie reviews with binary sentiment labels (positive or negative). For this project, 10% of the test set is used for evaluation:

## Dataset Details
- **Source:** IMDb dataset via Hugging Face Datasets library.
- **Classes:** Binary sentiment labels - Positive and Negative.
- **Preprocessing:**
  -Tokenized with AutoTokenizer.
  -Truncated and padded to a maximum sequence length of 512 tokens.
## Methodology

-**1.Preprocessing:**
Reviews are tokenized and prepared for input by applying truncation and padding to ensure consistent input lengths.
-**2.Model:**
The bert-base-uncased model is fine-tuned for binary classification, predicting either positive or negative sentiments.
-**3.Evaluation:**
Model predictions are compared against true labels, and metrics such as accuracy, precision, recall, F1-score, and Cohen's Kappa are calculated.
##Results

The following metrics summarize the model's performance:

Metric	Value
Accuracy	86.00%
Precision	87.50%
Recall	83.50%
F1-Score	85.45%
Cohen's Kappa	0.72
Example Misclassifications
Review ID	True Sentiment	Predicted Sentiment
review_0456	Positive	Negative
review_0321	Negative	Positive

