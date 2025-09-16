# Hate Speech Detection

This project explores different NLP techniques for classifying text into "hatespeech", "offensive", or "normal" categories. It compares traditional machine learning models with modern large language models using zero-shot and few-shot prompting.

## Project Structure

- `NLP_A2.ipynb`: Jupyter notebook containing the implementation of traditional ML models (e.g., Logistic Regression, SVM) with TF-IDF and Word2Vec embeddings.
- `NLP_A3.ipynb`: Jupyter notebook for hate speech classification using FLAN-T5 models with zero-shot and few-shot prompting techniques.
- `NLP_ass_train.tsv`, `NLP_ass_valid.tsv`, `NLP_ass_test.tsv`: Dataset files containing the text and corresponding labels.
- `GoogleNews-vectors-negative300.bin`: Pre-trained Word2Vec model from Google.

## Dataset

The dataset is provided in tab-separated files (`.tsv`). Each file contains two columns: "text" and "label". The labels are "hatespeech", "offensive", and "normal".

## Models and Methods

### Traditional Models (`NLP_A2.ipynb`)

This notebook focuses on traditional machine learning approaches.

- **Features**: TF-IDF and pre-trained Word2Vec embeddings (`GoogleNews-vectors-negative300.bin`) are used to represent the text data.
- **Models**: Logistic Regression and Support Vector Machines (SVM) are trained on the extracted features.

### Large Language Models (`NLP_A3.ipynb`)

This notebook utilizes the FLAN-T5 model for classification.

- **Models**: `google/flan-t5-base` and `google/flan-t5-small` are used.
- **Techniques**:
  - **Zero-shot learning**: The model is prompted to classify the text without any prior examples.
  - **Few-shot learning**: The model is provided with a few examples in the prompt to guide the classification.

## Setup

1.  Clone the repository.
2.  Install the required Python libraries:

    ```bash
    pip install pandas torch transformers scikit-learn jupyter gensim
    ```

3.  Download the pre-trained Word2Vec model (`GoogleNews-vectors-negative300.bin`) if it is not already present.

## Usage

1.  Launch Jupyter Notebook or Jupyter Lab.
2.  Open and run the cells in `NLP_A2.ipynb` to train and evaluate the traditional models.
3.  Open and run the cells in `NLP_A3.ipynb` to perform classification using the FLAN-T5 models.

The notebooks will load the data, process the text, train the models (where applicable), and print classification reports including accuracy and F1-scores.
