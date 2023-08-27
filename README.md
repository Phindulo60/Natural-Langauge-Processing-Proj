# Natural Language Processing Projects


Repository maintained by [@Phindulo60](https://github.com/Phindulo60)

## Overview

This repository contains projects related to Natural Language Processing (NLP). The main project focuses on text classification using various models and feature extraction techniques.

## Dataset

The dataset consists of text messages labeled as either `0` or `1`. The dataset is split into training, testing, and validation sets:

- **Training set**: 3102 entries
- **Testing set**: 1034 entries
- **Validation set**: 1035 entries

Each entry contains a subject line followed by the message content.

## Preprocessing

The data undergoes several preprocessing steps:

1. Conversion to lowercase
2. Tokenization
3. Removal of stop words, digits, and punctuation
4. Stemming using the Porter Stemmer

## Models

### Model1: Standard Naive Bayes

This model uses the entire feature set for training and achieved an accuracy of approximately 96.91% on the validation set.

### Model2: Naive Bayes with Top 10 Frequent Words

This model is trained using only the 10 most frequent words as features. It achieved an accuracy of approximately 79.90% on the validation set.

### Model3: Naive Bayes with Top 100 Frequent Words

This model uses the 100 most frequent words as features and achieved an accuracy of approximately 86.28% on the validation set.

### Model4: Naive Bayes excluding Top 100 Frequent Words

For this model, the top 100 most frequent words were removed from the feature set. The model achieved an accuracy of approximately 96.91% on the validation set.

### Model5: Naive Bayes using Subject Line

This model uses only the subject line of the text messages as the feature set. It achieved an accuracy of approximately 83.29% on the validation set.

## Evaluation Metrics

For each model, the following metrics were calculated:

- **Accuracy**
- **F1 Score**
- **Precision**
- **Recall**

Detailed results for each model can be found in the Jupyter notebook `1832463.ipynb`.

## Dependencies

The project uses the following libraries:

- nltk
- numpy
- pandas
- sklearn
- seaborn
- matplotlib

## How to Run

1. Clone the repository.
2. Install the required libraries.
3. Open the `1832463.ipynb` notebook in Jupyter.
4. Run the cells to train the models and see the results.


