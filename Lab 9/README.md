### Decision Trees & Random Forest Lab

#### Overview
This project demonstrates the use of Decision Tree and Random Forest classifiers to predict whether a loan will be fully paid or not.

#### Dataset
- File: `loan_data.csv`
- Target Variable: `not.fully.paid`
- Features include financial and categorical data such as credit policy, interest rate, purpose, etc.

#### Workflow

##### 1. Data Exploration
- Load dataset using pandas
- Inspect structure with `.info()` and `.describe()`

##### 2. Data Visualization
- Countplot of the target variable to understand class distribution

##### 3. Data Preprocessing
- Convert categorical variable `purpose` into dummy variables using one-hot encoding

##### 4. Train-Test Split
- Split data into training and testing sets (70/30)

##### 5. Decision Tree Model
- Train a DecisionTreeClassifier
- Evaluate using confusion matrix and classification report

##### 6. Random Forest Model
- Train a RandomForestClassifier with 200 estimators
- Evaluate performance and compare with Decision Tree

#### Results
- Random Forest generally performs better than a single Decision Tree due to ensemble learning
- Metrics used:
  - Precision
  - Recall
  - F1-score

#### How to Run
1. Place `loan_data.csv` in the same directory as the notebook
2. Open the notebook (`Decision_Trees_RF_Filled.ipynb`)
3. Run all cells sequentially

#### Notes
- Decision Trees are prone to overfitting
- Random Forest reduces overfitting by averaging multiple trees

