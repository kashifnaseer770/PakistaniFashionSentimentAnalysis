# 🇵🇰 Pakistani Fashion Brand Sentiment Analysis

This project analyzes **customer sentiment** toward two leading Pakistani fashion brands—**Khaadi** and **Sapphire**—by mining social media comments from **Instagram** and **Facebook**. Using natural language processing techniques, it provides insights into customer perceptions, identifies key sentiment drivers, and suggests strategies to improve brand engagement.

---

## 🎯 Objectives

- Scrape customer comments from Instagram and Facebook for **Khaadi** and **Sapphire**.
- Clean and preprocess unstructured textual data.
- Perform sentiment analysis using **TextBlob** to classify comments as **Positive**, **Negative**, or **Neutral**.
- Visualize sentiment patterns and trends.
- Save processed data for future modeling and trend tracking.

---

## 🧰 Technologies & Tools

**Programming Language:**  
- Python

**Libraries:**  
- `pandas`, `numpy`: Data handling  
- `textblob`, `nltk`: NLP and sentiment analysis  
- `emoji`: Emoji normalization  
- `matplotlib`, `seaborn`: Data visualization  
- `wordcloud`: Word cloud generation  

**Tools:**  
- `instaloader`: Instagram scraping  
- Facebook scraping tools (custom/manual scraping)  
- Jupyter Notebook / VS Code: Development environments  

---

## 📁 Dataset Details

Comments are sourced from **official social media pages** of:

- **Khaadi** → `khaadi.json`  
- **Sapphire** → `sapphire.json`

Each dataset contains:
- `username`: Commenter's username  
- `comment_text`: The content of the comment  
- `post_link`: URL of the original post  
- `comment_timestamp`: (If available) Timestamp of the comment  

**Processed Files:**
- `cleaned_comments.csv`: Preprocessed, cleaned text
- `sentiment_comments_final.csv`: Comments with sentiment labels
- `cleaned_fashion_comments_with_sentiment.json`: Final JSON dataset with sentiment categories and polarity scores

---

## ⚙️ Installation Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/PakistaniFashionSentimentAnalysis.git
cd PakistaniFashionSentimentAnalysis
````

### 2. Set Up Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate  # For Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn textblob nltk emoji wordcloud instaloader
```

### 4. Download NLTK Resources

```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

---

## 🚀 Usage

### 1. Place Datasets

Put the following files inside the `Datasets/` folder:

* `khaadi.json`
* `sapphire.json`

Update file paths in the notebook if needed.

### 2. Run the Notebook

```bash
jupyter notebook Kashifnaseer_ESHIP_project.ipynb
```

Execute all cells to:

* Load and clean data
* Run sentiment classification
* Generate visualizations
* Save output files

---

## 📊 Results Summary

### 🔹 Sentiment Distribution

* **Positive Drivers**: *“beautiful designs,” “quality fabric,” “great value”*
* **Negative Drivers**: *“expensive,” “late delivery,” “poor customer service”*

### 🔹 Visual Insights

* **Violin Plots**: Show sentiment score spread by brand
* **Word Clouds**: Top keywords in positive and negative comments
* **Temporal Trends**: Sentiment shifts during Eid sales, price hikes, etc.

---

## 🧠 Future Enhancements

* Integrate real-time sentiment monitoring via APIs
* Expand analysis to include more local fashion brands
* Use advanced NLP (e.g., BERT, RoBERTa) for higher accuracy
* Add Urdu language support
* Develop an interactive dashboard using Streamlit or Dash

---

## 📂 Directory Structure

```
PakistaniFashionSentimentAnalysis/
│
├── Datasets/
│   ├── khaadi.json
│   └── sapphire.json
│
├── Kashifnaseer_ESHIP_project.ipynb
├── sentiment_violinplot.png
├── cleaned_fashion_comments_with_sentiment.json
├── sentiment_comments_final.csv
├── cleaned_comments.csv
├── eship_Report.pdf
├── README.md
```

---

## 👥 Contributor

* **Kashif Naseer**

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more details.


> ⚠️ **Disclaimer**: This analysis is for academic and research purposes only. It is not affiliated with or endorsed by Khaadi or Sapphire.
