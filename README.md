## Fake News Classifier

A machine learning project to detect whether a news article is **real** or **fake** using Natural Language Processing (NLP). This beginner-friendly project uses a logistic regression model trained on labeled news data.

---

## Overview

Fake news spreads misinformation and confusion. This project aims to classify news articles as **fake** or **real** using their content (title and body text).  
It is built with:
- Python 
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
## How to run:

1. Clone the Repository
git clone https://github.com/ziziiprogrammingFake-News-Classifier.git
cd Fake-News-Classifier

2. Create & Activate Virtual Environment (optional but recommended)
python -m venv venv
source venv/bin/activate

3. Install Dependencies
pip install -r requirements.txt
pandas
numpy
scikit-learn
nltk
jupyter

4. Download NLTK Data (if needed)
If your code uses NLTK, add this once in your notebook or script:
python
Copy
Edit
import nltk
nltk.download('stopwords')
nltk.download('punkt')

5. Run the Classifier
Option A: If using Jupyter Notebook
jupyter notebook Fake_News_Classifier.ipynb

Option B: If using Python Script
python Fake_News_Classifier.py

6. Ensure the Dataset is Available:
Your dataset (e.g., train.csv) should be in the project folder or as specified in the code. If needed, provide the link to download it in your README.

7. Expected Output:
The model should print accuracy, confusion matrix, and classification report.

