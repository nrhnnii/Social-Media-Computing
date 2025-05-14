### 📁 Tutorial 3 & 4

**Topic**: Text Preprocessing & NLP with NLTK

**Description**:  
This tutorial introduces basic Natural Language Processing (NLP) techniques using the NLTK library. It covers essential preprocessing steps including sentence segmentation, tokenization, case folding, punctuation removal, stopword removal, stemming, and part-of-speech (POS) tagging. The tutorial also includes advanced tasks such as Named Entity Recognition (NER) using SpaCy and word cloud generation to visualize frequently used terms.

The analysis is performed on a restaurant reviews dataset collected from Google Maps: [`GoogleReview_data_cleaned.csv`](https://www.kaggle.com/datasets/choonkhonng/malaysia-restaurant-review-datasets) 

---

### 📁 Tutorial 5 & 6

**Topic**: Sentiment Analysis with TextBlob & VADER

**Description**:  
This tutorial focuses on unsupervised sentiment analysis using two lexicon-based tools: **TextBlob** and **VADER**. Both methods were applied to customer reviews to extract polarity (positive/negative) and subjectivity scores. TextBlob provided a basic sentiment score and subjectivity measure, while VADER offered a more granular breakdown including negative, neutral, positive proportions and a compound score optimized for social media-style text. A comparison between both methods was conducted through correlation analysis and visualization. This allowed deeper understanding of how each tool interprets tone and emotion in user-generated text.

The analysis was performed on a dataset of restaurant reviews from Google Maps: [`GoogleReview_data_cleaned.csv`](https://www.kaggle.com/datasets/choonkhonng/malaysia-restaurant-review-datasets)

---

### 📁 Tutorial 7

**Topic**: Social Network Analysis with NetworkX & Louvain

**Description**:  
This tutorial introduces the fundamentals of Social Network Analysis (SNA) using Python libraries **NetworkX** and **community-louvain**. A bipartite graph was constructed linking reviewers to restaurants. The graph was then projected into a reviewer–reviewer network based on shared restaurant interactions. The **Louvain method** was used to detect community structures within this network, revealing clusters of reviewers with similar food preferences. The detected communities were analyzed to identify common restaurant patterns, and results were visualized to highlight the connectivity and segmentation of reviewer behavior.

The network analysis was conducted on the same restaurant reviews dataset: [`GoogleReview_data_cleaned.csv`](https://www.kaggle.com/datasets/choonkhonng/malaysia-restaurant-review-datasets), making it possible to explore real-world social interactions and preferences within a local food scene.
