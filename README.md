<h1 align="center">📘 Student Study Habit Prediction Model 🎓</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9-blue.svg" />
  <img src="https://img.shields.io/badge/ML%20Techniques-Regression%2C%20EDA%2C%20Hyperparameter%20Tuning-orange.svg" />
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen" />
</p>

---

## 🧠 Project Overview

The **Student Study Habit Prediction Model** aims to **analyze students' behaviors and backgrounds** to **predict their academic performance**.

This project demonstrates:
- Data cleaning and preprocessing
- Feature transformation and encoding
- Exploratory Data Analysis (EDA)
- Regression modeling (Linear, Ridge, Lasso, ElasticNet, Random Forest, XGBoost)
- Hyperparameter tuning
- Evaluation and comparison of models

---

## 📁 Dataset

The dataset used is named `student_study_habits.csv`. It is:
- Clean (no null values)
- Scaled and transformed
- One-hot encoded for categorical columns

> 🔍 Example Features:
- Gender, parental education
- Study hours, internet access
- Participation level, health index
- Final Grade (Target variable)

---

## 📊 Exploratory Data Analysis (EDA)

EDA techniques used:
- Histogram plots of all features
- Correlation matrix (heatmap)
- Encoding impact of categorical variables:
  - **Participation Level** shows low correlation with grades → label encoding.
  - **Parental Education** shows strong influence → ordinal encoding with priority:
    ```
    High School < Master's < PhD
    ```

---

## 🧪 Preprocessing & Feature Engineering

- Merged one-hot encoded columns into single categorical columns
- Applied **Ordinal Encoding** for hierarchical categorical variables
- Split data into training and testing sets
- Ensured proper scaling before feeding to models

---

## 🤖 Models Used

Implemented and compared multiple **regression models**:
- 📐 **Linear Regression**
- 🧲 **Ridge & Lasso Regression**
- 🔀 **ElasticNet**
- 🌲 **Random Forest Regressor**
- ⚡ **XGBoost Regressor**

Each model was evaluated based on:
- R² Score
- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- RMSE (Root Mean Squared Error)

---

## 🎯 Hyperparameter Tuning

Used `RandomizedSearchCV` to tune:
- **Random Forest Regressor** (n_estimators, max_depth, etc.)

This boosted performance significantly by finding the best parameter set.

---

## 📈 Performance Comparison

Each model's performance was collected into a summary dictionary for side-by-side comparison.

> 📌 Example output:
```python
{
  'Linear Regression': {'R2 Score': 0.78, 'MAE': 2.3, 'RMSE': 3.1},
  'Random Forest': {'R2 Score': 0.89, 'MAE': 1.8, 'RMSE': 2.4},
  ...
}
```

Random Forest and XGBoost performed the best among all.

---

## 📌 Key Learnings

- Categorical data needs careful encoding based on domain knowledge.
- Even seemingly unimportant features like "internet access" can impact performance.
- Tree-based models often outperform linear ones when handling categorical + numerical mix.
- Model interpretability and performance evaluation are equally important.

---

## 📦 Requirements

Typical libraries used:
```bash
numpy
pandas
matplotlib
seaborn
scikit-learn
xgboost
```

---

## 🖼️ Sample Visuals

> *(Add your image links or screenshots if desired)*

- 📊 Correlation Heatmap
- 📉 Model Error Distribution
- 📈 Feature Importance from Random Forest

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Rakib61491/Student-Study-Habits-Analysis-with-Machine-Learning.git

   ```

2. Run the notebook:
   ```
   Student Study Habit Prediction Model.ipynb
   ```

---

## 🙌 Author

**MR. Rakib**  
_Student • ML Enthusiast • Data Explorer_

> Feel free to connect on [LinkedIn](https://www.linkedin.com/in/mr--rakib/)
> Connect with me in Kaggle [Kaggle])(https://www.kaggle.com/mrrakib0886)
> 
---

## ⭐ If you found this useful...

Give it a ⭐ and share the repo!  
Your feedback and ideas are welcome!
