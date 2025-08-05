# ❤️ Heart Disease Prediction using Logistic Regression

## 🧠 Project Overview

This project aims to build a reliable heart disease prediction system using machine learning. It involves extensive data preprocessing, exploratory data analysis, statistical testing, and training a logistic regression model on cleaned data. The model helps in predicting whether a person is likely to have heart disease based on various medical parameters.

---

## 📂 Dataset

The dataset contains patient-level information like:

- Age
- Gender
- Chest Pain Type
- Blood Pressure
- Cholesterol
- Max Heart Rate
- Presence or Absence of Heart Disease (target variable)

**Total Entries:** 270  
**Features Used:** 6 (after preprocessing)

---

## 🧹 Data Preprocessing

- ✅ Handled missing values (none found)
- ✅ Removed duplicate records
- ✅ Renamed columns for clarity
- ✅ Dropped unnecessary features:
  - FBS over 120, EKG results, Exercise angina, ST depression, Slope of ST, Number of vessels fluro, Thallium

---

## 📊 Exploratory Data Analysis (EDA)

### ✅ Univariate Analysis:
- Frequency distributions and histograms for:
  - Age, Gender, Chest Pain Type, Blood Pressure, Cholesterol, Max Heart Rate
- Count plots for Gender and Chest Pain Types

### ✅ Bivariate Analysis:
- Plots showing the relationship between:
  - Age vs Cholesterol
  - Age vs Blood Pressure
  - Gender vs Max Heart Rate

---

## 🔬 Statistical Analysis

### ✅ Correlation Heatmap:
- Revealed strong correlations between some features.

### ✅ Hypothesis Testing:
1. **High Cholesterol causes more heart disease?**
   - ❌ Null not rejected (p = 0.0527)

2. **Males have more heart disease than females?**
   - ✅ Null rejected (p < 0.00001)

---

## 🤖 Model Training

- **Model Used:** Logistic Regression
- **Target Variable:** Heart Disease (binary: 0 = Absence, 1 = Presence)
- **Training Ratios Tested:** 80%, 60%, and 50%

### 🔍 Results Summary:

| Split | Accuracy | Precision | Recall | MAE   |
|-------|----------|-----------|--------|--------|
| 80%   | 92.6%    | 94.7%     | 85.7%  | 0.0741 |
| 60%   | 74.1%    | 72.0%     | 62.2%  | 0.2593 |
| 50%   | 72.6%    | 66.0%     | 67.2%  | 0.2741 |

---

## 📈 Evaluation Metrics

- ✅ **Confusion Matrix**
- ✅ **Classification Report** (Precision, Recall, F1-Score)
- ✅ **Mean Absolute Error (MAE)**

Confusion matrices were visualized using heatmaps for clarity.

---

## 💡 Final Conclusion

> The logistic regression model performed best with an 80/20 train-test split, achieving **92.6% accuracy** and **high precision**, showing its reliability in identifying heart disease cases. However, recall values suggest room for improvement in minimizing false negatives.

---

## 🧠 Learning Outcomes
- Learned how to clean, preprocess, and visualize real-world health data
- Developed end-to-end data analysis skills, including statistical hypothesis testing
- Built and tuned a logistic regression model using scikit-learn
- Learned to evaluate models using confusion matrix, classification report, and MAE
- Gained hands-on experience with bivariate analysis and heatmap correlation
- Improved interpretation skills in healthcare-related machine learning

## 🚀 How to Run

### 🛠️ Requirements
- Python 3.x
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `scipy`

### 💻 Steps to Execute

1. Clone the repository or download the notebook.
2. Install the required libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy
