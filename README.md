# Spam-email-SMS-Identifier

An end-to-end **Machine Learning project** that classifies SMS messages as **Spam** or **Ham** (not spam) with high accuracy.

---

## 📌 Project Overview

This project builds a robust SMS Spam Detection system using **Natural Language Processing (NLP)** and **Machine Learning**. The model is trained on the classic SMS Spam Collection dataset and achieves excellent performance using **Multinomial Naive Bayes** with **TF-IDF vectorization**.

**Key Highlights:**
- Thorough data cleaning and EDA
- Text preprocessing (lowercasing, tokenization, removing stopwords, stemming)
- Multiple ML models compared
- Best model saved as a pickle file for easy deployment

---

## 🛠️ Technologies Used

- **Python**
- **Pandas** & **NumPy**
- **NLTK** (for text preprocessing)
- **Scikit-learn** (TF-IDF + ML models)
- **Matplotlib** & **Seaborn** (EDA)
- **Pickle** (model deployment)

---

## 📊 Dataset

- **Source**: Standard SMS Spam Collection Dataset (`spam.csv`)
- **Classes**: 
  - `Ham` (0) → 87.37%
  - `Spam` (1) → 12.63%
- Total messages after cleaning: **5,169**

---

## 🚀 Features

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Text Transformation (custom `transform_text` function)
- TF-IDF Vectorization (max 3000 features)
- Model Training & Comparison (11+ algorithms)
- Best Model: **Multinomial Naive Bayes**

---

## 📈 Model Performance

| Algorithm       | Accuracy   | Precision |
|-----------------|------------|---------|
| Multinomial NB  | **97.29%** | **99.16%** |
| Random Forest   | 97.20%     | 99.15%  |
| Extra Trees     | 97.97%     | **100%** |
| SVC             | 97.58%     | 94.78%  |

> **Best Model Chosen**: `MultinomialNB` (Excellent balance of accuracy + precision)

---

## 📁 Repository Structure

SMS-Spam-Classifier/
├── sms spam classifier.ipynb     # Main Jupyter Notebook
├── spam.csv                      # Dataset
├── Transform.pkl                 # Text preprocessor
├── vectorizer.pkl                # TF-IDF Vectorizer
├── model.pkl                     # Trained Model (MultinomialNB)
├── README.md
text

---

## 🏃‍♂️ How to Run
Clone the repository:
   git clone https://github.com/yourusername/SMS-Spam-Classifier.git

Install dependencies:Bashpip install pandas numpy nltk scikit-learn matplotlib seaborn
Open the notebook:Bashjupyter notebook "sms spam classifier.ipynb"
For Prediction (after running the notebook):
Load the saved pickle files (model.pkl, vectorizer.pkl, Transform.pkl)
