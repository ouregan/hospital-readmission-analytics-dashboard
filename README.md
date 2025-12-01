Predicting 30-Day Hospital Readmissions Using Machine Learning + Power BI
 Project Overview

This project builds a machine learning classification model to predict which patients are at risk of being readmitted within 30 days.
The final output is a Power BI dashboard showing:

1. Key hospital readmission metrics

2. Patient-level risk scores

3. Feature importance analysis (SHAP)

4. Demographic and clinical trends

The goal is to help healthcare providers identify high-risk patients early and improve operational planning.

🛠 Tech Stack
Python (Modeling)
Pandas
NumPy
Scikit-learn
XGBoost
Imbalanced-learn (SMOTE)
SHAP

Power BI (Visualization)

Patient risk explorer

Readmission trend analysis

Feature importance dashboard

📂 Project Structure
hospital-readmission-analytics-dashboard/
│
├── data/
│   ├── raw/                # Original raw dataset
│   └── processed/          # Cleaned dataset for modeling
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_feature_engineering.ipynb
├──  └── 03_model_training.ipynb
│
├── src/
│   ├── data_preprocessing.py
│   ├── train_model.py
│   └── generate_predictions.py
│
├── models/
│   └── xgboost_model.pkl
│
├── powerbi/
│   ├── hospital_readmission_dashboard.pbix
│   └── dashboard_data.csv
│
├── README.md
├── requirements.txt
└── .gitignore

Objectives

Build a binary classification model to predict readmissions.

Handle imbalanced data using SMOTE and/or class weighting.

Achieve 80%+ ROC-AUC.

Generate risk scores and SHAP explanations.

Create a professional Power BI dashboard for hospital decision-makers.

Power BI Dashboard Pages



----Executive Overview----

Total patients

30-day readmission rate

Monthly readmission trend

Readmission rate by age group

Disease category distribution

----Model Insights----

SHAP feature importance

Risk score distribution

Readmission rate by risk level

Risk score vs length of stay

Patient Risk Explorer

Interactive table with:

Patient ID

Demographics

Diagnosis

Risk score

Predicted label

Previous admissions

Filters:

Age

Gender

Diagnosis

Risk level
(To Fill After Training)
Metric	Score
ROC-AUC	—
Accuracy	—
Precision	—
Recall	—
F1-Score	—


----How to Reproduce----
1. Clone the Repository
git clone https://github.com/<your-username>/hospital-readmission-analytics-dashboard.git

2. Install Dependencies
pip install -r requirements.txt

3. Run Data Preprocessing
python src/data_preprocessing.py

4. Train Model
python src/train_model.py

5. Generate Predictions for Power BI
python src/generate_predictions.py


This will create dashboard_data.csv inside powerbi/.

6. Open Power BI Dashboard

Load:

powerbi/dashboard_data.csv


Open the PBIX file:

powerbi/hospital_readmission_dashboard.pbix

Deliverables

✔ Cleaned dataset

✔ ML model + metrics

✔ Risk score output

✔ SHAP feature explanations

✔ Power BI dashboard

✔ GitHub repository with code + documentation

 Contributing

Contributions and improvements are welcome.
Create a pull request or open an issue.

📜 License

This project is open-source under the MIT License.
