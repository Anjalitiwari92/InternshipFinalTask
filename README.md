# 🎬 Movie Success Prediction and Sentiment Study

## 📌 Objective
This project analyzes IMDB movie reviews to:
- Perform sentiment analysis using VADER
- Simulate and predict movie success using sentiment scores
- Visualize sentiment distribution and compare model predictions
- (Optional) Analyze genre-wise sentiment trends

---

## 🧰 Tools & Libraries
- **Python**  
- **Pandas, NumPy** – data wrangling  
- **NLTK (VADER)** – sentiment analysis  
- **Scikit-learn** – regression modeling  
- **Matplotlib, Seaborn** – visualizations  
- **Excel** – data review and reporting (optional)

---

## 📂 Dataset
- **Source:** [IMDB 50K Movie Reviews Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
- **Fields:**
  - `review`: User-submitted movie review text
  - `sentiment`: Labeled sentiment (positive/negative)

---

## 🧪 Steps Performed

### 1. Data Loading
- Loaded `IMDB Dataset.csv` (50,000 reviews)
- Cleaned and structured data for sentiment analysis

### 2. Sentiment Analysis (VADER)
- Applied NLTK’s VADER analyzer
- Generated `vader_compound` score per review
- Classified sentiment as Positive / Negative / Neutral

### 3. Success Score Simulation
- Simulated a `success_score` based on `vader_compound`:

### 4. Regression Modeling
- Used Linear Regression to predict `success_score` from sentiment
- Evaluated model using RMSE

### 5. Visualizations
- VADER sentiment score distribution
- Crosstab: IMDB label vs VADER classification
- (Optional) Genre-wise sentiment bar chart if genre data is added

---

## 📊 Example Visuals
- Histogram of VADER sentiment scores
- Comparison matrix of labeled vs computed sentiment
- Regression predictions on test set

---

## 📁 Deliverables
- `movie_sentiment_analysis.ipynb` – Notebook with full analysis
- `IMDB_with_VADER.csv` – Dataset with added sentiment scores (optional)
- Visual plots for report and insights
- README documentation

---

## 🚀 Future Work
- Merge with TMDb/Kaggle metadata for budget, revenue, and genre-based modeling
- Explore advanced NLP models (e.g., BERT) for deeper review analysis
- Genre-wise success prediction and sentiment classification

---

## 🧠 Credits
- VADER Sentiment Analyzer: [NLTK Docs](https://www.nltk.org/api/nltk.sentiment.vader.html)
- Dataset: [Kaggle IMDB Review Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

---
