# 🏛️ Global Historical Sites Review Intelligence System
### NLP + Machine Learning + GeoAnalytics | IKS Activity | NEP 2020

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![NLP](https://img.shields.io/badge/NLP-VADER%20%7C%20TextBlob%20%7C%20LDA-green)
![ML](https://img.shields.io/badge/ML-Logistic%20Regression%20%7C%20Naive%20Bayes%20%7C%20Random%20Forest-orange)
![GeoAnalytics](https://img.shields.io/badge/Geo-Folium%20%7C%20GeoPandas-red)
![Dataset](https://img.shields.io/badge/Data-Real%20Kaggle%20TripAdvisor-yellow)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📌 Problem Statement

Visitor reviews at heritage sites are rich in opinion and insight — but unstructured and difficult to analyze at scale. This project bridges that gap by applying NLP, machine learning, and geo-analytics to **20,000+ real TripAdvisor reviews** across 10 of the world's most iconic heritage sites.

The central question: **How does visitor sentiment at Indian heritage sites compare to global counterparts?**

---

## 🎯 Objectives

- Analyze 20,000+ real-world TripAdvisor reviews
- Perform sentiment analysis using VADER and TextBlob
- Build and evaluate ML classifiers for sentiment prediction
- Extract key themes via LDA topic modeling
- Visualize global sentiment patterns using interactive geo-maps
- Derive actionable insights to support tourism and heritage preservation

---

## 📊 Key Results

| Metric | Value |
|---|---|
| Reviews Analyzed | 20,000+ |
| Heritage Sites | 10 (5 Indian + 5 Global) |
| Countries Covered | 7 |
| Best ML Model | Logistic Regression |
| Sentiment Tools | VADER + TextBlob |
| Topics Extracted | Architecture, Experience, Spirituality, Infrastructure, Archaeology |

### 🔍 Notable Findings

- Indian heritage sites exhibit significantly stronger **spiritual sentiment** in visitor reviews
- Global sites score higher on **infrastructure satisfaction**
- Visitor experience patterns vary substantially by region and site type — pointing to meaningful cultural differences in how heritage is perceived and communicated

---

## 🧠 Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Folium |
| NLP | NLTK, TextBlob, VADER |
| Machine Learning | Scikit-learn |
| Topic Modeling | LDA (Latent Dirichlet Allocation) |
| Geo-Analytics | Folium (Interactive HTML Maps) |

---

## 📂 Project Structure

```
heritage-review-intelligence/
│
├── Heritage_Review_Intelligence.ipynb   # Main analysis notebook
├── requirements.txt                     # Python dependencies
├── README.md
├── .gitignore
│
├── data/                                # Raw and processed datasets
├── outputs/                             # Charts and visualizations
└── maps/                                # Interactive geo maps (HTML)
```

---

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/heritage-review-intelligence.git
cd heritage-review-intelligence
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Add datasets

Download the required datasets from Kaggle and place them inside the `/data` folder.

### 4. Run the notebook

```bash
jupyter notebook Heritage_Review_Intelligence.ipynb
```

---

## 📈 Methodology

### 1. Data Preprocessing
- Text cleaning and normalization
- Tokenization
- Stopword removal
- Lemmatization

### 2. Sentiment Analysis
- VADER sentiment scoring
- TextBlob polarity comparison and cross-validation

### 3. Machine Learning
- TF-IDF feature extraction
- Classifiers: Logistic Regression, Naive Bayes, Random Forest

### 4. Topic Modeling
- Latent Dirichlet Allocation (LDA) to surface dominant visitor themes

### 5. Geo-Analytics
- Folium-powered interactive world map
- Sentiment scores visualized by site location

---

## 🏛️ Heritage Sites Covered

| 🇮🇳 India | 🌍 Global |
|---|---|
| Taj Mahal, Agra | Colosseum, Italy |
| Hampi, Karnataka | Great Wall of China |
| Ajanta Caves, Maharashtra | Machu Picchu, Peru |
| Khajuraho Temples, Madhya Pradesh | Petra, Jordan |
| Qutb Minar, Delhi | Angkor Wat, Cambodia |

---

## 💡 Research & Business Value

- Helps tourism boards understand and act on visitor sentiment at scale
- Supports data-driven heritage preservation and infrastructure planning
- Enables cross-cultural benchmarking — relevant for UNESCO-style assessments
- Demonstrates practical application of NLP and ML to real-world cultural data

---

## 👩‍💻 Author

**Kaveri Koli**  
MSc Data Science (2025–2027)  
Dr. D. Y. Patil ACS College, Pune

---

## 📌 Academic Note

This project is part of the **Indian Knowledge Systems (IKS)** initiative under **NEP 2020**. It demonstrates applied competencies in Data Science, Natural Language Processing, and Machine Learning through the lens of cultural heritage analysis.

---

*If you found this project useful, consider starring the repository or reaching out for collaboration.*
