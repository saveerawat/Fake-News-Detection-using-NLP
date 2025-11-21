# Fake-News-Detection-using-NLP
A machine learning project that classifies news articles as True or Fake using text analysis on ~40,000 Kaggle articles.

**1. Project Overview**

This project builds a Fake News Detection model using Logistic Regression. It evaluates prediction performance using:<br>
1. Title only<br>
2. Content only<br>
3. Title + Content (combined)

**2. Dataset**

Used two Kaggle datasets:<br>
True.csv – Real news<br>
Fake.csv – Fake news

A binary label was added: 1 → True news, 0 → Fake news

**3. Preprocessing**

Removed stopwords, short tokens, and non-text characters using Gensim, spaCy, and NLTK
<br>Standardized subject labels (e.g., politics → PoliticsNews)
<br>Tokenized & cleaned text with gensim.utils.simple_preprocess()

**4. Model**

Used Logistic Regression with CountVectorizer for feature extraction.

**5. Result**

1.	Title Only	94% accuracy
2.	Content Only	99% accuracy
3.	Title+Content	99.6% accuracy
