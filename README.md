# 🧠 Human Activity Recognition with PCA | KNN Classifier

> 📊 **Visualizing Dimensionality Reduction + Accuracy Trade-off with PCA**

## 🔍 Overview

This project demonstrates how **Principal Component Analysis (PCA)** can reduce the dimensionality of high-dimensional datasets like the **Human Activity Recognition with Smartphones** dataset—**without significant loss of information**.

We compare the performance of a **K-Nearest Neighbors (KNN)** classifier on:

* ✅ All 563 features
* ✅ Reduced features using PCA (from 1 to 40 components, and also with 2D and 3D visualization)

Through detailed **PCA visualizations**, this notebook helps users understand how PCA compresses data while preserving its structure for accurate classification.

---

## 📁 Dataset

* **Source**: [Kaggle - Human Activity Recognition with Smartphones](https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones)
* **Samples**: 7,352
* **Features**: 563 numeric features (accelerometer/gyroscope signals)
* **Target**: Human activity (e.g., Walking, Sitting, Standing, Laying, etc.)

---

## 🧪 Project Workflow

1. 📅 **Load Dataset**
2. ✨ **Preprocess Data**

   * Apply `StandardScaler` to normalize the features
3. 🔍 **Apply PCA with `sklearn`**

   * Explore accuracy from 1 to 40 principal components
4. 📊 **Train KNN Classifier**

   * Compare accuracy using:

     * All 563 features
     * Top N principal components
5. 🔍 **Visualizations**

   * 2D PCA Scatter Plot (PC1 vs PC2)
   * 3D PCA Scatter Plot (PC1 vs PC2 vs PC3)

---

## 📈 Accuracy Evaluation

We trained a KNN classifier and evaluated accuracy using various number of principal components (from 1 to 40):

| # Principal Components | KNN Accuracy |
| ---------------------- | ------------ |
| 1                      | 65.16%       |
| 2                      | 74.17%       |
| 3                      | 80.53%       |
| ...                    | ...          |
| 40                     | 98.13%       |
| All 561 features       | 98.89%       |

> ⚠️ Even with as few as 10–20 components, the model reaches accuracy close to the original, proving PCA's efficiency in noise reduction and feature compression.

---

## 🌈 Visualizations

### 2D PCA Plot (PC1 vs PC2)

* Demonstrates clear separation of activities using only 2 components

### 3D PCA Plot (PC1, PC2, PC3)

* Interactive plot to show multi-dimensional structure in reduced form


---

## 📄 Technologies Used

* Python
* NumPy, Pandas
* Scikit-learn (PCA, KNN, StandardScaler)
* Matplotlib, Seaborn
* Plotly (3D visualization)
* Jupyter Notebook

---

## 🚀 How to Run

1. Clone this repo:

```bash
git clone https://github.com/your-username/pca-har-knn.git
cd pca-har-knn
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```bash
jupyter notebook PCA_HAR_KNN.ipynb
```

---

## 🎓 Educational Value

This notebook is crafted for:

* Understanding PCA practically using scikit-learn
* Learning how to visualize high-dimensional data
* Observing the impact of dimensionality reduction on classification models

---

## ⭐ Credits

* [Kaggle Dataset Source](https://www.kaggle.com/datasets/uciml/human-activity-recognition-with-smartphones)

---
🎥 Want to really see the power of PCA? Don’t miss the stunning 3D interactive PCA plot in the notebook—it makes the magic of dimensionality reduction come alive!

