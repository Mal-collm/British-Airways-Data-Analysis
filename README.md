# British-Airways-Data-Analysis
This project analyzes customer reviews of British Airways to uncover insights into passenger sentiment, service performance, and frequently mentioned topics.

# Project Strcture
- `data/` – Contains raw and cleaned review data
- `notebooks/` – Google Colab used for cleaning, analysis, and modeling
- `images/` – Word clouds and visualizations
- `sentiment_model` – Trained ML model for sentiment prediction

# Features

# 1. Data Collection
- Collected 1,000+ customer reviews from a public airline review website
- Handled pagination and stored reviews for analysis

# 2. Data Cleaning
- Removed irrelevant phrases (e.g., “✅ Trip Verified”)
- Removed symbols and special characters
- Stripped whitespace and standardized text

# 3. Word Cloud Visualization
- Highlighted most frequently used words in reviews
- Identified common discussion points like: `flight`, `seat`, `food`, `service`, `crew`

# 4. Sentiment Analysis
- Used VADER sentiment analyzer to label reviews as:
  - Positive (compound score ≥ 0.05)
  - Negative (≤ -0.05)
  - Neutral (between -0.05 and 0.05)
  
# 5. Machine Learning Model
- Vectorized text using `TfidfVectorizer`
- Trained a `LogisticRegression` model to predict sentiment
- Achieved ~82% accuracy on test data

# Sample Results

| Sentiment | Precision | Recall | F1-Score | Support |
|-----------|-----------|--------|----------|---------|
| Positive  | 0.83      | 0.78   | 0.80     | 89      |
| Negative  | 0.82      | 0.88   | 0.85     | 109     |
| Neutral   | 0.00      | 0.00   | 0.00     | 2       |
| **Accuracy** |       |        | **0.82** | **200** |


# Key Insights

- Most discussed topics: **flight**, **seat**, **food**, **service**, **BA crew**
- Negative reviews were often tied to **delays**, **luggage issues**, and **refund problems**
- Positive reviews focused on **crew friendliness** and **business class service**


## 📌 Technologies Used

- Python
- Pandas, NumPy
- NLTK (VADER)
- Scikit-learn
- Matplotlib, Seaborn
- WordCloud

# Author

Developed by MALCOLM AGBATI  
Feel free to connect or suggest improvements!
