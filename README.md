# 🎓 Topic Modeling & Aspect-Based Sentiment Analysis Using LDA & Naive Bayes

This repository contains the implementation of topic modeling and aspect-based sentiment analysis (ABSA) on **ChatGPT user reviews from Google Play Store**. This project was conducted as part of my undergraduate thesis, aiming to identify key aspects of user experience and their associated sentiments using Natural Language Processing (NLP) techniques.

---

## 📌 Background

With the exponential growth in the number of ChatGPT users, it's crucial to understand what aspects of the application contribute to its popularity and what issues users are facing. Manually analyzing thousands of user reviews is time-consuming, hence the need for automated text analysis.

This study uses:
- **Latent Dirichlet Allocation (LDA)** for topic modeling to extract user concern aspects.
- **Multinomial Naive Bayes** for performing sentiment classification on those aspects.

---

## 🎯 Objectives

- 🧠 Implement **LDA** to identify major topics (aspects) from ChatGPT user reviews.
- 💬 Implement **Aspect-Based Sentiment Analysis (ABSA)** using **Naive Bayes** and compare with **SVM**.
- 📊 Identify dominant user opinions—positive or negative—for each aspect.
- 🤖 Understand user concerns and expectations in adopting AI technologies.

---

## 🛠️ Methodology

### 1. Data Collection
- Source: Google Play Store reviews for ChatGPT app.
- Preprocessing steps include: lowercasing, tokenization, stopword removal, and lemmatization.

### 2. Topic Modeling with LDA
- LDA trained with:
  - **Iterations**: 100
  - **Number of Topics**: 10
- Best coherence score: **0.524**
- Final 5 extracted topics:
  - **Usability**
  - **Response**
  - **Features**
  - **Functionality**
  - **Satisfaction**

### 3. Aspect-Based Sentiment Analysis
- Classifier: **Multinomial Naive Bayes**
- Evaluation: Data split ratios of 75:25, 80:20, and 90:10
- Best performance at **80:20 split**, avoiding overfitting

---

## 📈 Results

| Aspect        | Accuracy |
|---------------|----------|
| Usability     | 85.1%    |
| Response      | 89.5%    |
| Features      | 89.2%    |
| Functionality | 89.7%    |
| Satisfaction  | 92.8%    |

- Positive sentiments **dominate** across all aspects.
- **Usability** had the most positive feedback: users found the app easy to use.
- **Response** had the most negative sentiment, mainly due to complaints about response speed and accuracy.

---

## 🚧 Limitations

- The model struggles to classify **negative sentiments** due to **class imbalance**.
- Low precision, recall, and F1-score for negative labels in some aspects.

---

## 📌 Conclusion

This project demonstrates how NLP and machine learning can be used to:
- Identify what users value most in ChatGPT (usability, features, etc.)
- Understand satisfaction and pain points at a granular aspect level
- Support future product improvements through user voice analysis

---


---

## 🧠 Tech Stack

- Python
- Scikit-learn
- Gensim
- NLTK / SpaCy
- Pandas & NumPy
- Matplotlib & Seaborn

---

---

## 🎞️ Presentation Slides

You can view the full presentation slide deck here:

📎 [Sentiment Analysis of ChatGPT Application Users (Google Drive)](https://drive.google.com/file/d/1Ievpo9NPNtFPJcMLIb2KPyuSA2QHN80Q/view?usp=sharing)

---


