# Heart Disease EDA
Exploratory Data Analysis on patient clinical data to identify patterns and risk factors associated with heart disease.

## Project Overview
This project analyzes a heart disease dataset to explore how clinical measurements — age, cholesterol, blood pressure, chest pain type, and more — relate to the presence of heart disease. The notebook walks through data cleaning and answers 20+ clinical questions using pandas, with visualizations built in matplotlib and seaborn, including correlation analysis and pairwise comparisons.

## Dataset
- **Source:** `EDA03_Heart.csv` (Kaggle — Heart Disease dataset)
- **Records:** ~300 patient records
- **Key columns:** `age`, `sex`, `cp` (chest pain type), `trestbps` (resting blood pressure), `chol` (cholesterol), `fbs` (fasting blood sugar), `restecg`, `thalach` (max heart rate), `exang` (exercise-induced angina), `oldpeak`, `ca` (major vessels), `thal`, `target` (heart disease presence)

## Data Cleaning
- Checked for and confirmed no missing values across columns
- Identified and removed duplicate rows
- Verified data types and dataset shape before and after cleaning

## Key Insights
- The average patient age was 54.4, with males making up about 68% of the dataset
- Average cholesterol (246.5 mg/dl) and resting blood pressure (131.6 mmHg) were both above typical normal ranges
- Patients without exercise-induced angina reached higher average max heart rates (155.6 bpm) than those with it (137.2 bpm)
- Heart disease was most common in patients with 0 major vessels colored by fluoroscopy, decreasing as vessel count rose
- Thalassemia type 2 was most associated with heart disease presence, while type 3 was more common in patients without it
- The most frequent risk-factor combination in heart disease patients was chest pain type 2, normal fasting blood sugar, no exercise-induced angina, and thalassemia type 2
- Fasting blood sugar showed only a weak relationship with heart disease presence
- Age and cholesterol showed a weak positive correlation (0.207)

## Skills Demonstrated
- **Data Cleaning:** Detecting and removing duplicates, validating data types and missing values
- **Exploratory Data Analysis (EDA):** Framing clinical questions and answering them with pandas groupby, crosstabs, and correlation analysis
- **Data Visualization:** Creating stacked bar charts, bar plots, and pairplots with matplotlib and seaborn to compare patient groups
- **Insight Generation:** Translating statistical outputs into clear, medically-relevant conclusions
- **Python Programming:** Working with pandas DataFrames, NumPy, and Jupyter Notebook workflows

## Tech Stack
- Python
- pandas, numpy
- matplotlib, seaborn
- Jupyter Notebook

## Project Structure
```
├── EDA03_heart.ipynb
|
├── EDA03_Heart.csv
|
└── README.md
```

## Future Improvements
- Build a predictive model (e.g., logistic regression, random forest) to classify heart disease presence
- Perform feature importance analysis to rank risk factors
- Add interactive dashboards (e.g., Plotly/Streamlit) for the key metrics

## Acknowledgments
Dataset sourced from Kaggle: Heart Disease dataset.
