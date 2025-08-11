# Movie-Recommender-system-using-NLP-and-ML
# 🎥 Advanced Movie Recommendation System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0%2B-orange)
![NLTK](https://img.shields.io/badge/NLTK-3.7-yellowgreen)
![License](https://img.shields.io/badge/License-MIT-brightgreen)

A hybrid recommendation engine combining **content-based filtering** with **sentiment-aware reranking** for personalized movie suggestions.

## 🔍 Overview
This system recommends movies using:
1. **Weighted fusion** of:
   - Plot similarity (S-BERT + Cosine similarity)
   - Metadata similarity (genres/directors)
   - Review text similarity
2. **Sentiment-based reranking** of top candidates from sentiments of User Reviews
3. 

## 🚀 Key Features
- **Multi-dimensional similarity analysis**
- ## Weighted fusion of various similarity aspects
- **Sentiment-powered reranking** (VADER/TextBlob)
- **Modular design** for easy experimentation
- **Cold-start capable** (no user history required)

## 📦 Installation
```bash
git clone https://github.com/yourusername/movie-recommender.git
cd movie-recommender
pip install -r requirements.txt
