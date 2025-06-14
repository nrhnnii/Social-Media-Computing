# 📚 Natural Language Processing on Malaysian Restaurant Reviews

This repository explores a full NLP pipeline using real-world customer reviews from Google Maps. The tutorials cover everything from basic preprocessing to advanced sentiment analysis and social network modeling — all using the same dataset:

📁 **Dataset**: [GoogleReview_data_cleaned.csv](https://www.kaggle.com/datasets/choonkhonng/malaysia-restaurant-review-datasets)  
🗂️ **Source**: Google Maps reviews of restaurants across Malaysia

---

## 🔍 Tutorials Overview

### 📁 Tutorial 3 & 4 – Text Preprocessing & NLP with NLTK
**Goal**: Learn essential text preprocessing techniques  
**Topics**:
- Sentence segmentation, tokenization, case folding
- Punctuation and stopword removal
- POS tagging, stemming
- Named Entity Recognition (NER) using spaCy
- Word cloud visualization

---

### 📁 Tutorial 5 & 6 – Sentiment Analysis with TextBlob & VADER
**Goal**: Extract sentiment orientation using lexicon-based models  
**Tools**: TextBlob, VADER  
**Tasks**:
- Polarity and subjectivity scoring
- Social-media-aware sentiment analysis
- Comparing and visualizing both tools

---

### 📁 Tutorial 7 – Social Network Analysis with NetworkX & Louvain
**Goal**: Discover user behavior through reviewer–restaurant relationships  
**Tools**: NetworkX, community-louvain  
**Tasks**:
- Bipartite graph modeling
- Reviewer similarity projection
- Community detection and visualization

---

### 📁 Tutorial 8 & 9 – Opinion Mining & Sentiment Enrichment with Transformers
**Goal**: Go deeper into meaning, tone, and nuance in user reviews  
**Tools**: spaCy, pywsd, Hugging Face Transformers, VADER  
**Tasks**:
- Named Entity Recognition (NER)
- Word Sense Disambiguation (WSD)
- Sentence sentiment classification (RoBERTa)
- Lexicon-based word sentiment
- Polarity and sentiment strength extraction

---

### 📁 Tutorial 10 & 11 – Aspect-Based Opinion Mining & Sentiment Modeling  
**Goal**: Identify what people like or dislike about specific aspects (e.g., food, service)  
**Tools**: spaCy, WordCloud, Matplotlib  
**Tasks**:
- Opinion type classification: Explicit vs Implicit
- Aspect-opinion extraction via dependency parsing (spaCy)
- Grouping aspects by sentiment using rating-based labels
- Visualization of top aspects and opinions using word clouds

---

### 📁 Exercise 3 – Machine Learning-Based Sentiment Modeling  
**Goal**: Apply both unsupervised and supervised ML to analyze review sentiments  
**Dataset Used**: `GoogleReview_data_cleaned.csv`

#### a) Dependency-Based Parsing for Aspect Sentiment
- Used **SpaCy** to extract adjective–noun pairs (e.g., *"bad service"*, *"great ambience"*)
- Parsed opinion-bearing phrases using dependency labels like `amod`
- Helped identify sentiment tied to specific review aspects (e.g., food, staff, view)

#### b) Unsupervised Learning (Clustering)
- Applied **TF-IDF** vectorization + **K-Means** clustering (`k=3`)
- Grouped reviews into semantic clusters:
  - Cluster 0: Highly negative complaints
  - Cluster 1: Mixed or service-focused
  - Cluster 2: Vague or fragmented reviews
- Explored common themes per cluster for topic modeling

#### c) Supervised Learning (Sentiment Classification)
- Generated sentiment labels from review ratings:
  - Ratings 4–5 → Positive
  - Ratings 1–2 → Negative
- Trained a **Logistic Regression** classifier on TF-IDF features
- Achieved **93.3% accuracy**, with high performance on positive reviews
- Noted some performance drop in identifying negative reviews
