# 🎬 Movie Success Prediction and Sentiment Study

## 📌 Objective
To analyze sentiment trends in movie reviews and predict the success of movies based on user review data using machine learning.

---

## 🛠️ Tools & Libraries
- Python (Pandas, NLTK, Sklearn, Matplotlib, Seaborn)
- VADER Sentiment Analyzer (from NLTK)
- Scikit-learn (for classification models)
- Excel (optional for data export/analysis)

---

## 📥 Data Source
- [IMDB Movie Reviews Dataset (Kaggle)](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
- 50,000 movie reviews labeled as **positive** or **negative**

---

## 🧠 Project Workflow

### 1. **Data Cleaning & Preprocessing**
- Removed HTML tags, special characters
- Converted text to lowercase
- Tokenized text, removed stopwords (optional)
- Applied **TF-IDF vectorization**

### 2. **Sentiment Analysis (VADER)**
- Used `VADER` to compute sentiment scores:
  - Compound score ranges from -1 (negative) to +1 (positive)
- Added `vader_compound` column to dataset

### 3. **Genre-wise Sentiment Study**
- Simulated genres (e.g., Drama, Comedy, Action) for each review
- Exploded genre tags and analyzed sentiment per genre
- 📊 Generated bar plot for average sentiment by genre

### 4. **Predictive Modeling**
- Converted reviews to TF-IDF vectors
- Trained multiple ML models:
  - Logistic Regression
  - Naive Bayes
  - Random Forest
  - Support Vector Machine (SVM)
- Evaluated using accuracy, precision, recall, and ROC-AUC

---

## 📈 Predictive Model Summary

| Model                  | Accuracy | Notes                                      |
|------------------------|----------|--------------------------------------------|
| **Logistic Regression**| ~88%     | Lightweight, fast, interpretable           |
| **Random Forest**      | ~85%     | Decent but slower                          |
| **Naive Bayes**        | ~84%     | Simple, performs well                      |
| **SVM (Linear)**       | ~89%     | Best performer for this dataset            |

- **🏆 Best Model:** `SVM + TF-IDF`
- Strong correlation between `vader_compound` and true sentiment labels

---

## 📊 Visualizations
- Confusion matrix
- ROC Curve
- Bar chart of average VADER sentiment by genre

---

## 📂 Deliverables
- Python notebooks for:
  - Preprocessing
  - VADER sentiment analysis
  - Model training & evaluation
- `README.md` (this file)
-------
