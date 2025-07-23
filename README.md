#  Amazon Alexa Customer Review Sentiment Analysis

This project uses Natural Language Processing (NLP) and machine learning to predict customer satisfaction from Amazon Alexa product reviews.

---

##  Objective

The goal is to determine whether a customer is **satisfied** (`feedback = 1`) or **not satisfied** (`feedback = 0`) based on their written product review.

---

##  Technologies Used

- Python
- pandas, NumPy, seaborn, matplotlib
- NLTK for text preprocessing
- `CountVectorizer` for text feature extraction
- Machine Learning Models:
  - Naive Bayes
  - Logistic Regression
- Scikit-learn for model training, evaluation, and metrics

---

##  Dataset

The dataset is from [Amazon Alexa Reviews on Kaggle](https://www.kaggle.com/datasets/sid321axn/amazon-alexa-reviews) and includes the following features:
- `verified_reviews` (text of the review)
- `variation` (product type)
- `rating` (1–5 stars)
- `feedback` (target: 1 = satisfied, 0 = not satisfied)

---

##  Exploratory Data Analysis

- Distribution of ratings and feedback
- Word clouds for all reviews and negative reviews
- Heatmaps for missing values
- Histograms for review length

---

##  Model Training & Evaluation

We trained and evaluated two classification models:
| Model              | Accuracy |
|-------------------|----------|
| Naive Bayes        | ~93%     |
| Logistic Regression | ~95%  |

- **Logistic Regression** performed best overall
- Class imbalance was observed (most reviews were positive)
- Models had high precision/recall for satisfied customers, and moderate performance for dissatisfied ones

---

##  Conclusion

Yes — the majority of customers in the dataset are **satisfied** with their Alexa product.  
Our models successfully learned to classify review sentiment based on text with high accuracy.

---

