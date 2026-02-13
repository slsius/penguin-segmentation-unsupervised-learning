# Unsupervised Clustering Case Study – Penguin Segmentation

## 📌 Project Overview

This project applies unsupervised machine learning techniques to segment penguin observations into natural groupings based on physical characteristics.

The objective was to identify underlying structure within the dataset and determine the optimal number of clusters using objective evaluation methods.

This case study demonstrates structured data preprocessing, exploratory analysis, model selection, clustering implementation, and analytical interpretation.

---

## 📊 Dataset Description

The dataset contains physical measurements of penguins collected in Antarctica:

| Column | Description |
|--------|------------|
| culmen_length_mm | Culmen length (mm) |
| culmen_depth_mm | Culmen depth (mm) |
| flipper_length_mm | Flipper length (mm) |
| body_mass_g | Body mass (g) |
| sex | Penguin sex |

Species labels were excluded during modelling to simulate a real-world unsupervised learning scenario.

---

## 🧠 Methodology

### 1️⃣ Data Cleaning & Preparation

- Removed missing or inconsistent records
- Encoded categorical variable (`sex`)
- Standardised numerical features using `StandardScaler`
- Verified feature distributions and relationships

---

### 2️⃣ Exploratory Data Analysis (EDA)

- Visualised feature distributions
- Analysed correlations between physical attributes
- Assessed separability across dimensions

---

### 3️⃣ Cluster Selection

The optimal number of clusters was determined using:

- **Elbow Method** (inertia analysis)
- **Silhouette Score** (cluster separation quality)

The value of **K was selected based on the strongest silhouette score and visual elbow inflection point**, ensuring a data-driven decision rather than assumption-based selection.

---

### 4️⃣ Clustering Implementation

- Applied K-Means clustering using the selected K value
- Evaluated cluster compactness and separation
- Visualised clusters using PCA dimensionality reduction

---

## 🔎 Key Findings

- Distinct clusters emerged primarily differentiated by **body mass** and **flipper length**
- Silhouette analysis confirmed meaningful separation between clusters
- PCA visualisation demonstrated clear segmentation patterns
- Results illustrate how unsupervised learning can identify natural groupings within structured datasets

---

## 🛠 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- StandardScaler  
- KMeans  
- PCA  

---

## 📁 Repository Structure
├── penguins.csv

├── clustering_notebook.ipynb

├── visualisations/

└── README.md

---

## 💼 Business Relevance

Unsupervised clustering techniques are widely used in commercial and enterprise environments for:

- Customer segmentation  
- Risk categorisation  
- Fraud detection  
- Behavioural profiling  
- Market analysis  

This project demonstrates the ability to:

- Prepare and transform structured datasets  
- Select models using objective evaluation techniques  
- Interpret cluster outputs analytically  
- Document methodology in a reproducible format  

---

## 🚀 Skills Demonstrated

- Data cleaning & preprocessing  
- Feature scaling & encoding  
- Unsupervised machine learning  
- Model evaluation (Elbow & Silhouette)  
- Dimensionality reduction (PCA)  
- Analytical interpretation  
- Structured documentation  
