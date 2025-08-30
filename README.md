# Diabetes Prediction with Logistic Regression (Python)

This project implements a **machine learning pipeline in Python** for predicting diabetes using the **Pima Indians Diabetes Dataset**. The workflow demonstrates the complete process of **data preprocessing, feature engineering, model training, and evaluation**.

## Key Steps

1. **Data Loading & Exploration**
   - Loaded dataset using **pandas** and assigned descriptive column names.
   - Performed exploratory data analysis (EDA) with **Matplotlib** and **Seaborn**.

2. **Data Cleaning & Preprocessing**
   - Replaced invalid `0` entries with `NaN` and handled missing values.
   - Applied **mean imputation** for Insulin and **median imputation** for other numeric features using `SimpleImputer`.
   - Dropped irrelevant features (e.g., *Pregnancies*) to improve model performance.

3. **Feature Engineering**
   - Split dataset into features (**X**) and target (**Y**: diabetic = 1, non-diabetic = 0).
   - Normalized/standardized features to prepare for model training.

4. **Modeling**
   - Split data into training and test sets with `train_test_split`.
   - Trained a **Logistic Regression** model using **scikit-learn**.

5. **Evaluation**
   - Achieved an **accuracy score of ~77.6%**.
   - Assessed performance using a **confusion matrix**.
   - Compared actual vs. predicted labels for interpretability.

## Tools & Libraries

- **Python** (Jupyter Notebook)
- **Pandas, NumPy** – Data manipulation
- **Matplotlib, Seaborn** – Visualization
- **scikit-learn** – Preprocessing, Logistic Regression, Model Evaluation

## Results & Insights

- The model reached **77.6% accuracy**, which is a solid baseline for logistic regression on this dataset.  
- From the **confusion matrix**:
  - The model performs well in predicting **non-diabetic (label = 0)** cases.  
  - Some misclassifications occur in **diabetic (label = 1)** cases, which is common in imbalanced datasets.  
- Insights suggest that improving feature engineering (e.g., handling outliers, feature scaling, or using advanced models like Random Forest or XGBoost) could increase predictive performance.  

---
