# Employee Attrition Prediction Using Machine Learning

## Introduction

Employee attrition is a major challenge for organizations because it increases recruitment costs, affects productivity, and leads to the loss of experienced employees. The objective of this project is to analyze employee data, identify the factors associated with employee attrition, and build a predictive model that helps HR identify employees who may be at risk of leaving. The insights from this analysis can support better workforce planning and employee retention strategies.

---

## Dataset

* **Dataset:** IBM HR Analytics Employee Attrition Dataset [https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset]
* **Source:** Kaggle
* **Target Variable:** Attrition (Yes/No)

---

## Project Workflow

### 1. Data Loading and Exploration

* Loaded the dataset using Pandas.
* Explored the dataset structure, dimensions, and data types.
* Identified the target variable (Attrition).
* Calculated the overall attrition rate.
* Distinguished numeric and categorical features.

### 2. Data Preprocessing

* Checked and handled missing values.
* Removed columns with little or no predictive value.
* Converted the Attrition column from Yes/No to 1/0.
* Applied One-Hot Encoding to categorical variables.
* Standardized numeric features using StandardScaler.

### 3. Exploratory Data Analysis (EDA)

The following analyses were performed to understand employee attrition patterns:

* Attrition rate by department.
* Attrition rate by job role.
* Monthly income comparison between employees who left and stayed.
* Relationship between work-life balance and attrition.
* Relationship between years at the company and attrition.

### 4. Model Building

The dataset was divided into training (80%) and testing (20%) sets. Three machine learning models were trained and evaluated:

* Logistic Regression
* Random Forest Classifier
* Gradient Boosting Classifier

The models were compared using Accuracy, Precision, Recall, F1-Score, ROC-AUC Score, and Confusion Matrix. Gradient Boosting achieved the best overall balance in identifying employees who were likely to leave.

---

# Charts and Insights

## Chart 1: Attrition Rate by Department and Job Role
<img width="1553" height="1031" alt="chart1" src="https://github.com/user-attachments/assets/9503af0d-c1cd-4ae5-9e5e-0f3554aad743" />


This chart compares employee attrition across different departments and job roles. The analysis showed that the Sales department had the highest attrition rate, with Sales Representatives experiencing the highest turnover. These groups should be prioritized for retention efforts.

## Chart 2: Monthly Income of Employees Who Left vs Stayed
<img width="992" height="719" alt="chart2" src="https://github.com/user-attachments/assets/efbfab13-4068-46c1-918d-2e14b862a204" />

The box plot compares monthly income for employees who stayed and those who left. Employees who left generally had lower monthly incomes, indicating that compensation influences attrition. However, salary alone does not fully explain employee turnover.

## Chart 3: Confusion Matrix
<img width="825" height="649" alt="chart3" src="https://github.com/user-attachments/assets/b09a7547-07ee-4e1d-b44d-415726aacb44" />

The confusion matrix shows how effectively the final model classified employees who stayed and those who left. The model successfully identified most employees while maintaining a balanced performance, making it suitable for supporting HR decisions.

## Chart 4: Top 10 Feature Importances
<img width="1296" height="796" alt="chart4" src="https://github.com/user-attachments/assets/ffd1c26b-1f83-447b-a4cb-61bc67d0795e" />

The feature importance chart identifies the factors most associated with employee attrition. Overtime, monthly income, stock option level, years at the company, and age were the strongest contributors, highlighting the importance of workload, compensation, and career progression.

## Chart 5 (Bonus): ROC Curve Comparison
<img width="1014" height="732" alt="chart5" src="https://github.com/user-attachments/assets/378906d7-ea29-45a2-9f90-faf702ef3c32" />

The ROC curve compares the performance of all three prediction models. The selected model demonstrated the strongest ability to distinguish between employees who stayed and those who left, making it the preferred model for this project.

---

# HR Insights and Recommendations

### Key Insights

* Employees working frequent overtime are more likely to leave the company.
* Lower monthly income and fewer financial benefits increase the likelihood of attrition.
* Employees in the Sales department, especially Sales Representatives, experience the highest turnover.
* Employees in their early years with the company are at greater risk of leaving.
* Employee retention depends on multiple factors, including workload, compensation, career growth, and engagement.

### Recommendations

1. Monitor overtime and introduce work-life balance initiatives to reduce employee burnout.
2. Prioritize retention efforts for high-turnover departments and job roles through regular check-ins, career development opportunities, and competitive compensation and benefits.

---

# Conclusion

This project demonstrates how employee data can be used to identify patterns related to attrition and support informed HR decisions. The analysis revealed that overtime, compensation, financial benefits, and career progression are the primary factors associated with employee turnover. Among the evaluated models, Gradient Boosting provided the most balanced and reliable performance for predicting attrition. While the model offers valuable insights, it should be used as a decision-support tool alongside employee feedback and managerial judgment. By acting on these findings, organizations can improve employee satisfaction, strengthen retention strategies, and reduce the overall cost of employee turnover.
