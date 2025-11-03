# maternal-health-risk-prediction
Machine Learning project predicting maternal risk during pregnancy


## Project Overview
This project uses machine learning to predict maternal health risk (low, medium, or high) during pregnancy based on vital health indicators. The goal is to help identify women who may be at risk so that doctors and healthcare providers can take preventive actions early.
The dataset was obtained from Kaggle and contains 1,014 entries, including features such as age, systolic and diastolic blood pressure, blood sugar, body temperature, and heart rate. Risk levels are categorized as low, medium, or high.

## About the Dataset
The dataset was obtained from Kaggle and contains 1,014 entries collected from hospitals and clinics to monitor maternal health risk. It includes features such as age, systolic and diastolic blood pressure, blood sugar, heart rate, and the target variable, RiskLevel, which is categorized as low, medium, or high risk. Outliers were removed before analysis.

## Methodology / Project Steps
We loaded the dataset in Python and examined its structure using pandas. The data was cleaned by handling missing values, removing duplicates, and checking datatypes. We conducted exploratory data analysis using histograms, boxplots, and correlation heatmaps to study feature distributions and their relationships with RiskLevel. Outliers were identified and 37 rows were removed using the Z-score method to prevent extreme values from affecting the model. The RiskLevel target variable was encoded into numeric labels, and numeric features were standardized for consistent scaling. The dataset was split into training (70%) and testing (30%) sets. We trained a Random Forest Classifier to predict maternal risk levels and evaluated its performance using accuracy, precision, recall, and F1-score. Finally, we analyzed feature importance and suggested threshold values for high-risk indicators.

## Main Results
The Random Forest model achieved 85% accuracy, demonstrating reliable predictions across low, medium, and high-risk classes. Precision, recall, and F1-scores were balanced across all categories. The most influential features were blood sugar, systolic and diastolic blood pressure, and age. Possible thresholds for higher risk include age above 35 years, systolic BP above 120 mmHg, diastolic BP above 90 mmHg, blood sugar above 11 mmol/L, body temperature above 98°C, and heart rate above 78 bpm. Monitoring these key indicators can help identify high-risk patients early and guide preventive healthcare actions.

## Prescriptive Insights
Patients exceeding these thresholds should be monitored more closely. Regular check-ups and early interventions can help prevent complications. Healthcare providers can use such predictive models to improve maternal care programs. Model performance can be further improved with larger and more diverse datasets.

## Authors
•	Emiliano Gallardo
•	Rodrigo Rivas
•	Laura Victoria Miquel Herrera
•	Luis Felipe Navarro Torres
•	Janna Freund
•	Jacobo Ceballos Moná

## Technologies & Tools
•	Python (Pandas, NumPy, Matplotlib, Seaborn)
•	Jupyter Notebook 
•	Visual Studio Code 
•	GitHub repository


