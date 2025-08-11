# 🎬 Hybrid Content-Based Movie Recommendation System with Sentiment-Aware Re-Ranking

This project is a **hybrid content-based movie recommender system** that calculates similarity across **plot, genre, metadata, and user reviews**, then re-ranks the top recommendations based on **audience sentiment** from user reviews.

Unlike traditional recommenders that only use plot or genre similarity, our system:
- Extracts **semantic embeddings** of plot and reviews using **Sentence-BERT**.
- Computes **genre similarity** with **Jaccard Similarity**.
- Processes **cast, crew, and keywords** using **TF-IDF**.
- Combines similarities using **weighted sum**.
- Enhances recommendations by incorporating **Logistic Regression sentiment classification** for re-ranking.

---

## 🚀 Features
- Hybrid similarity calculation using:
  - **SBERT** embeddings for plot and reviews
  - **TF-IDF** for metadata
  - **Jaccard** for genre
- Sentiment analysis using **Logistic Regression**
- Re-ranking with **0.8 similarity weight** and **0.2 sentiment score**
- Customizable top-k results
- Supports **TMDB API** for fetching movie metadata
- Streamlit/Flask UI for easy interaction

---

## 📊 Example Output

| Query Movie  | Recommended Movie  | Similarity | Sentiment | Final Score |
|--------------|--------------------|------------|-----------|-------------|
| Inception    | Minority Report    | 0.499      | 0.981     | 0.596       |
| Spider-Man   | Spider-Man 2       | 0.693      | 0.982     | 0.751       |

---

## 🛠️ Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/movie-recommender.git
cd movie-recommender
