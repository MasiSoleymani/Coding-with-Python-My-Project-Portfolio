Diabetes Prediction with Logistic Regression

This notebook presents a complete machine learning pipeline for predicting diabetes using the Pima Indians Diabetes dataset. The workflow covers data preprocessing, missing value imputation, model training, and evaluation.

Dataset
	•	Source: diabetes.data
	•	Features include: Glucose, BloodPressure, SkinThickness, Insulin, BMI, Age, and more.
	•	Target: label (1 = diabetic, 0 = non-diabetic)

 Key Steps
	1.	Data Cleaning:
	•	Renamed unnamed columns using appropriate feature names
	•	Replaced invalid 0 values with NaN and imputed them using:
	•	Mean for Insulin
	•	Median for other numeric features using SimpleImputer
	2.	Feature Engineering:
	•	Dropped irrelevant features like Pregnancies
	•	Separated features (X) and labels (Y)
	3.	Modeling:
	•	Split the data into training and test sets
	•	Trained a Logistic Regression model from sklearn
	•	Evaluated using:
	•	Accuracy Score: ~77%
	•	Confusion Matrix
	•	Prediction Comparison
