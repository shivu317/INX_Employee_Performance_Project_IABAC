# INX Employee Performance Analysis

**Project Code:** 10281  
**Organization:** INX Future Inc.  
**Domain:** Human Resource Analytics / Data Science  

---

## Project Overview

INX Future Inc. observed a decline in employee performance indexes, resulting in reduced service delivery quality and an 8% drop in client satisfaction.  
The goal of this project is to analyze employee data, identify performance drivers, assess department-wise performance, build a predictive model, and recommend actionable strategies to improve productivity without impacting employee morale.

This project follows the complete Data Science lifecycle: Data Understanding → Preprocessing → Exploratory Data Analysis → Feature Engineering → Model Building → Evaluation → Recommendations.

---

## Business Objectives

1. Analyze **department-wise employee performance**.  
2. Identify the **top 3 factors affecting employee performance**.  
3. Build a **machine learning model** to predict employee performance.  
4. Provide **data-driven recommendations** to improve employee performance.

---

## Dataset

- **Target Variable:** `PerformanceRating` (Ordinal: 2 = Low, 3 = Good, 4 = Excellent)  
- **Key Features Include:**  
  - Department, JobRole, Age, Gender, Education, MonthlyIncome, JobLevel  
  - JobSatisfaction, EnvironmentSatisfaction, WorkLifeBalance  
  - YearsAtCompany, YearsInCurrentRole, TrainingTimesLastYear, Attrition  

> **Note:** Raw and processed datasets are located in the `data/raw` and `data/processed` folders respectively.

---

## Folder Structure

```INX_Employee_Performance_Project
│
├── Project Summary
│ ├── Requirement
│ ├── Analysis
│ └── Summary
│
├── data
│ ├── raw
│ ├── processed
│ └── external
│
├── src
│ ├── Data Processing
│ │ ├── data_processing.ipynb
│ │ └── data_exploratory_analysis.ipynb
│ ├── models
│ │ ├── model.training.ipynb
│ │ └── train_model.ipynb
│ └── visualization
│ └── visualize.ipynb
│
├── references
└── README.md```

---

## Key Steps

1. **Data Processing**  
   - Load raw data  
   - Handle missing values  
   - Encode categorical variables  
   - Save processed data  

2. **Exploratory Data Analysis**  
   - Department-wise performance analysis  
   - Identify patterns and trends  
   - Visualize correlations between features  

3. **Feature Engineering & Selection**  
   - Identify top performance drivers  
   - Analyze correlation of key features  

4. **Model Training**  
   - Random Forest Classifier used as final model  
   - Train-test split  
   - Evaluate model with Accuracy and Classification Report  
   - Save trained model (`employee_performance_model.pkl`)  

5. **Prediction**  
   - Load trained model  
   - Predict employee performance for sample inputs  

6. **Visualization**  
   - Feature importance plots  
   - Department-wise performance visualizations  

---

## Key Insights

- **Department-wise Performance:** R&D and Sales require targeted interventions.  
- **Top 3 Performance Drivers:** Job Satisfaction, Monthly Income, Work-Life Balance.  
- **Experience:** Employees with 3–8 years at company perform best.  
- **Training Impact:** Regular training improves mid-level performance.  

---

## Recommendations

1. Introduce department-specific engagement programs.  
2. Improve job satisfaction via recognition and career growth plans.  
3. Optimize compensation for high-performing roles.  
4. Use the predictive model during hiring to assess performance potential.  

---

## Tools & Technologies

- Python 3.x  
- Pandas, NumPy  
- Scikit-learn (RandomForestClassifier, LabelEncoder)  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/INX_Employee_Performance_Project.git
