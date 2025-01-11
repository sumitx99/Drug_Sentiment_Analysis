# 💊 Sentiment Analysis on Drug Review Dataset 📊

## Overview
This project utilizes the **Drug Review Dataset** to analyze user evaluations of various medications for different diseases. These reviews, available in both written and numerical formats, are categorized into five sentiment polarity groups. We tested several classification models, including **LGBM**, **XGBoost**, **CatBoost**, and **Naive Bayes Classifier**. The **LightGBM** classifier achieved the highest accuracy at **75%**. Based on numerical ratings, the system suggests highly-rated medications for specific ailments.

## Dataset
🔗 [Drug Review Dataset](https://www.kaggle.com/jessicali9530/kuc-hackathon-winter-2018)

## Methodology

### 1. 🧹 Data Cleaning
- **Null and Empty Values**: Removed to maintain dataset integrity.
- **Sorting**: Based on user ratings to identify top-rated drugs.
- **Unique Conditions**: Formed the foundation of the recommendation system.

### 2. 📝 Sentiment Analysis
- **TextBlob**: Used for determining sentiment polarity and subjectivity.
  - Polarity ranges from **-1** (negative) to **1** (positive).
  - **Negation Words**: Invert polarity for nuanced analysis.
- **Stopwords and Stemming**: Retained to maintain the essence of reviews.

### 3. 🔢 Feature Engineering
- **Weighted Rating**: Prioritized ratings to enhance recommendation system effectiveness.
- **Correlation Matrix**: Plotted to show linear relationships between features.
- **Label Encoding**: Converted drug names and conditions into numeric values.

### 4. 🤖 Model Training
- **LGBM**, **XGBoost**, **CatBoost**, and **Naive Bayes Classifier** were trained to evaluate their performance in sentiment prediction.
- **Target Variable**: Sentiment Rating.

## Results

### 📈 LightGBM
- **Accuracy**: **75.2%**
- **True Positive (TP) Count**: 24,251

### 📉 XGBoost
- **Accuracy**: **55%**
- **True Positive (TP) Count**: 24,390

### 📉 CatBoost
- **Accuracy**: **55%**
- **Lower TP Count** compared to XGBoost.

### 🚫 Naive Bayes Classifier
- **Lowest Accuracy**: Not suitable for this task.
