# McDonald’s Sentiment Analysis (Lexicon-Based NLP)

This project performs lexicon-based sentiment analysis on McDonald’s customer reviews using three widely used sentiment lexicons: **Bing**, **AFINN**, and **NRC**.  
The goal is to compare how different lexicons capture sentiment polarity, intensity, and emotional content in real-world customer feedback.

---

## Dataset
- **Source:** McDonald’s customer reviews (CSV format)
- **Size:** 500 sampled reviews
- **Text Field:** Review text
- **Metadata:** Star rating, store information, review time

> The dataset is used for educational and portfolio purposes.

---

## Methodology

### 1. Text Preprocessing
- Tokenisation (word-level)
- Lowercasing
- Stop-word removal
- Removal of punctuation and non-alphabetic tokens

### 2. Sentiment Lexicons Applied

#### 🔹 Bing Lexicon
- Classifies words as **positive** or **negative**
- Produces a review-level sentiment score:  
  **positive words − negative words**

#### 🔹 AFINN Lexicon
- Assigns **numeric sentiment scores** (−5 to +5) to words
- Captures **sentiment intensity**
- Review-level score is the sum of word scores

#### 🔹 NRC Lexicon
- Maps words to **emotions** (joy, trust, anger, fear, etc.)
- Provides emotional composition rather than a single polarity score

---

## Key Findings

- **Overall sentiment is mildly positive** across all lexicons.
- Bing results show most reviews cluster around small positive scores (+1).
- AFINN reveals a wider score range, capturing sentiment intensity while still indicating a slight positive bias.
- NRC analysis highlights dominant emotions such as **positive**, **trust**, and **joy**, alongside smaller but meaningful levels of **anger**, **fear**, and **sadness**.
- Text-based sentiment aligns well with customer star ratings.

---

## Visualisations
The project includes:
- Sentiment score histograms (Bing & AFINN)
- Positive vs negative word counts
- Sentiment vs star rating boxplots
- Emotion distribution bar chart (NRC)

---

## Files in This Repository
- `mcdonalds_sentiment_analysis.Rmd` — R Markdown source code
- `mcdonalds_sentiment_analysis.html` — Rendered analysis output
- `README.md` — Project documentation

---

## How to View the Results
- Download and open `mcdonalds_sentiment_analysis.html` in a browser  
  **or**
- Knit the `.Rmd` file in RStudio to reproduce the analysis

---

## Tools & Libraries
- R
- tidyverse
- tidytext
- textdata
- ggplot2

---

## Author
**Awad Pervez**  
MSc Data Science

