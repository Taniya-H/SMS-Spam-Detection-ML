# 📧Email Spam Detection ML

## 🚀 Project Description

This project builds a Machine Learning model to classify text messages as **Spam** or **Ham (Not Spam)** using Natural Language Processing techniques.

It demonstrates a complete ML pipeline:

Data preprocessing -> Feature extraction -> Model training -> Evaluation -> Prediction

The model uses **TF-IDF Vectorization** and **Logistic Regression**, achieving high accuracy with strong precision-recall balance.

---

## 🎯 Objectives

- Understand text preprocessing for NLP tasks  
- Convert raw text into numerical vectors using TF-IDF  
- Train a supervised classification model  
- Evaluate performance using proper metrics  
- Build an end-to-end ML workflow  

---

## 📂 Dataset Used

The dataset consists of labeled messages:

- **Spam** -> Promotional or unwanted messages  
- **Ham** -> Legitimate messages  

Each entry contains:
- Text message  
- Corresponding label  

The dataset was split into training and testing sets to ensure fair evaluation.

---

## 🛠 Technologies & Tools Used

- Python  
- Pandas  
- Scikit-learn  
- Google Colab  

Key Components:
- `TfidfVectorizer`
- `LogisticRegression`
- `train_test_split`
- `classification_report`
- `confusion_matrix`

---

## 🤖 Model Details

### 1. Text Vectorization (TF-IDF)

TF-IDF converts text into numerical feature vectors by:

- Giving importance to meaningful words  
- Reducing weight of common words  
- Making text machine-readable  

---

### 2. Classification Model

Logistic Regression was used with:

- `class_weight='balanced'`  
- `max_iter=2000`  

It is efficient, interpretable, and performs well for binary text classification tasks.

---

### 3. Evaluation Metrics

The model was evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  

Example Performance:

- Accuracy: ~97.7%  
- Spam Precision: ~0.92  
- Spam Recall: ~0.90  

Low false positives and false negatives indicate strong classification capability.

---

## 🔎 Prediction Logic

1. User inputs a message  
2. Text is transformed using trained TF-IDF vectorizer  
3. Vector is passed into Logistic Regression model  
4. Model predicts:
   - `1` -> Spam  
   - `0` -> Ham  
5. Output is returned to the user  

---

## 🧩 Project Workflow

1. Load dataset  
2. Preprocess text data  
3. Split into train and test sets  
4. Apply TF-IDF vectorization  
5. Train Logistic Regression model  
6. Evaluate model performance  
7. Generate predictions  
---

## 🗂 Project Structure
```bash
Spam-Detection-Using-TFIDF-and-LogisticRegression/
│
├── data/
│ └── spam.csv
│
├── notebook/
│ └── spam_detection.ipynb
└── README.md


