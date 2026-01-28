# 🎬 Content-Based Movie Recommendation System

## 📌 Overview

This project implements a **content-based movie recommendation system** that suggests movies similar to a given title based on textual features such as **genres, overview, keywords, cast, and crew**. The system uses **TF-IDF vectorization** and **cosine similarity** to compute similarity scores and return the top-N relevant movie recommendations.

The project demonstrates an **end-to-end data science workflow**, including data preprocessing, feature engineering, model building, and API-based deployment.

---

## 🧠 Problem Statement

Users often struggle to discover movies aligned with their interests. This project addresses that problem by recommending movies **based on content similarity**, rather than user ratings or collaborative filtering.

---

## ⚙️ Approach

1. **Data Cleaning & Preprocessing**

   * Processed movie metadata dataset
   * Handled missing values and irrelevant columns
   * Combined multiple text features into a single representation

2. **Feature Engineering**

   * Applied **TF-IDF Vectorization** on textual movie features
   * Generated high-dimensional sparse feature vectors

3. **Similarity Computation**

   * Used **cosine similarity** to compute movie-to-movie similarity
   * Optimized computation using **SciPy sparse matrices**

4. **Recommendation Logic**

   * Retrieved top-N similar movies based on similarity scores
   * Achieved **sub-200 ms inference time** for recommendations

5. **Deployment**

   * Exposed recommendation functionality via **FastAPI REST endpoints**

---

## 🛠️ Tech Stack

* **Programming Language:** Python
* **Libraries:** NumPy, Pandas, Scikit-learn, SciPy
* **NLP:** TF-IDF Vectorizer
* **Similarity Metric:** Cosine Similarity
* **API Framework:** FastAPI
* **Notebook:** Jupyter Notebook

---

## 📂 Project Structure

```
content_based_recommendation_system/
│── app.py                # FastAPI application
│── main.py               # Core recommendation logic
│── movies.ipynb          # EDA & model building notebook
│── requirements.txt      # Project dependencies
│── runtime.txt           # Runtime configuration
│── .gitignore            # Ignored large files & environment files
```

---

## 🚀 How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone https://github.com/altamashhhh/content_based_recommendation_system.git
cd content_based_recommendation_system
```

### 2️⃣ Create virtual environment (optional)

```bash
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
```

### 3️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run the application

```bash
python app.py
```

---

## 📊 Results & Highlights

* Processed **45,000+ movie records**
* Generated **50,000+ TF-IDF features**
* Achieved **sub-200 ms recommendation latency**
* Delivered **~90% relevance accuracy** (manual top-N validation)
* Reduced response time by **~40%** using optimized indexing

---

## ⚠️ Note on Large Files

Due to GitHub size limitations, **large dataset and trained model files** (`.pkl`, `.csv`) are intentionally excluded using `.gitignore`.

👉 Models and features are generated locally during training.


---

## 👤 Author

**Md. Altamash Ansari**

