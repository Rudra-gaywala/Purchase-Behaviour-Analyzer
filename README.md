# 📊 Data Preprocessing & Feature Engineering Notebook

## 📌 Overview

This notebook demonstrates a complete **data preprocessing and feature engineering pipeline** using Python. It covers essential steps required to prepare raw data for machine learning models, including cleaning, transformation, encoding, scaling, and feature construction.

---

## 🧾 Dataset

* A synthetic dataset (CSV) with ~50 entries was used.
* Contains both **numerical** and **categorical** features.
* Includes columns such as:

  * Date
  * Customer ID
  * Purchase Amount
  * Categorical attributes

---

## ⚙️ Steps Performed

### 1. Data Loading

* Imported dataset using pandas
* Checked structure using:

  * `.head()`
  * `.info()`
  * `.describe()`

---

### 2. Handling Missing Values

* Used:

  * Mean/median imputation (numerical)
  * Most frequent imputation (categorical)

---

### 3. Outlier Detection & Treatment

* **Z-Score Method**
* **IQR Method**
* **Winsorization** (capping extreme values instead of removing)

---

### 4. Feature Transformation

* Log transformation
* Square root transformation
* Applied based on skewness

---

### 5. Feature Encoding

* **Label Encoding** → Binary variables
* **One-Hot Encoding** → Nominal variables
* **Ordinal Encoding** → Ordered categories

---

### 6. Date Feature Extraction

* Converted date column into:

  * Day
  * Month
  * Year

---

### 7. Feature Construction

Created new meaningful features:

* **Average Monthly Spend per Customer**
* **Purchase Frequency**
* **Days Since Last Purchase (Recency)**

---

### 8. Binning

* Converted continuous variables into categories:

  * Equal-width binning
  * Custom binning (e.g., young, adult, senior)

---

### 9. Feature Scaling

* **Min-Max Scaling**
* **Standardization (StandardScaler)**

---

### 10. Final Dataset

* Cleaned and transformed dataset saved as:

```bash
cleaned_data.csv
```

---

## 📦 Libraries Used

* pandas
* numpy
* scikit-learn
* scipy

---

## 📈 Key Learnings

* Importance of handling missing data and outliers
* Choosing correct encoding techniques
* Feature transformation improves model performance
* Feature engineering adds strong predictive power

---

## 🚀 How to Run

1. Open the notebook in Jupyter Notebook / VS Code
2. Run cells sequentially
3. Ensure required libraries are installed:

```bash
pip install pandas numpy scikit-learn scipy
```

---

## 📁 Project Structure

```
project/
│
├── data/
│   ├── raw/
│   └── processed/
│       └── cleaned_data.csv
│
├── project.ipynb
└── README.md
```

---

## 📌 Conclusion

This notebook provides a **complete end-to-end preprocessing pipeline** suitable for machine learning workflows. It demonstrates best practices in:

* Data cleaning
* Feature engineering
* Data transformation

---
