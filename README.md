# 🏠 Bengaluru House Price Prediction

This project involves building a machine learning model to predict house prices in Bengaluru using regression techniques. The workflow includes exploratory data analysis (EDA), data cleaning, outlier detection, feature engineering, and model training.

---

## 📂 Dataset

- **Source**: `Bengaluru_House_Data.csv`
- **Features**:
  - `location`
  - `size` (e.g., 2 BHK, 3 BHK)
  - `total_sqft`
  - `bath`
  - `price` (in lakhs)

---

## 📊 EDA & Data Cleaning

Key steps:

- Handled missing values and inconsistent data.
- Created a new feature: **`price_per_sqft`**.
- Standardized `size` to numerical BHK.
- Removed outliers based on:
  - `total_sqft` per BHK
  - `price_per_sqft` standard deviations
  - Price variations within the same location

---

## 🛠️ Feature Engineering

- One-hot encoded the `location` column (after dimensionality reduction).
- Converted `size` to BHK.
- Final dataset prepared with selected features for model training.

---

## 🤖 Model Building

- **Algorithm Used**: Linear Regression
- **Train/Test Split**: 80/20
- **Performance Metric**: R² score

> 📌 Other models (e.g., Lasso, Decision Tree, etc.) can also be explored to improve performance.

---

## 📈 Results

- **Model Accuracy**: Around ~80% R² score (can vary depending on split).
- The model gives fairly reasonable estimates for most common locations and sizes.

---

## 🚀 How to Run

1. Clone the repo or download the `.ipynb` file.
2. Install required libraries:

   ```bash
   pip install pandas numpy matplotlib scikit-learn
