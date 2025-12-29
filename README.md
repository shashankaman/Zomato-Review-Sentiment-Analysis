# 🍽️ Zomato Reviews Sentiment Analysis

## 📌 Project Overview

This project analyzes customer reviews from **Zomato** using **Natural Language Processing (NLP)** techniques.
The objective is to classify reviews into **Positive, Negative, and Neutral** sentiments and derive **actionable business insights** that help understand customer satisfaction and service quality.

The project demonstrates how **unstructured text data** can be transformed into **data-driven insights** for business decision-making.

---

## 🎯 Business Problem

Food delivery platforms receive thousands of customer reviews every day.
Manually analyzing this feedback is inefficient, subjective, and not scalable.

### Key Questions Addressed:

* What is the overall customer sentiment?
* Are customers generally satisfied or dissatisfied?
* Do written reviews align with customer ratings?
* How can textual feedback be converted into business insights?

---

## 🗂️ Dataset

The dataset consists of real-world customer feedback collected from Zomato and includes:

| Column   | Description                 |
| -------- | --------------------------- |
| `Id`     | Unique review identifier    |
| `Rating` | Customer rating (1–5 stars) |
| `Review` | Customer review text        |

The combination of **ratings and review text** allows both sentiment analysis and validation of results.

---

## 🔧 Tools & Technologies Used

* **Python**
* **Pandas & NumPy** – data manipulation
* **TextBlob** – NLP-based sentiment analysis
* **Matplotlib & Seaborn** – data visualization
* **Regular Expressions (Regex)** – text preprocessing

---

## 🧹 Data Cleaning & Preprocessing

To improve sentiment accuracy, the following preprocessing steps were applied:

* Converted text to lowercase
* Removed special characters, numbers, and emojis
* Handled missing values safely
* Removed empty reviews after cleaning

These steps help reduce noise and standardize text for NLP analysis.

---

## 🧠 Sentiment Analysis Approach

* Used **TextBlob polarity score** to determine sentiment
* Polarity ranges from `-1` (negative) to `+1` (positive)

### Sentiment Classification Rules:

* **Positive** → Polarity > 0
* **Negative** → Polarity < 0
* **Neutral** → Polarity = 0

TextBlob was chosen for its simplicity, interpretability, and suitability for business-focused analysis without requiring labeled training data.

---

## 📊 Sentiment Distribution

* The majority of customer reviews are **positive**
* Indicates overall customer satisfaction
* Results are visualized using bar charts for easy interpretation by both technical and non-technical stakeholders

---

## ✅ Rating-Based Sentiment Mapping (Validation)

Customer ratings were converted into sentiment categories:

* **4–5 stars** → Positive
* **3 stars** → Neutral
* **1–2 stars** → Negative

This step provides a **ground truth benchmark** to validate NLP-based sentiment classification.

---

## 🔍 Rating vs NLP Sentiment Comparison

* Compared rating-based sentiment with NLP-based sentiment using cross-tabulation
* Visualized alignment using bar charts

### Key Findings:

* High ratings mostly align with **Positive** sentiment
* Low ratings strongly align with **Negative** sentiment
* Strong alignment confirms the **reliability of the NLP approach**

---

## 📌 Key Insights

* Majority of customer reviews are positive, indicating overall satisfaction
* Negative reviews highlight delivery delays and food quality issues
* NLP-based sentiment strongly aligns with customer ratings
* Unstructured customer feedback can be transformed into actionable business insights

---

## 🧠 Learning Outcomes

* Practical implementation of NLP techniques
* Text preprocessing and sentiment classification
* Business-oriented data analysis
* Validation of NLP results using customer ratings
* Translating unstructured text into meaningful insights

---

## ⚠️ Limitations & Future Improvements

### Current Limitations:

* TextBlob may misclassify sarcasm
* Emojis and slang are ignored during preprocessing

### Future Enhancements:

* Use VADER for social media–style text
* Apply machine learning–based sentiment models
* Emoji sentiment mapping
* Aspect-based sentiment analysis (food, delivery, service)

---

## 📌 Conclusion

This project demonstrates how NLP can be effectively used to analyze customer feedback and support **data-driven decision-making**.
By combining sentiment analysis with rating-based validation, the project ensures insights are both **interpretable and reliable**.
