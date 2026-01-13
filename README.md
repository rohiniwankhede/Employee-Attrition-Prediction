Employee Attrition Prediction using Machine Learning 

1. Introduction 

Employee attrition is a critical challenge for organizations as it leads to increased recruitment costs, loss of experienced talent, and reduced productivity. This project focuses on building a Machine Learning model that can predict whether an employee is likely to leave the organization. By using historical HR data, the model helps HR teams take proactive decisions to improve employee retention. 

2. Project Objectives 

- To analyze employee data and understand key factors influencing attrition. 
- To perform Exploratory Data Analysis (EDA) for identifying patterns and trends. 
- To preprocess data for machine learning model readiness. 
- To build and evaluate multiple ML models for attrition prediction. 
- To provide actionable insights for HR decision-making. 

3. Exploratory Data Analysis (EDA) 

EDA was performed to understand the structure and characteristics of the dataset. Initial analysis included checking dataset shape, data types, missing values, and duplicate records. 

Key insights from EDA revealed that features such as Gender, Marital Status, OverTime, Monthly Income, Tenure, and Average Weekly Hours showed minimal difference between employees who stayed and those who left. 

However, Employee Engagement Score showed a strong inverse relationship with attrition. Employees with low engagement scores (1–3) were more likely to leave, whereas those with high scores (4–5) tended to stay. Boxplot visualization clearly demonstrated this separation. 

4. Data Preprocessing 

Data preprocessing was carried out to prepare the dataset for machine learning models. The target variable Attrition was encoded as Yes = 1 and No = 0. 

Categorical variables with binary values were encoded using Label Encoding, while multi-category variables such as department, job role, designation, marital status, and education level were converted using One-Hot Encoding. 

Missing values detected after scaling were handled using median imputation. The DateOfJoining column was dropped as it was not useful for prediction. 

5. Feature Scaling 

Feature scaling was applied using StandardScaler to normalize numerical features. This step ensures that all features contribute equally to model training and improves model performance. 

6. Model Building 

Three machine learning models were trained and evaluated: 
- Logistic Regression 
- Decision Tree Classifier 
- Random Forest Classifier 
 
Logistic Regression was trained with increased iterations to ensure convergence. Decision Tree and Random Forest models were constrained using max depth to avoid overfitting. 

7. Model Evaluation 

Model performance was evaluated using Accuracy, Confusion Matrix, and Classification Report. All models achieved high performance with testing accuracy around 99.7%. 

The confusion matrix showed zero false negatives, indicating that employees likely to leave were correctly identified. Precision, recall, and F1-scores were also very high, confirming model reliability. 

8. Conclusion 

In conclusion, this project successfully developed an Employee Attrition Prediction system using machine learning. EDA revealed that employee engagement score is the most significant factor influencing attrition. 

Among all models, Logistic Regression was selected as the final model due to its simplicity, stability, and interpretability, making it suitable for business use. 

This project demonstrates how machine learning can support HR teams by enabling proactive retention strategies, reducing attrition costs, and improving overall organizational performance. 
