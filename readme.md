# Machine Learning Model for Predicting COVID-19 Patient Survival

The aim of this machine learning model is to predict whether a COVID-19 patient will survive or not based on their current symptoms, status, and medical history. The goal is to achieve an accuracy of 90% or higher.

## Dataset Information

- The dataset contains 21 features.
- It includes information for 1,048,575 unique patients.
- In the Boolean features, the value 1 indicates "yes," and 2 indicates "no."

## Features

1. `USMER`: Indicates whether the patient received medical treatment at the first, second, or third level.
2. `MEDICAL_UNIT`: Type of institution within the National Health System that provided the care.
3. `SEX`: Gender of the patient.
4. `PATIENT_TYPE`: Indicates whether the patient returned home or was hospitalized.
5. `DATE_DIED`: If the patient died, it indicates the date of death; otherwise, it is set to "9999-99-99."
6. `INTUBED`: Indicates whether the patient was connected to a ventilator.
7. `PNEUMONIA`: Indicates whether the patient already had air sac inflammation.
8. `AGE`: Age of the patient.
9. `PREGNANT`: Indicates whether the patient is pregnant.
10. `DIABETES`: Indicates whether the patient has diabetes.
11. `COPD`: Indicates whether the patient has Chronic Obstructive Pulmonary Disease (COPD).
12. `ASTHMA`: Indicates whether the patient has asthma.
13. `INMSUPR`: Indicates whether the patient is immunosuppressed.
14. `HIPERTENSION`: Indicates whether the patient has hypertension.
15. `OTHER_DISEASE`: Indicates whether the patient has other diseases.
16. `CARDIOVASCULAR`: Indicates whether the patient has heart or blood vessel-related diseases.
17. `OBESITY`: Indicates whether the patient is obese.
18. `RENAL_CHRONIC`: Indicates whether the patient has chronic renal disease.
19. `TOBACCO`: Indicates whether the patient is a tobacco user.
20. `CLASIFFICATION_FINAL`: COVID-19 test findings. Values 1-3 indicate different degrees of COVID-19 diagnosis, while 4 or higher means the patient is not a carrier or the test is inconclusive.
21. `ICU`: Indicates whether the patient had been admitted to an Intensive Care Unit (ICU).

## Getting Started

To use this machine learning model, you'll need to follow these steps:

1. **Install Required Libraries:** Make sure you have the necessary libraries installed. You can use numpy, pandas, seaborn, matplotlib, xgboost, sklearn, and imblearn for this project. You can install these libraries using pip:

   `pip install numpy pandas seaborn matplotlib xgboost scikit-learn imbalanced-learn`

2. **Data Preparation:** Ensure that you have the dataset (`covid19.csv`) available in the appropriate directory. You can adjust the file path in the code accordingly.

3. **Exploratory Data Analysis (EDA):** The project begins with an EDA to understand the dataset's structure, data types, and initial insights. You will handle missing values, encode categorical variables, and visualize the data.

4. **Training and Classification:** The machine learning model involves training classifiers like XGBoost, Random Forest, and Stochastic Gradient Descent (SGD). You will evaluate their accuracy and make predictions.

5. **Oversampling:** After analyzing the initial results, you may choose to experiment with oversampling techniques to improve the model's performance.

6. **Feature Importance:** The feature importance analysis helps you identify the most relevant features for the model's predictions.

# Results

- The initial models, including XGBoost, Random Forest, and SGD, provide relatively high accuracy on the dataset.
- After experimenting with oversampling techniques, the accuracy scores did not show significant improvements.
