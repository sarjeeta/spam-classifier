# Spam Classifier using Machine Learning and NLP

## Overview

This project builds a Spam Message Classifier using Natural Language Processing (NLP) and Machine Learning techniques. The model classifies SMS messages as either **Spam** or **Ham (Not Spam)** using text preprocessing, TF-IDF vectorization, and classification algorithms.

The project demonstrates a complete NLP pipeline from raw text processing to model evaluation.

---

## Dataset

The project uses the **SMS Spam Collection Dataset**, containing 5,572 SMS messages labeled as:

* Ham (Not Spam)
* Spam

### Dataset Statistics

| Class          | Count |
| -------------- | ----- |
| Ham            | 4825  |
| Spam           | 747   |
| Total Messages | 5572  |

---

## Project Workflow

1. Data Loading
2. Data Exploration
3. Data Cleaning
4. Text Preprocessing
5. Feature Engineering
6. TF-IDF Vectorization
7. Train-Test Split
8. Model Training
9. Model Evaluation
10. Model Comparison

---

## Exploratory Data Analysis

Performed:

* Class distribution analysis
* Message length analysis
* Missing value check
* Spam vs Ham visualization

### Key Observation

* Spam messages tend to be longer than Ham messages.
* Significant overlap exists between the two classes.
* Message length alone is not sufficient for classification.

---

## Text Preprocessing

The following preprocessing steps were applied:

* Convert text to lowercase
* Remove punctuation
* Remove stopwords
* Tokenization
* Text normalization

### Example

Original Message:

Congratulations!!! You won a FREE iPhone.

Processed Message:

congratulations free iphone

---

## Feature Engineering

Text messages were converted into numerical representations using:

### TF-IDF Vectorization

This converts text into machine-readable numerical vectors while assigning higher importance to informative words.

Feature Matrix Shape:

* Training Data: (4457, 8288)
* Testing Data: (1115, 8288)

---

## Models Implemented

### 1. Multinomial Naive Bayes

A probabilistic classification algorithm widely used for text classification tasks.

### 2. Logistic Regression

A linear classification algorithm commonly used for binary classification problems.

---

## Model Performance

| Model               | Accuracy | Precision | Recall | F1 Score |
| ------------------- | -------- | --------- | ------ | -------- |
| Naive Bayes         | 97.13%   | 100.00%   | 78.52% | 87.97%   |
| Logistic Regression | 96.05%   | 97.30%    | 72.48% | 83.08%   |

### Best Model

**Multinomial Naive Bayes** achieved the best overall performance.

---

## Confusion Matrix (Naive Bayes)

|             | Predicted Ham | Predicted Spam |
| ----------- | ------------- | -------------- |
| Actual Ham  | 966           | 0              |
| Actual Spam | 32            | 117            |

### Interpretation

* No Ham messages were incorrectly classified as Spam.
* The model achieved 100% precision.
* Some Spam messages were missed, resulting in lower recall.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* NLTK
* Jupyter Notebook

---

## Project Structure

spam-classifier/

├── README.md

├── requirements.txt

├── notebooks/spam_classifier.ipynb

├── images/

│   ├── spam_distribution.png

│   └── message_length_histogram.png

└── .gitignore

---

## Skills Demonstrated

* Natural Language Processing (NLP)
* Text Preprocessing
* Feature Engineering
* TF-IDF Vectorization
* Classification Algorithms
* Model Evaluation
* Data Visualization
* Machine Learning with Scikit-learn

---

## Future Improvements

* Hyperparameter Tuning
* Cross Validation
* N-Gram Features
* Word Embeddings
* Deep Learning Models (LSTM, GRU)
* Transformer-based Models (BERT)
* Streamlit Web Application Deployment

---

## Author

Sarjeeta 
