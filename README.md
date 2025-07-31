## Fake News Classifier

A machine learning project to detect whether a news article is **real** or **fake** using Natural Language Processing (NLP). This beginner-friendly project uses a logistic regression model trained on labeled news data.

---

## Overview

Fake news spreads misinformation and confusion. This project aims to classify news articles as **fake** or **real** using their content (title and body text).  
It is built with:
- Python 🐍
- Pandas & NumPy for data handling
- Scikit-learn for ML model and evaluation
- TF-IDF Vectorizer for text representation

---

## Dataset

We used two CSV files:  

### `True.csv.zip`
- Contains real news articles from verified sources.
- Columns: `title`, `text`, `subject`, `date`.

### `Fake.csv.zip`
- Contains fake/misleading articles from untrustworthy sources.
- Columns: `title`, `text`, `subject`, `date`.

The files are labeled (`1` = Real, `0` = Fake) and merged for training/testing.

---

## 🛠️ How It Works

1. **Load and combine** real and fake news datasets.
2. **Clean the data** (drop missing values, select relevant columns).
3. **Label** real as `1`, fake as `0`.
4. **Split** the dataset into training and testing sets.
5. **Convert** text into numbers using `TfidfVectorizer`.
6. **Train** a Logistic Regression model.
7. **Evaluate** with accuracy, confusion matrix, and classification report.

---
