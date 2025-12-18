# 💬 Sentiment Analysis using NLP

Sentiment Analysis is a Natural Language Processing (NLP) project that analyzes user reviews and classifies them into **Positive**, **Neutral**, or **Negative** sentiments. This project focuses on understanding customer opinions, identifying common concerns, and improving user experience using machine learning techniques.

---

## 📌 Problem Statement

User reviews contain valuable feedback but are unstructured and difficult to analyze manually.  
This project builds an automated sentiment analysis system to extract meaningful insights from textual reviews using NLP and Machine Learning.

---

## 📂 Dataset

- ChatGPT-style user reviews dataset
- Columns:
  - `review` – User review text
  - `rating` – Numeric rating (1–5)
  - `platform` – Review source
- Sentiment is derived from ratings:
  - 1–2 → Negative
  - 3 → Neutral
  - 4–5 → Positive

---

## 🔧 Data Preprocessing

- Text cleaning and normalization
  - Lowercasing
  - Removing punctuation & special characters
  - Stopword removal
  - Lemmatization
- Handling missing values
- Feature engineering (review length)
- Dataset balancing (optional)

---

## 📊 Exploratory Data Analysis (EDA)

- Sentiment distribution analysis
- Review length analysis
- Rating vs sentiment trends
- Platform-wise review analysis
- Word frequency visualization using:
  - Word Clouds
  - Histograms
  - Count plots

---

## 🤖 Feature Engineering

- Text vectorization using:
  - TF-IDF (primary approach)
  - Tokenization & Padding (for LSTM)
- N-grams for improved context capture

---

## 🧠 Models Used

- Logistic Regression
- Multinomial Naive Bayes
- Random Forest
- LSTM (Deep Learning)

---

## 📈 Model Evaluation

Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Special handling is applied for LSTM outputs by converting probabilities into class labels.

---

## 🚀 Deployment

An interactive **Streamlit dashboard** is built to:
- Accept user review input
- Predict sentiment in real time
- Display model evaluation metrics
- Visualize prediction distribution and confusion matrix

---

## 💾 Model Serialization

- TF-IDF Vectorizer saved using `pickle`
- Machine Learning models saved using `pickle`
- LSTM model saved using `.h5` format

