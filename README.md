# 🛒 Amazon Product Review Sentiment Analysis

*A Natural Language Processing (NLP) Project using TF-IDF and Logistic Regression*

---

## 📖 **Project Overview**

This project focuses on analyzing **Amazon product reviews** to automatically determine whether a review expresses a **positive** or **negative** sentiment.

With the exponential growth of online reviews, manually interpreting customer feedback has become impractical. This project leverages **Machine Learning** and **Natural Language Processing (NLP)** techniques to extract insights from text data, helping businesses make **data-driven decisions** about products, services, and customer satisfaction.

---

## 🎯 **Objectives**

* 🧹 Clean and preprocess raw review text.
* 🔤 Convert text into numerical features using **TF-IDF Vectorization**.
* 🤖 Train a **Logistic Regression** model to classify sentiments.
* 📈 Evaluate the model using accuracy and confusion matrix.
* ☁️ Visualize frequent words in positive and negative reviews with **Word Clouds**.

---

## 🧠 **Technologies Used**

| Category          | Tools / Libraries                                                          |
| ----------------- | -------------------------------------------------------------------------- |
| **Language**      | Python 🐍                                                                  |
| **Libraries**     | Pandas, NumPy, Matplotlib, Scikit-learn, WordCloud, NLTK                   |
| **Techniques**    | Text Cleaning, Stopword Removal, TF-IDF Vectorization, Logistic Regression |
| **Visualization** | Word Cloud, Confusion Matrix                                               |

---

## 📊 **Dataset Information**

* **Source:** Amazon Product Reviews Dataset
* **Total Records:** 25,000
* **Columns:**

  * `Review`: The text content of customer reviews
  * `Sentiment`: Numeric sentiment labels (1–5 stars converted to binary classes)

| Sentiment Score | Meaning         | Label Used |
| :-------------: | :-------------- | :--------- |
|       1–3       | Negative Review | 0          |
|       4–5       | Positive Review | 1          |

---

## ⚙️ **Workflow / Methodology**

1. **Data Preprocessing**

   * Removed null entries
   * Lowercased text
   * Removed stopwords
   * Tokenized and joined cleaned words

2. **Feature Extraction**

   * Used **TF-IDF Vectorizer** (`max_features=2500`) to convert text into numerical representation.

3. **Model Building**

   * Split dataset into **75% training** and **25% testing** sets.
   * Trained **Logistic Regression** model on TF-IDF features.

4. **Evaluation**

   * Calculated model **accuracy** and generated **confusion matrix**.
   * Visualized results using Matplotlib.

5. **Visualization**

   * Created **Word Clouds** for positive and negative sentiment words.

## 🧩 **Model Results**

| Metric                   |   Value  |
| :----------------------- | :------: |
| **Accuracy**             | **~83%** |
| **True Positives (TP)**  |   1787   |
| **True Negatives (TN)**  |   3310   |
| **False Positives (FP)** |    408   |
| **False Negatives (FN)** |    745   |

✅ The Logistic Regression model achieved **83% accuracy**, successfully distinguishing positive and negative sentiments with good reliability.
