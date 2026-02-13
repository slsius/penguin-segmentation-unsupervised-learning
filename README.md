# Unsupervised Clustering Case Study – Penguin Species Segmentation

## 📌 Project Overview

This project applies unsupervised machine learning techniques to segment penguin observations into distinct groups based on physical characteristics.

The objective was to identify natural clusters within the dataset and determine whether clustering methods could meaningfully separate species without labelled data.

This project demonstrates structured data preprocessing, exploratory analysis, clustering model implementation, and evaluation.

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
- Checked feature distributions and correlations

---

### 2️⃣ Exploratory Data Analysis (EDA)

- Visualised feature distributions
- Analysed relationships between culmen dimensions and body mass
- Assessed separability of potential clusters

---

### 3️⃣ Model Selection

Applied **K-Means Clustering**:

- Tested multiple values of K
- Used the **Elbow Method** to determine optimal cluster number
- Evaluated inertia score for cluster compactness

---

### 4️⃣ Model Evaluation

- Compared clustering output to known species (for validation only)
- Analysed centroid characteristics
- Visualised cluster separation
- Interpreted feature importance across clusters

---

## 🔎 Key Findings

- Optimal cluster number identified: **K = 3**
- Body mass and flipper length were primary differentiators
- Clear separation observed between Gentoo and Adelie clusters
- Chinstrap showed partial overlap due to feature similarity

This demonstrates how unsupervised learning can uncover natural segmentation patterns in structured datasets.

---

## 🛠 Tools & Technologies

- Python  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- Scikit-learn  
- StandardScaler  
- KMeans  

---

## 📁 Repository Structure
├── penguins.csv

├── clustering_notebook.ipynb

├── visualisations/

└── README.md


---

## 💼 Business Relevance

Clustering techniques are widely used in commercial and enterprise environments for:

- Customer segmentation  
- Risk categorisation  
- Fraud detection  
- Behavioural profiling  
- Market analysis  

This project demonstrates foundational capability in applying structured unsupervised learning techniques to real-world analytical problems.

---

## 🚀 Skills Demonstrated

- Data cleaning & preprocessing  
- Feature scaling & transformation  
- Unsupervised machine learning  
- Model evaluation techniques  
- Analytical interpretation of results  
- Structured documentation of analytical workflow  

