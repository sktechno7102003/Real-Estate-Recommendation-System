# 🏡 Real Estate Insight Engine & Recommender

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B)
![Model](https://img.shields.io/badge/Model-Random%20Forest-green)
![Scraper](https://img.shields.io/badge/Scraper-Selenium-yellow)

> **From raw data to smart property decisions.** An end-to-end platform that scrapes real-time market data to predict property prices with 90% accuracy and recommends similar listings using vector similarity.

---

## 🚀 Overview

The real estate market is opaque and data-fragmented. This project solves that by building a self-reliant data pipeline. Instead of using pre-baked datasets, I engineered a **custom Selenium scraper** to gather fresh market data, ensuring the model reflects current realities.

The platform serves two core purposes:
1.  **Valuation:** Estimating property prices using an optimized Random Forest Regressor.
2.  **Discovery:** Helping users find similar properties through a content-based recommendation system.

## ✨ Key Features

* **🕷️ Autonomous Data Collection:** Built a robust **Selenium scraper** to mine **3,000+ property listings**, handling dynamic content loading and pagination automatically.
* **🎯 Precision Feature Engineering:** Applied advanced selection techniques including **Recursive Feature Elimination (RFE)** and **Permutation Importance** to isolate the true drivers of property value.
* **🧠 High-Accuracy Modeling:** Trained a **Random Forest Regressor** with extensive hyperparameter tuning, achieving an **$R^2$ Score of 0.9**, significantly reducing prediction error.
* **🤝 Smart Recommendations:** Designed a user-configurable recommendation engine that computes **Cosine Similarity** across feature subspaces to find "look-alike" properties based on user preferences.
* **📊 Interactive Dashboard:** Fully deployed web interface built with **Streamlit** for real-time interaction.

---

## 🛠️ The Pipeline

1.  **Scraping:** Custom Selenium bots navigate property sites to extract raw HTML data.
2.  **Preprocessing:** Data cleaning pipeline handles missing value imputation and outlier detection.
3.  **Feature Selection:** RFE reduces dimensionality to the most impactful features.
4.  **Modeling:** Random Forest training with Cross-Validation.
5.  **Deployment:** Streamlit app integration for inference and recommendations.

---

## 🏆 Performance

| Metric | Score | Description |
| :--- | :--- | :--- |
| **$R^2$ Score** | **0.90** | Explains 90% of the variance in property prices. |
| **Data Volume** | **3K+** | Unique listings scraped and processed. |

*The model effectively captures non-linear relationships between location, amenities, and price.*

---

## 💻 Tech Stack

* **Language:** Python
* **Web Scraping:** Selenium
* **Machine Learning:** Scikit-Learn (Random Forest, RFE), Pandas, NumPy
* **Web Framework:** Streamlit
* **Data Viz:** Matplotlib/Seaborn

## 📦 Installation

```bash
# Clone the repository
git clone [https://github.com/yourusername/Real-Estate-Insight.git](https://github.com/yourusername/Real-Estate-Insight.git)

# Install dependencies
pip install -r requirements.txt
