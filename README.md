# Customer Churn Prediction

## 📌 Project Overview

Customer churn is a critical issue for businesses, as retaining existing customers is often more cost-effective than acquiring new ones. This project aims to analyze customer data, identify key factors leading to churn, and build a predictive model to classify customers who are likely to leave.

## 🎯 Objectives

- Understand customer churn patterns using exploratory data analysis (EDA).
- Preprocess the dataset by handling categorical variables and feature engineering.
- Build a machine learning model to predict customer churn.
- Evaluate model performance and extract actionable insights.

## 📂 Dataset

The dataset consists of customer-related information, including:

- **Demographic Data**: Geography, Gender, Age, Tenure
- **Financial Data**: Credit Score, Balance, Estimated Salary
- **Customer Behavior**: Number of Products, Has Credit Card, Is Active Member
- **Target Variable**: `Exited` (1 = Customer left, 0 = Customer stayed)

## 🏗️ Methodology

### 1️⃣ **Data Preprocessing**

- Removed unnecessary columns (`RowNumber`, `CustomerId`, `Surname`).
- Encoded categorical variables (`Geography`, `Gender`) using One-Hot Encoding and Label Encoding.
- Split data into **train (80%)** and **test (20%)** sets.

### 2️⃣ **Exploratory Data Analysis (EDA)**

- Visualized churn distribution and feature relationships using `matplotlib` and `seaborn`.
- Key insights:
  - Older customers tend to churn more.
  - Customers with lower credit scores and fewer active products have higher churn rates.
  - Geography plays a role in churn, with some regions having higher churn rates.

### 3️⃣ **Model Building**

- Used `scikit-learn` to train multiple models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost
- Evaluated models using **accuracy, precision, recall, and F1-score**.

### 4️⃣ **Model Evaluation & Findings**

- **Random Forest and XGBoost performed best**, achieving high precision and recall.
- Feature importance analysis showed:
  - `Age`, `Balance`, and `NumOfProducts` were key drivers of churn.
  - Active members and customers with credit cards had lower churn rates.

## 📊 Key Findings & Business Impact

- **Targeted Retention Strategies**: Focus on retaining older customers with high balances.
- **Improve Customer Engagement**: Encourage multi-product usage to reduce churn.
- **Personalized Offers**: Offer better incentives to customers at high risk of churning.

## 🚀 Next Steps

- Hyperparameter tuning to improve model performance.
- Deploying the model using Flask or a cloud-based solution.
- Expanding dataset with additional customer interaction data.

## 🛠️ Technologies Used

- **Python (pandas, numpy, matplotlib, seaborn, scikit-learn, XGBoost)**
- **Jupyter Notebook** for analysis
- **Tableau/Excel** for visualization

## 📌 Conclusion

This project demonstrates how data analytics and machine learning can help businesses **predict and prevent customer churn**. By implementing data-driven strategies, companies can significantly reduce churn and improve customer retention.

