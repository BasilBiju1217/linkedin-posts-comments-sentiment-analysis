📊 LinkedIn Data Scraping & Sentiment Analysis Project

This project automates the extraction, preprocessing, sentiment analysis, and visualization of LinkedIn posts and comments. It provides a complete data pipeline from scraping to analytics, enabling insights into engagement patterns, author behavior, sentiment trends, reactions distribution, and text analytics.

---

## 🚀 Project Overview

This project performs:

### ✔ 1. **Data Scraping**
- Scrapes **LinkedIn posts and comments** using Selenium/Playwright.
- Extracts post text, author details, timestamps, reaction counts, and comment threads.
- Exports raw JSON data for further processing.

### ✔ 2. **Processing & Cleaning**
- Converts nested LinkedIn JSON into structured rows.
- Cleans text (lowercasing, punctuation removal, stopword removal, etc.)
- Combines posts and comments into a unified long-format dataset.

### ✔ 3. **Sentiment Analysis (VADER)**
- Computes `positive`, `negative`, `neutral`, `compound` scores.
- Generates categorical sentiment labels for posts and comments.

### ✔ 4. **Visualization & Insights**
The script produces **10 analytics plots**, including:

1. Sentiment Distribution  
2. Sentiment Score Distribution  
3. Post vs Comment Sentiment Heatmap  
4. Sentiment Match Analysis  
5. Engagement Metrics vs Sentiment  
6. Reaction Types Distribution  
7. Posts Over Time  
8. Top Authors  
9. Text Length Analysis  
10. Correlation Matrix  

### ✔ 5. **Dashboard Generation**
- Combines all plots into a single **dashboard.html** file.
- Generates `dashboard_summary_plot.png` (combined collage of plots).

---
## 🔗 URN Linking

Comments are automatically linked to posts using LinkedIn URN IDs:
- Post URN: `urn:li:activity:7357944725993086976`
- Comment file: `linkedin-7357944725993086976.csv`

## 🧰 Technologies Used

### **Languages**
- Python 3.10+

### **Libraries**
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- NLTK (VADER Sentiment)  
- Selenium / Playwright  
- WordCloud  

---

## ⚙️ Setup Instructions

### **1. Clone the repository**
```bash
git clone https://github.com/your-username/linkedin-extractor.git
cd LinkedIn-analysis
2. Create virtual environment
bash
Copy code
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows
3. Install dependencies
bash
Copy code
pip install -r requirements.txt

## 📝 Input Data Format

### Posts CSV
Required columns:
- `text` - Post content
- `full_urn` - LinkedIn URN for linking

### Comments CSV
Required columns:
- `Comment` - Comment text
- Filename must contain URN: `linkedin-[URN_ID].csv`

## 🎯 Key Features

- **Text Preprocessing**: Lowercasing, URL removal, mention cleaning, stop words removal
- **VADER Sentiment**: Specialized for social media text
- **Batch Processing**: Handles multiple files automatically
- **Error Handling**: Graceful failures with detailed logging
- **Flexible Output**: CSV for analysis, JSON for programming

## 📊 Example Results

```python
# Long Format CSV
post_urn_id | post_text | post_sentiment_label | comment_text | comment_sentiment_label
7357944...  | "Hiring..." | Positive | "Great!" | Positive
7357944...  | "Hiring..." | Positive | "Thanks" | Positive

# Nested JSON
{
  "post_urn_id": "7357944...",
  "post_sentiment": {"label": "Positive", "compound": 0.67},
  "comment_stats": {"total_comments": 15, "positive_comments": 10},
  "comments": [...]
}
```
📜 License

This project is open-source and free to use for academic or research purposes.

✉️ Contact

Created by Basil Biju
For queries or suggestions — feel free to reach out via LinkedIn or GitHub.
