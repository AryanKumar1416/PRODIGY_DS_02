# Titanic Survival Prediction - Exploratory Data Analysis & Machine Learning

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** and builds a **Logistic Regression model** to predict passenger survival on the **Titanic** dataset.

The goal is to understand the key factors affecting survival and develop a machine learning pipeline that includes **data preprocessing, feature engineering, model training, and evaluation**.

---

## 📁 Dataset

The dataset used is from the **Titanic survival challenge**. It contains passenger details such as:

| Feature | Description |
|---------|-------------|
| Pclass  | Passenger class (1st, 2nd, 3rd) |
| Sex     | Gender of the passenger |
| Age     | Age in years |
| SibSp   | Number of siblings/spouses aboard |
| Parch   | Number of parents/children aboard |
| Fare    | Passenger fare |
| Embarked| Port of embarkation |
| Survived| Target variable (0 = No, 1 = Yes) |

---

## 🧹 Data Cleaning & Preprocessing

- Missing values in **Age** were imputed using the **median**.
- Missing values in **Embarked** were **removed**.
- **Cabin** was **dropped** due to excessive missing data.
- Created new features:
  - `FamilySize` → SibSp + Parch + 1
  - `IsAlone` → 1 if FamilySize == 1, else 0
  - `Title` → Extracted from Name

---

## 📊 Exploratory Data Analysis (EDA)

- Value counts of **Survived**, **Sex**, and **Pclass**
- Count plots showing survival distribution across **gender and class**
- **Age distribution histogram**
- **Correlation heatmap** to identify strong relationships
- **Violin plot**: Age vs Survival by Pclass
- **Scatter plot**: Fare vs Age

---

## 🔢 Feature Encoding & Scaling

- Applied **One-Hot Encoding** to categorical variables (`Sex`, `Embarked`, `Title`)
- Standardized numerical features (`Age`, `Fare`, `FamilySize`, etc.) using **StandardScaler**

---

## 🧠 Model Training

- Split the dataset into **Training (X_train, y_train)** and **Testing sets**
- Trained a **Logistic Regression model**
- Evaluated using:
  - ✅ Accuracy
  - ✅ Precision
  - ✅ Recall
  - ✅ F1-Score

---

## ✅ Conclusion

The project demonstrates a complete **end-to-end data science workflow**:

✔️ Data Cleaning  
✔️ EDA and Visualization  
✔️ Feature Engineering  
✔️ Model Training & Evaluation  

The **Logistic Regression model performed well**, but future enhancements may include:

- Trying **Random Forest / XGBoost / SVM**
- **Hyperparameter tuning**
- Advanced **feature selection techniques**

---

## 🚀 How to Run the Project

```bash
# Clone the repository
git clone <your-repo-link>

# Install required libraries
pip install -r requirements.txt

# Open the notebook
jupyter notebook Titanic_EDA_Model.ipynb
