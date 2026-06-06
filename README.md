# 📰 Fake News Detection System

> *"Empowering social networks and users to distinguish truth from misinformation."*

![Model](https://img.shields.io/badge/Model-Passive_Aggressive_Classifier-blue)
![Backend](https://img.shields.io/badge/Backend-Flask-lightgrey)
![Accuracy](https://img.shields.io/badge/Accuracy-96%25-success)

## 📖 Overview
This project is a comprehensive machine learning web application designed to detect fake news in real-time. By utilizing natural language processing (NLP) and a continuously updating classification model, the system analyzes the content of news articles to classify them as either reliable or unreliable. 

The intended application is to provide visibility weights for social media platforms, allowing them to confidently identify and reduce the spread of stories from recurring fake news sources.

---

## 🧠 Core Features & Mechanics

### ⚡ 1. Real-Time Online Learning
* **Continuous Updates:** The system utilizes a **Passive Aggressive Classifier (PAC)**, which continuously updates its model as new data arrives.
* **High Efficiency:** This online learning algorithm makes the model highly efficient and exceptionally well-suited for real-time fake news detection.
* **Proven Performance:** The PAC model achieved a 96% accuracy rate during evaluation.

### 🛡️ 2. Source-Based Misclassification Tolerance
* **Strategic Focus:** Rather than solely analyzing isolated articles, the system focuses on identifying fake news *sources* by analyzing multiple articles originating from them.
* **High Confidence Predicting:** Once a source is flagged, the model can predict future fake articles from that producer with high confidence, safely widening the system's misclassification tolerance.

### 🌐 3. Interactive Web Interface
* **Instant Validation:** Users can input news headlines directly into a responsive web interface to uncover the truth and validate authenticity instantly.
* **Seamless Integration:** Built on **Flask**, the application seamlessly bridges the Python machine learning logic with an interactive HTML/CSS frontend.

---

## 📊 Datasets
The model is trained and tested on comprehensive data from Kaggle:
* **train.csv:** Contains full attributes for training, including `id`, `title`, `author`, `text`, and a binary `label` (1 for unreliable, 0 for reliable).
* **test.csv:** Contains identical attributes for testing purposes, excluding the reliable/unreliable label.

---

## 🛠️ Tech Stack
* **Frontend:** HTML, CSS (Outfit & Roboto fonts)
* **Backend:** Python, Flask
* **Machine Learning:** Scikit-Learn (PassiveAggressiveClassifier, TfidfVectorizer)
* **Natural Language Processing:** NLTK (WordNetLemmatizer, Stopwords)
* **Data Processing:** Pandas, NumPy, Regular Expressions (re)
