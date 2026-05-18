# 🏛️ Global Historical Sites Review Intelligence System
### NLP + Machine Learning + GeoAnalytics | IKS Activity | NEP 2020

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![NLP](https://img.shields.io/badge/NLP-VADER%20%7C%20TextBlob%20%7C%20LDA-green)
![ML](https://img.shields.io/badge/ML-Logistic%20Regression%20%7C%20Naive%20Bayes%20%7C%20Random%20Forest-orange)
![GeoAnalytics](https://img.shields.io/badge/Geo-Folium%20%7C%20GeoPandas-red)
![Dataset](https://img.shields.io/badge/Data-Real%20Kaggle%20TripAdvisor-yellow)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Project Overview

This is a complete **end-to-end Data Science project** that analyses real visitor reviews of globally significant heritage sites using **Natural Language Processing (NLP)**, **Machine Learning (ML)**, and **Geo-Spatial Analytics**.

The project is designed as an **Indian Knowledge Systems (IKS) academic activity** under NEP 2020, comparing Indian heritage sites (Taj Mahal, Hampi, Ajanta Caves, Khajuraho, Qutb Minar) against global counterparts (Colosseum, Great Wall of China, Machu Picchu, Petra, Angkor Wat).

---

## 🗂️ Repository Structure

```
heritage-review-intelligence/
│
├── 📓 notebooks/
│   ├── Heritage_Review_Intelligence_v2.ipynb   ← Main project notebook (run this)
│   └── Heritage_Review_Intelligence_v1.ipynb   ← Synthetic data version (reference)
│
├── 📊 data/
│   ├── README_data.md                          ← Instructions to download Kaggle CSVs
│   ├── heritage_reviews_processed.csv          ← Generated after running notebook
│   ├── heritage_site_analytics.csv             ← Generated after running notebook
│   └── lda_topic_summary.csv                   ← Generated after running notebook
│
├── 🖼️ outputs/
│   ├── eda_rating_sentiment.png
│   ├── eda_site_visitor.png
│   ├── eda_top_words.png
│   ├── eda_temporal.png
│   ├── eda_heatmap.png
│   ├── eda_sentiment_by_site.png
│   ├── nlp_sentiment_comparison.png
│   ├── nlp_vader_dist.png
│   ├── nlp_lda_topics.png
│   ├── nlp_wordclouds_all.png
│   ├── ml_confusion_matrices.png
│   ├── ml_model_comparison.png
│   ├── ml_feature_importance.png
│   ├── geo_bubble_map.png
│   ├── insight_india_vs_global.png
│   └── final_summary_dashboard.png
│
├── 🗺️ maps/
│   └── geo_heritage_sentiment_map.html         ← Interactive Folium world map
│
├── requirements.txt                            ← All Python dependencies
├── .gitignore                                  ← Files to exclude from Git
└── README.md                                   ← This file
```

---

## 📥 Datasets Used (Real Kaggle Data)

| # | Dataset | Source | Rows | Download |
|---|---------|--------|------|----------|
| 1 | **Trip Advisor Hotel Reviews** | Kaggle — andrewmvd | 20,456 | [Download](https://www.kaggle.com/datasets/andrewmvd/trip-advisor-hotel-reviews) |
| 2 | **TripAdvisor Reviews 2023 (New Delhi)** | Kaggle — arnabchaki | ~5,000 | [Download](https://www.kaggle.com/datasets/arnabchaki/tripadvisor-reviews-2023) |

> ⚠️ Due to Kaggle's terms of service, raw CSV files are **not included** in this repository.  
> Please download them manually and place in the `data/` folder before running the notebook.

---

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/heritage-review-intelligence.git
cd heritage-review-intelligence
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Download Kaggle Datasets
```bash
# Option A: Kaggle CLI
pip install kaggle
kaggle datasets download -d andrewmvd/trip-advisor-hotel-reviews
kaggle datasets download -d arnabchaki/tripadvisor-reviews-2023
unzip "*.zip" -d data/

# Option B: Manual
# Visit the links above → Download → place CSVs in data/ folder
```

### 4. Run the Notebook
```bash
jupyter notebook notebooks/Heritage_Review_Intelligence_v2.ipynb
```

---

## 🔬 Project Methodology

```
RAW DATA (Kaggle TripAdvisor Reviews)
         ↓
DATA CLEANING & PREPROCESSING
  • Lowercase → URL removal → Punctuation removal
  • Tokenization → Stopword removal → Lemmatization
  • Rating → Sentiment Label (≥4=Positive, 3=Neutral, ≤2=Negative)
         ↓
EXPLORATORY DATA ANALYSIS (EDA)
  • Rating distribution, Sentiment pie, Top words
  • Temporal trends, Correlation heatmap, Site comparison
         ↓
NLP ANALYSIS
  • Sentiment: VADER + TextBlob (comparison)
  • Topic Modeling: LDA (5 topics)
  • WordClouds per heritage site
         ↓
MACHINE LEARNING
  • TF-IDF Vectorization (5000 features, n-grams)
  • Logistic Regression | Naive Bayes | Random Forest
  • Accuracy, Precision, Recall, F1, Confusion Matrix
         ↓
GEO-SPATIAL ANALYTICS
  • Folium interactive world map (sentiment-colored markers)
  • Static bubble map (bubble size = review count)
         ↓
INSIGHTS & INTERPRETATION
  • IKS-based preservation recommendations
  • India vs Global benchmarking
```

---

## 📊 Key Results

| Metric | Value |
|--------|-------|
| Total Reviews Analysed | 20,000+ (real TripAdvisor) |
| Heritage Sites Covered | 10 (5 Indian + 5 Global) |
| Best ML Model | Logistic Regression |
| NLP Tools Used | VADER, TextBlob, LDA |
| LDA Topics Discovered | 5 (Architecture, Experience, Spirituality, Infrastructure, Archaeology) |
| Geo Coverage | 7 countries across 4 continents |

---

## 🏛️ Heritage Sites Covered

| Indian Sites 🇮🇳 | Global Sites 🌍 |
|---|---|
| Taj Mahal (Agra) | Colosseum (Rome, Italy) |
| Hampi (Karnataka) | Great Wall of China (Beijing) |
| Ajanta Caves (Maharashtra) | Machu Picchu (Peru) |
| Khajuraho Temples (MP) | Petra (Jordan) |
| Qutb Minar (Delhi) | Angkor Wat (Cambodia) |

---

## 🧰 Tech Stack

| Category | Libraries |
|----------|-----------|
| Data Processing | `pandas`, `numpy` |
| Visualisation | `matplotlib`, `seaborn` |
| NLP | `nltk`, `textblob`, `vaderSentiment` |
| Topic Modeling | `sklearn.decomposition.LDA` |
| WordCloud | `wordcloud` |
| Machine Learning | `scikit-learn` |
| Geo Analytics | `folium` |

---

## 🎓 IKS Relevance (NEP 2020)

This project fulfils the **Indian Knowledge Systems (IKS)** activity requirement under NEP 2020 by:

1. **Computational validation** of Shilpa Shastra architectural principles through visitor sentiment
2. **Data-driven preservation** insights for Indian heritage sites
3. **Global benchmarking** of Indian heritage against world-class sites
4. **Cross-disciplinary** integration of data science with cultural heritage studies
5. **Policy recommendations** grounded in real visitor feedback data

---

## 📈 Sample Outputs

> All output images are saved in the `outputs/` folder after running the notebook.

- `eda_rating_sentiment.png` — Overall rating & sentiment distribution
- `nlp_wordclouds_all.png` — WordClouds for all 10 heritage sites
- `ml_confusion_matrices.png` — ML model evaluation
- `geo_heritage_sentiment_map.html` — Interactive world map *(open in browser)*
- `final_summary_dashboard.png` — Dark-theme project dashboard

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Kaveri Koli**  
Department of Computer Science  
MSc Data Science 
Academic Year: 2025–26

---

## 📚 References

1. andrewmvd. *Trip Advisor Hotel Reviews*. Kaggle, 2020.
2. arnabchaki. *Tripadvisor Reviews 2023*. Kaggle, 2023.
3. Hutto & Gilbert (2014). *VADER Sentiment Analysis*. ICWSM.
4. Blei et al. (2003). *Latent Dirichlet Allocation*. JMLR.
5. Ministry of Education. *NEP 2020*. Government of India.
6. UNESCO. *World Heritage List*, 2024.

---


