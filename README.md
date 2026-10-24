# Customer-Churn-Prediction-modal


A Machine Learning project that predicts customer churn using Python and Scikit-learn. The project focuses on data preprocessing, feature engineering, Logistic Regression, and model evaluation using the IBM Telco Customer Churn dataset.

## 🎯 Objective

Customer churn occurs when customers discontinue a service. The goal of this project is to build a classification model that identifies customers who are likely to leave a telecom service, helping businesses make data-driven customer retention decisions.

## 📊 Dataset

- **Dataset:** IBM Telco Customer Churn
- **Records:** 7,043 customers
- **Target variable:** `Churn`
- **Problem type:** Binary classification

The dataset contains customer demographics, tenure, service subscriptions, contract details, payment methods, and billing information.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## ⚙️ Machine Learning Workflow

1. **Data Loading and Exploration** — inspected the dataset, data types, distributions, and churn patterns.
2. **Data Cleaning** — handled invalid values in `TotalCharges` and prepared the data for modeling.
3. **Feature Preparation** — separated input features from the target variable and removed the customer ID.
4. **Preprocessing Pipeline** — used `StandardScaler` for numerical features and `OneHotEncoder` for categorical features.
5. **Model Training** — trained a Logistic Regression classifier using Scikit-learn.
6. **Model Evaluation** — assessed performance using classification metrics and a confusion matrix.
7. **Threshold Analysis** — explored probability thresholds to balance churn detection and prediction precision.

## 🤖 Model

**Logistic Regression** was used as the classification algorithm to estimate the probability that a customer will churn.

A Scikit-learn pipeline combines preprocessing and model training to help keep transformations consistent between training and prediction.

## 📈 Evaluation Metrics

The model is evaluated using:

- **Accuracy:** Overall proportion of correct predictions.
- **Precision:** Proportion of predicted churn cases that are actual churn cases.
- **Recall:** Proportion of actual churn cases correctly identified.
- **F1-score:** Harmonic mean of precision and recall.
- **Confusion Matrix:** Breakdown of correct and incorrect classifications.
- **ROC-AUC:** Ability to distinguish between churn and non-churn customers across classification thresholds.

The project considers recall and F1-score important because missing customers who are likely to churn can be costly for a business.

## 📁 Project Structure

```text
Customer-Churn-Prediction/
│
├── Customer_Churn_Prediction
