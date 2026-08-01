# 🐦🤖 Twitter & Reddit Feedback Sentiment Model

An end-to-end Natural Language Processing (NLP) and Machine Learning project designed to analyze public sentiment and customer feedback across social media platforms (Twitter and Reddit). The project cleans unstructured social media text, performs exploratory data analysis, and implements a **RandomForest Classifier** to categorize feedback into positive, negative, or neutral sentiments.

---

## 🚀 Project Overview
Social media is a goldmine for real-time customer opinions. This project builds a pipeline to aggregate and analyze text data from Twitter and Reddit to help brands understand customer pain points and satisfaction levels. 

### Key Objectives:
- Preprocess noisy social media text (removing handles, hashtags, URLs, and emojis).
- Vectorize text using techniques like TF-IDF or CountVectorizer.
- Train a **RandomForest Model** to accurately classify the sentiment of posts/tweets.
- Extract key trends and keywords driving public discussion.

## 📊 Dataset & Features
The dataset consists of scraped or open-source social media posts containing:
- **Text Content:** Raw tweets and Reddit comments.
- **Platform:** Source indicator (Twitter vs. Reddit) to compare community behaviors.
- **Metadata:** Upvotes/Likes, Retweets, or timestamps (if available).
- **Target Variable:** Sentiment Label (`Positive`, `Negative`, `Neutral`).

## 🛠️ Tech Stack & Libraries
- **Language:** Python 3.x
- **Environment:** Jupyter Notebook (`Twitter_Reddit_Feedback_Model.ipynb`)
- **Text Processing & NLP:** NLTK / SpaCy, Regex (`re`)
- **Feature Extraction:** Scikit-Learn (`TfidfVectorizer` / `CountVectorizer`)
- **Machine Learning:** Scikit-Learn (`RandomForestClassifier`, `train_test_split`)
- **Evaluation:** Confusion Matrix, Classification Report, Accuracy Score
- **Visualization:** Matplotlib, Seaborn, WordCloud

## 📂 Project Structure
```text
├── data/
│   ├── raw_feedback_data.csv       # Combined raw Twitter & Reddit text
│   └── cleaned_feedback_data.csv   # Tokenized and preprocessed text
├── Twitter_Reddit_Feedback_Model.ipynb # Main Jupyter Notebook containing the pipeline
├── README.md                       # Project documentation
└── requirements.txt               # Dependencies list
```

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd twitter-reddit-feedback-model
   ```

2. **Install required libraries:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the analysis:**
   Launch Jupyter Notebook and open `Twitter_Reddit_Feedback_Model.ipynb` to execute the code cells.

## 📈 Key Insights & Results
- **Text Cleaning:** Stripping platform-specific noise (like `u/username` or `RT @handle`) significantly boosted model accuracy.
- **Model Performance:** The RandomForest Classifier achieved an overall accuracy of **81%** .
- **Model Performance:** LogisticRegression Accuracy: 0.8707 **0.8707%** .
- **Model Performance:** LinearSVC Accuracy: **0.8776%** .
- **Platform Variation:** Reddit comments tended to be longer and more descriptive, while Twitter data was concise but heavily reliant on emojis and slang.

## 🤝 Contributing
Feel free to open an issue or submit a pull request if you want to improve the text preprocessing pipeline or test different ML architectures!
