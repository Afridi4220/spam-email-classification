# Spam Email Classification

## Project Overview

This project is a machine learning system developed to classify text messages as **Spam** or **Ham (Not Spam)**.

The project uses Natural Language Processing (NLP) techniques to preprocess text and **TF-IDF (Term Frequency-Inverse Document Frequency)** to convert messages into numerical features. Two machine learning models were trained and evaluated: **Multinomial Naive Bayes** and **Logistic Regression**.

## Project Objective

The main objectives of this project are:

- Load and understand a labeled spam message dataset
- Explore the dataset and analyze spam/ham distribution
- Clean and preprocess text messages
- Convert text into numerical features using TF-IDF
- Train machine learning classification models
- Evaluate model performance using accuracy, precision, recall, F1-score, and confusion matrices
- Test the trained models on new messages
- Compare the performance of different models

## Dataset

The project uses a labeled SMS spam dataset containing messages classified as:

- **Ham** — legitimate messages
- **Spam** — unwanted or promotional messages

After removing duplicate messages, the dataset contained **5,169 messages**.

## Data Preprocessing

The text data was processed using the following steps:

1. Convert text to lowercase
2. Remove non-alphanumeric characters
3. Remove English stopwords
4. Split the dataset into training and testing sets
5. Convert text into numerical features using TF-IDF

The dataset was divided using an **80/20 stratified train-test split**.

## Machine Learning Models

### 1. Multinomial Naive Bayes

Multinomial Naive Bayes is commonly used for text classification because it works well with word-frequency-based features such as TF-IDF.

**Accuracy: 96.23%**

### 2. Logistic Regression

Logistic Regression was used as a second classification model to compare its performance with Naive Bayes.

**Accuracy: 95.07%**

## Model Performance

| Model | Accuracy |
|---|---:|
| Multinomial Naive Bayes | 96.23% |
| Logistic Regression | 95.07% |

The models were evaluated using the same training and testing data.

## Evaluation Metrics

The following evaluation techniques were used:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

These metrics provide a more detailed view of classification performance than accuracy alone.

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- TF-IDF
- Natural Language Processing (NLP)

## Project Structure

```text
spam-email-classification/
│
├── data/
│   └── spam.csv
│
├── notebooks/
│   └── spam_classification.ipynb
│
└── README.md
