# 🎬 CineMatch: AI Movie Recommendation System

**Collaborative Filtering-Based Movie Recommender**



## 📋 Project Overview

In the era of streaming platforms like **Netflix** and **Amazon Prime**, users often face **analysis paralysis** due to an overwhelming number of choices.

**CineMatch** is an intelligent movie recommendation system that learns user preferences from past ratings and predicts movies they are likely to enjoy using **Collaborative Filtering techniques**.



## ⚙️ Implemented Approaches

* 🔹 Memory-Based Collaborative Filtering

  * User-User Similarity (Cosine Similarity)
  * Item-Item Similarity

* 🔹 Model-Based Collaborative Filtering

  * Matrix Factorization using **SVD (Singular Value Decomposition)**
  * Hyperparameter tuning for performance optimization

* 🔹 Evaluation Metrics

  * RMSE (Root Mean Square Error)
  * MAE (Mean Absolute Error)
  * Precision@K
  * Recall@K

* 🔹 Baseline Model

  * Popularity-Based Recommendation (for cold start problem)

---

## 📊 Dataset Information

* **Dataset**: MovieLens Small Dataset
* **Total Ratings**: 100,836
* **Total Movies**: 9,742
* **Total Users**: 610
* **Sparsity**: 98.30%

---

## 🛠️ Technologies Used

* **Python**
* pandas, numpy
* matplotlib, seaborn
* scikit-learn
* scikit-surprise

---

## 📁 Project Structure

```
CineMatch_Project/
├── CineMatch_Recommendation_System.ipynb
├── CineMatch_Report.pdf
├── CineMatch_Presentation.pptx
├── README.md
├── requirements.txt
├── ratings.csv
└── movies.csv
```

---

## 📈 Key Results

| Model               | Type            | RMSE       | MAE        | Precision@10 | Recall@10  |
| ------------------- | --------------- | ---------- | ---------- | ------------ | ---------- |
| Popularity Baseline | Baseline        | -          | -          | -            | -          |
| User-User KNN       | Memory-Based    | 0.9823     | 0.7578     | -            | -          |
| Item-Item KNN       | Memory-Based    | 0.9800     | 0.7532     | -            | -          |
| **SVD (Tuned)**     | **Model-Based** | **0.8613** | **0.6630** | **0.7507**   | **0.5236** |

🏆 **Best Performing Model: SVD (Tuned)**

---

## ❄️ Cold Start Handling

For new users with no prior ratings:

1. Recommend **popular movies**
2. Ask users to rate 5–10 movies during onboarding
3. Transition to a **hybrid recommendation system**

---

## 🚀 How to Run the Project

### 1️⃣ Open Anaconda Prompt

Launch Anaconda Prompt on your system.

### 2️⃣ Create & Activate Environment (First Time Only)

```
conda create -n cine_env python=3.9
conda activate cine_env
pip install -r requirements.txt
```

### 3️⃣ Activate Environment

```
conda activate cine_env
```

### 4️⃣ Navigate to Project Directory

```
cd "path_to_your_project_folder"
```

### 5️⃣ Launch Jupyter Notebook

```
jupyter notebook
```

### 6️⃣ Run the Notebook

Open **CineMatch_Recommendation_System.ipynb** and run all cells.

---

## 🔮 Future Improvements

* 🔹 Hybrid Model (Collaborative + Content-Based using TF-IDF)
* 🔹 Add diversity and serendipity in recommendations
* 🔹 Deploy as a web app (Streamlit / Flask)
* 🔹 Implement Neural Collaborative Filtering
* 🔹 Add advanced metrics like NDCG@K and Coverage

---

## 📦 Deliverables

* 📓 Jupyter Notebook (Full implementation)
* 📄 PDF Report
* 📊 PowerPoint Presentation
* 📂 Dataset files
* 📜 requirements.txt

---

## ⭐ Acknowledgements

* MovieLens Dataset (GroupLens Research)

---

## 💡 Author

**G Pranav Reddy**

---
