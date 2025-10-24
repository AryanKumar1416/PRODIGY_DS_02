# Titanic Survival Prediction 🚢

![Python](https://img.shields.io/badge/Python-3.11-blue) ![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-brightgreen) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-yellow)

Predict passenger survival on the Titanic using exploratory data analysis (EDA) and machine learning.

---

## 📖 Project Overview

This project performs a full data analysis and builds a predictive model for the Titanic dataset:

1. **Data Loading & Exploration** – Inspect dataset, check missing values, and view descriptive statistics.  
2. **Data Cleaning & Preprocessing** – Handle missing values, drop irrelevant columns.  
3. **Exploratory Data Analysis (EDA)** – Visualize distributions, correlations, and survival patterns.  
4. **Feature Engineering** – Create `FamilySize`, `IsAlone`, and extract `Title` from names.  
5. **Feature Encoding & Scaling** – One-hot encode categorical variables and scale numerical features.  
6. **Model Training & Evaluation** – Train a Logistic Regression model and evaluate performance using accuracy, precision, recall, and F1-score.  

---

## 📊 Key Insights from EDA

* Female passengers had higher survival rates than males.  
* Passengers in 1st class had higher chances of survival.  
* Traveling alone decreased survival probability.  
* Certain titles (`Mr`, `Mrs`, `Miss`) correlate with survival outcomes.

---

## 🛠 Technologies Used

* **Python** – Data processing and modeling  
* **Pandas & NumPy** – Data manipulation  
* **Matplotlib & Seaborn** – Data visualization  
* **Scikit-learn** – Machine learning & evaluation  

---

## ⚡ Installation & Usage

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/titanic-survival-prediction.git
   cd titanic-survival-prediction
