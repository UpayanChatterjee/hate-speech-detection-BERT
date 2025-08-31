# NLP Assignments

This repository contains the work for two NLP assignments. The primary tasks involve text classification and sequence labeling.

## Assignment 2: Text Classification

`NLP_A2.ipynb` contains the code for a text classification task. The goal is to classify text into different categories. The notebook covers the entire process from data loading and preprocessing to model training and evaluation.

### Model
A transformer-based model is used for this task. The notebook details the model architecture and training process.

### Results
The model's performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. The notebook includes a confusion matrix and a classification report to summarize the results.

## Assignment 3: Sequence Labeling

`NLP_A3.ipynb` and `A3.ipynb` focus on a sequence labeling task, likely Named Entity Recognition (NER). The objective is to assign a label to each token in a sequence of text.

### Model
Similar to Assignment 2, a transformer-based model is employed for this sequence labeling task. The notebook provides a detailed explanation of the model and its implementation.

### Results
The performance of the sequence labeling model is presented in the notebook, including metrics like accuracy and a classification report for each entity type.

## Data
The dataset for these assignments is provided in the following files:
- `NLP_ass_train.tsv`
- `NLP_ass_valid.tsv`
- `NLP_ass_test.tsv`

## Usage
To reproduce the results, you can run the Jupyter notebooks. The notebooks are self-contained and include all the necessary code and outputs.

1.  **Assignment 2:** Open and run the cells in `NLP_A2.ipynb`.
2.  **Assignment 3:** Open and run the cells in `NLP_A3.ipynb` or `A3.ipynb`.

Make sure you have the required libraries installed. The notebooks use common NLP and deep learning libraries such as PyTorch, Transformers, and scikit-learn.
