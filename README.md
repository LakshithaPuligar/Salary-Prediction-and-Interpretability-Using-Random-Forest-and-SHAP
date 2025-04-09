Project Overview: The goal of this project is to forecast employee pay based on a number of professional and demographic characteristics, including job title, years of experience, gender, age, and education level. Predictions are made using a Random Forest Regressor model, and interpretability is provided by integrating SHAP (Shapley Additive Explanations), which explains how each attribute contributes to the model's prediction. A practical investigation of how modifications to particular attributes, such years of experience, impact the pay projections is also included in the project.
Important attributes:
Machine Learning for Predicting Salary: This project's main objective is to use machine learning techniques to forecast employee pay. The research makes use of the Random Forest Regressor algorithm, an ensemble learning technique that can simulate intricate correlations between the target variable (salary) and features.

Preprocessing Data:

The dataset contains both numerical (e.g., Age, Years of Experience) and categorical (e.g., Gender, Education, Job Title) variables.

The categorical variables are transformed into a format appropriate for machine learning algorithms by applying One-Hot Encoding.

The dataset is cleaned by removing any rows that have missing values and removing excessive spaces from column names.
Model Training: The preprocessed data is used to train the Random Forest Regressor, with the target variable (y) being employee salaries and the features (X) consisting of professional and demographic characteristics.

Interpretability of SHAP:

The output of the trained model is explained by the project using SHAP (Shapley Additive Explanations).

Understanding how each feature (such as Years of Experience and Education Level) contributes to a particular pay estimate is made easier with SHAP.

For a test sample, a waterfall plot is created to show the impact of each feature on the model's prediction.
Following model training, an intriguing experiment is carried out in which two years are added to one of the features (Years of Experience). This illustrates how this modification directly affects the salary forecast and offers information on how years of experience affect pay.

Evaluation and Findings: The model's predictive power for test data that hasn't been seen is used to assess its performance. It calculates and shows the difference in expected pay brought on by modifications to a feature (such adding years of experience).

Technologies and Libraries Used:
Pandas: For data loading, cleaning, and manipulation.

NumPy: For handling arrays and numerical operations.

Scikit-learn: For machine learning tools like RandomForestRegressor, data splitting, and preprocessing (OneHotEncoder).

SHAP: For explaining the model’s predictions using Shapley values.

Matplotlib: For plotting the SHAP waterfall plot.

Output and Results:
SHAP Waterfall Plot: A visualization showing how different features (e.g., Education Level, Years of Experience, Age, etc.) influence the predicted salary for a test sample.

Predicted Salary Comparison: The comparison between the original predicted salary and the new predicted salary after changing the years of experience.

Original Test Sample Features: The original values for the test sample that was selected for prediction.
