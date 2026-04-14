# Employee-Retention-Analysis-Salifort-Motors
Salifort Motors, a mid-sized automotive company, faced high employee turnover that was affecting productivity, recruitment costs, and overall morale. The business wanted to understand why employees were leaving and identify measurable factors contributing to attrition. This challenge matters because retaining skilled.

##  Project Overview
This portfolio project investigates employee attrition at Salifort Motors, a fictional automotive company. The goal is to identify the key drivers of employee turnover and provide actionable insights to improve retention.  
Employee Retention

In the Salifort Motors project, employee retention was examined as a critical business challenge where data science was used to uncover why staff members were departing. The analysis revealed a clear correlation between retention and the physical and mental demands placed on employees; specifically, those tasked with six or more projects or working over 250 hours per month reached a "breaking point" that led to high turnover. Retention was also heavily influenced by employee satisfaction and company culture, as many who left felt stagnant due to a lack of promotions or felt undervalued despite high performance scores. By identifying these patterns through predictive modelling, the project demonstrated that retention isn't just about salary, but about managing workloads, providing clear career progression, and maintaining a healthy work-life balance to keep top talent from seeking opportunities elsewhere.
<img src="https://github.com/user-attachments/assets/ca65b350-d577-4317-8e41-1c04951c7104">

---

##  Business Problem
Employee turnover is one of the most expensive challenges for organizations. Salifort Motors faces rising attrition rates, which impact productivity, morale, and costs.  
This project answers:
- What factors most strongly influence employee attrition?
- Can we predict which employees are at risk of leaving?
- What strategies can HR implement to improve retention?

---

##  Dataset
The datasets is called the **HR_capstone_dataset.csv** from [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv). where 
- **Features**:employee satisfaction, performance evaluations, project counts, monthly hours, tenure, work accidents, promotion history, department, and salary levels, all used to predict the target variable of employee attrition. 
- **Target Variable**: Attrition (Yes/No).  
- **Size**: ~1,500 employee records, 10 columns.

| Column Name | Description |
| :--- | :--- |
| satisfaction_level | The employee’s self-reported satisfaction level [0-1] |
| last_evaluation | Score of employee's last performance review [0–1] |
| number_project | Number of projects employee contributes to |
| average_monthly_hours | Average number of hours employee worked per month |
| time_spend_company | How long the employee has been with the company (years) |
| work_accident | Whether or not the employee experienced an accident while at work |
| left | Whether or not the employee left the company |
| promotion_last_5years | Whether or not the employee was promoted in the last 5 years |
| department |The employee's department |
| salary |The employee's salary (low, medium, or high) |
---

##  Methodologies Used

1. Exploratory Data Analysis (EDA)- Visualized attrition trends by age, department, salary, overtime. Identified patterns and correlations using heatmaps, bar charts, and boxplots.  
2. Descriptive Statistics - Summarized key variables (mean, median, variance).Compared distributions between attrition vs. non-attrition groups.  
3. Logistic Regression Model - Established a baseline predictive model.Interpreted coefficients to understand feature importance.  
4. Decision Tree - Built interpretable tree-based model to capture non-linear relationships.Visualized decision paths for HR managers.  
5. Random Forest - Improved predictive performance using ensemble learning. Ranked feature importance to highlight key drivers of attrition.  
6. XGBoost - Applied gradient boosting for high accuracy.Tuned hyperparameters to optimize ROC-AUC and Recall.  

##  Data Cleansing
Before working on a dataset, it is important to ensure the data is clean. It is also necessary to understand the dataset through EDA before diving deeper into the data.
Firstly, I loaded the dataset and gathered some basic information about the dataset.

1.Some column names were misspelt or not in snake case, hence renamed them.

2.Check for any missing or duplicated values in the dataset.

3.There were 3008 duplicated rows, since the dataset has 10 variable removing the duplicates will work best.

4.The last step is to determine outliers in the dataset.

## Exploratory Data Analysis
Understand the ratio of employees who stayed in the company to those who left.
For data cleaning, descriptive statistics .describe(), .value_counts(), and handling missing values.
For numerical operations and summary statistics.
For visualizations like histograms, bar charts, boxplots, heatmaps, and correlation matrices.
For encoding categorical variables, scaling features, and preparing data for modeling.


---

##  Results
- **Top attrition drivers**: Overtime, job satisfaction, compensation, tenure.  
- **Best model**: Random Forest with ROC-AUC of 0.87 and Recall of 0.82.  
- **Business insight**: Employees with low satisfaction and high overtime are most at risk.  
- **Recommendation**: Improve work-life balance policies and review compensation structures.

---

##  Tools & Technologies
- **Python**: Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **EDA & Modeling**: Jupyter Notebook  
- **Dashboard**: Streamlit / PowerBI  
- **Version Control**: Git & GitHub  

---



---

