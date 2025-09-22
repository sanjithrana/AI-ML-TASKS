# AI-ML-TASKS-1
# Elevate Labs - AI/ML Internship Task 1

## Project: Data Cleaning & Preprocessing

This repository contains the solution for Task 1 of the AI/ML Internship at Elevate Labs.The objective of this task is to clean and preprocess a raw dataset to make it suitable for machine learning models.

### Dataset
The [Titanic Dataset](https://www.kaggle.com/c/titanic/data) was used for this task, as suggested in the problem description.

### Steps Performed
The following data preprocessing steps were performed on the dataset:

1. **Data Exploration**: Loaded the dataset using Pandas and explored its basic information, including data types, and the count of null values for each column.
2.  **Handling Missing Values**:
    * Missing values in the `Age` column were imputed using the **median**.
    * Missing values in the `Embarked` column were filled with the **mode**. 
    * The `Cabin` column was dropped as it contained a large number of missing values.
3.  **Categorical Encoding**: Converted categorical features (`Sex`, `Embarked`) into numerical format using **One-Hot Encoding** to be used in ML models.
4.  **Outlier Removal**: Visualized outliers in the `Fare` and `Age` columns using **boxplots**. Outliers in the `Fare` column were removed using the **Interquartile Range (IQR)** method.
5.  **Feature Scaling**: Standardized the numerical features (`Age`, `Fare`, `SibSp`, `Parch`) using `StandardScaler` from Scikit-learn to bring them to a common scale. 

### Tools and Libraries Used
* **Python** 
* **Pandas**: For data manipulation and analysis.
* **NumPy**: For numerical operations.
* **Matplotlib & Seaborn**: For data visualization.
* **Scikit-learn**: For feature scaling.
