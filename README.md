# customer-churn-prediction

## Bank Customer Churn Prediction

This project develops a machine learning classification model to predict customer churn in a banking environment. By identifying customers who are highly likely to leave the bank, the institution can proactively design and execute customer retention strategies.

### 📋 Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Machine Learning Workflow](#machine-learning-workflow)
- [Technologies & Libraries](#technologies--libraries)
- [Key Results](#key-results)
- [Conclusion & Next Steps](#conclusion--next-steps)

---

### 🔍 Project Overview
Customer churn represents one of the most critical metrics for consumer-facing businesses. This notebook walks through the end-to-end data science process to ingest, clean, explore, preprocess, and train a **Random Forest Classifier** to predict the target variable `Exited` (0 = Stayed, 1 = Left).

### 📊 Dataset
- **Name:** Bank Customer Churn Dataset
- **Size:** 10,000 records
- **Target Variable:** `Exited`

### ⚙️ Machine Learning Workflow
1. **Data Ingestion & Cleaning:** Handled missing values and dropped structurally irrelevant columns (e.g., `RowNumber`, `CustomerId`, `Surname`).
2. **Exploratory Data Analysis (EDA):** Visualized churn ratios, geographic distributions, gender gaps, and age histograms to understand behavior patterns.
3. **Statistical Analysis:** Generated summary statistics and correlation heatmaps.
4. **Preprocessing:** Split data into features ($X$) and target ($y$), performed One-Hot Encoding on categorical features (`Geography`, `Gender`), applied stratified train-test splitting (80:20), and normalized the data using `StandardScaler`.
5. **Model Training:** Built a baseline `Random Forest Classifier` and optimized it using class weight balancing and hyperparameter constraints.
6. **Evaluation:** Generated Confusion Matrices and Classification Reports (Precision, Recall, F1-Score, and Accuracy).

### 🛠️ Technologies & Libraries
- **Language:** Python
- **Data Manipulation:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`
- **Machine Learning:** `scikit-learn`
- **Environment:** Google Colab

### 🏆 Key Results
- **Base Accuracy:** ~86.4%
- **Model Feature Engineering:** Successfully addressed categorical features using dynamic dummy variables.
- **Improved Random Forest Model:** Configured class balancing to improve prediction recall metrics on minority classes.
