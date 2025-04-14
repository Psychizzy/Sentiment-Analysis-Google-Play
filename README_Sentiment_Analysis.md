# 📊 Sentiment Analysis of Google Play Store App Reviews

> Developed by **Ajayi Oluwaseyi** | April 2025  
> 📧 Oluwaseyi1414@gmail.com

---

## 📘 Project Overview

This project aims to analyze user feedback from Google Play Store apps and classify each review as **Positive**, **Neutral**, or **Negative** using **Natural Language Processing (NLP)** and **Machine Learning (ML)** techniques. The goal is to uncover insights into public opinion, customer experience, and app performance.

---

## 📂 Dataset Summary

- **`apps.csv`**: Metadata for over 9,000 apps including category, rating, installs, and price.
- **`user_reviews.csv`**: Pre-labeled app reviews with sentiment labels and polarity scores.
- Merged using the **`App`** column to enrich the review data with app-level metadata.

---

## 🔧 Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python | Programming Language |
| Pandas, NumPy | Data Processing |
| Scikit-learn | ML Modeling & Evaluation |
| Seaborn, Matplotlib | Data Visualization |
| TF-IDF | Feature Engineering |
| Jupyter Notebook | Development Environment |

---

## 🧠 Key Steps

### ✅ Data Cleaning
- Handled missing values in ratings, reviews, sizes
- Converted review text into numerical features using **TF-IDF**

### ✅ Sentiment Classification
- **Model 1: Naive Bayes**  
  - Accuracy: ~74%  
  - Struggled with Neutral class

- **Model 2: Logistic Regression**  
  - Accuracy: ~90%  
  - High F1-scores for all sentiment classes  
  - Chosen as final model

### ✅ Visualizations
- **Sentiment by App Type** (Free vs Paid)
- **Sentiment by App Category**
- **Sentiment by Star Rating**

---

## 📈 Model Evaluation

| Sentiment | Precision | Recall | F1-Score |
|-----------|-----------|--------|----------|
| Negative  | 0.90      | 0.78   | 0.84     |
| Neutral   | 0.84      | 0.81   | 0.82     |
| Positive  | 0.91      | 0.95   | 0.93     |

✅ Final model achieved **~90% accuracy** using Logistic Regression.

---

## 🖼️ Sample Visuals

<div align="center">
  <img src="visuals/sentiment_by_app_type.png" width="600">
  <img src="visuals/sentiment_by_category.png" width="600">
  <img src="visuals/sentiment_by_rating.png" width="600">
</div>

---

## 📁 Project Structure

```
Sentiment-Analysis-Google-Play-Reviews/
├── notebooks/
│   └── sentiment_analysis_notebook.ipynb
├── data/
│   ├── apps.csv
│   └── user_reviews.csv
├── visuals/
│   └── (charts & plots)
├── presentation/
│   └── Sentiment_Analysis_Presentation_Ajayi_Oluwaseyi.pptx
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

1. Clone the repository  
2. Open `notebooks/sentiment_analysis_notebook.ipynb`
3. Install required packages:  
   ```bash
   pip install -r requirements.txt
   ```
4. Run all cells

---

## 💬 Final Notes

This project demonstrates how machine learning and NLP can turn qualitative text data into measurable insights. It was completed as part of a sentiment analysis internship task and serves as a practical application of real-world data science.

---

## 🙏 Acknowledgements

- Dataset originally from [Google Play Store Kaggle Dataset](https://www.kaggle.com/datasets/lava18/google-play-store-apps)

---

> ✨ *Feel free to fork this repo, ask questions, or connect with me on LinkedIn!*
