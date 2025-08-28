## Employee Attrition Classification

### Project Overview

This project aims to predict **employee attrition** (whether an employee will leave or stay) based on a comprehensive dataset of employee attributes. By analyzing factors such as age, job role, monthly income, job satisfaction, and work-life balance, the goal is to develop a machine learning model that can accurately forecast attrition. This is a critical task for human resources management and organizational planning.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Employee Attrition Dataset](https://www.kaggle.com/datasets/stealthtechnologies/employee-attrition-dataset)
  * **Size**: 74,498 entries, 24 columns. The dataset is a combination of training and testing data provided.
  * **Key Features**:
      * `Age`, `Gender`, `Years at Company`, `Job Role`, `Monthly Income`, `Job Satisfaction`, `Performance Rating`, `Overtime`, `Distance from Home`, `Education Level`, `Marital Status`, `Company Size`, `Company Tenure`.
  * **Approach**:
      * **Data Cleaning**: The dataset was clean with no missing values or duplicates.
      * **Exploratory Data Analysis**: The code checks basic statistics, null values, duplicates, and unique values for all columns. The target variable `Attrition` is relatively balanced between 'Stayed' and 'Left'.
      * **Label Encoding**: Applied to all categorical features and the target `Attrition`.
      * **Binary Classification**: The target variable `Attrition` is classified into two categories: 'Stayed' and 'Left'.
      * **Models Used**:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * **75.9%** with Gradient Boosting Classifier.
      * **75.7%** with AdaBoost Classifier.
      * **75.6%** with XGBoost Classifier.
      * The moderate accuracies suggest that predicting attrition is a complex problem, but the models show good predictive power on this dataset.

-----

### Purpose and Applications

  * **Forecast employee attrition rates** for better human resources planning.
  * Identify key factors that contribute to employee turnover, allowing organizations to take proactive measures.
  * Support the development of retention strategies by understanding which employee attributes and work conditions are most correlated with staying.
  * Provide a tool for managers and HR professionals to assess flight risk and improve employee engagement.

-----

### Installation

Clone the repository and extract the data from the zip file.

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Performing comprehensive hyperparameter tuning and cross-validation for the top-performing models to ensure robustness.
  * Exploring more advanced feature engineering, such as creating interaction terms between different employee attributes.
  * Investigating alternative encoding methods for categorical features (e.g., One-Hot Encoding) to see if they improve performance.
  * Adding explainability (e.g., SHAP or LIME) to understand which features are the most critical predictors of attrition.
