# LinkedIn Posts & Comments Sentiment Analysis

This project performs **sentiment analysis on LinkedIn posts and their comments** using **NLTK’s VADER sentiment analyzer**.  
It processes raw CSV data, cleans text, calculates sentiment scores, classifies emotions, and outputs structured results for analysis.

---

## 🔍 Project Overview

Social media content contains valuable emotional signals.  
This project helps answer questions like:
- Are LinkedIn posts perceived positively or negatively?
- How do people emotionally react through comments?
- Which posts generate positive engagement?

The pipeline is designed for **data analysis, NLP learning, and portfolio demonstration**.

---

## 🧠 Features

- Text cleaning and preprocessing
- Sentiment scoring (Positive, Negative, Neutral)
- Separate analysis for posts and comments
- Post-wise comment sentiment mapping
- CSV output for easy visualization and reporting

---

## 🛠️ Technologies Used

- Python
- Pandas
- NLTK
- VADER Sentiment Analyzer
- Regular Expressions
- CSV-based data pipeline

project-root/
│
├── data/
│ ├── processed/
│ │ ├── filtered_posts_cleaned.csv
│ │ ├── comments/
│ │ │ ├── linkedin-<post_id>.csv
│ │ └── result/
│ │ ├── results_filtered_posts_cleaned.csv
│ │ └── comments/
│ │ ├── results_linkedin-<post_id>.csv
│
├── sentiment_analysis.py
├── README.md
└── requirements.txt




## 📂 Project Structure

