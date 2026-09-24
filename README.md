# 🏦 Loan Approval Prediction using Machine Learning

A Machine Learning project that predicts whether a loan application will be **approved or rejected** based on applicant information such as education, income, marital status, credit history, property area, and other relevant features.

---

## 📌 Project Overview

Loans are an important part of the modern financial system. Banks and financial institutions need to evaluate several factors before approving a loan application.

This project uses Machine Learning classification algorithms to analyze applicant information and predict the loan approval status.

The target variable is:

* **Y → Loan Approved**
* **N → Loan Not Approved**

---

## 🎯 Objectives

* Analyze loan application data
* Perform Exploratory Data Analysis (EDA)
* Identify important features affecting loan approval
* Handle categorical variables
* Handle missing values
* Visualize relationships between features
* Train multiple Machine Learning classification models
* Compare model performance
* Predict loan approval status

---

## 🗂️ Dataset

The dataset contains **13 features** related to loan applicants.

### Dataset Features

| Feature             | Description                              |
| ------------------- | ---------------------------------------- |
| `Loan_ID`           | Unique identification number of the loan |
| `Gender`            | Gender of the applicant                  |
| `Married`           | Marital status of the applicant          |
| `Dependents`        | Number of dependents                     |
| `Education`         | Education status of the applicant        |
| `Self_Employed`     | Whether the applicant is self-employed   |
| `ApplicantIncome`   | Income of the applicant                  |
| `CoapplicantIncome` | Income of the co-applicant               |
| `LoanAmount`        | Requested loan amount                    |
| `Loan_Amount_Term`  | Loan repayment term in months            |
| `Credit_History`    | Applicant's credit history               |
| `Property_Area`     | Rural, Urban, or Semi-urban              |
| `Loan_Status`       | Loan approval status                     |

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**

---

## 🔄 Machine Learning Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Exploration
   ↓
Data Preprocessing
   ↓
Categorical Encoding
   ↓
Missing Value Handling
   ↓
Data Visualization
   ↓
Feature & Target Separation
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Loan Approval Prediction
```

---

## 🔍 Exploratory Data Analysis

The project performs Exploratory Data Analysis to understand the characteristics of loan applicants.

The analysis includes:

* Dataset information
* Statistical summary
* Categorical variable analysis
* Applicant income analysis
* Loan amount analysis
* Credit history analysis
* Property area analysis
* Correlation analysis
* Loan status analysis

---

## 🧹 Data Preprocessing

The following preprocessing techniques are applied:

### Removing Irrelevant Features

`Loan_ID` is removed because it is a unique identifier and does not provide useful predictive information.

### Categorical Encoding

Categorical features are converted into numerical values using **Label Encoding**.

This allows Machine Learning algorithms to process categorical applicant information.

### Missing Value Handling

Missing values in the dataset are handled before model training.

---

## 📊 Feature Analysis

A correlation heatmap is used to understand relationships between different features.

The analysis indicates relationships between variables such as:

* Loan Amount
* Applicant Income
* Credit History
* Loan Status

Credit History is identified in the project analysis as having an important relationship with Loan Status.

---

## ✂️ Train-Test Split

The dataset is divided into training and testing datasets.

| Dataset       | Samples |
| ------------- | ------: |
| Training Data |     358 |
| Testing Data  |     240 |

The split uses:

* **60% Training Data**
* **40% Testing Data**

A fixed random state is used to make the results reproducible.

---

## 🤖 Machine Learning Models

Four classification algorithms are trained and evaluated:

### 1. Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees to make predictions.

### 2. K-Nearest Neighbors

Classifies an applicant based on the characteristics of nearby data points.

### 3. Support Vector Classifier

Finds a decision boundary that separates different classes.

### 4. Logistic Regression

A classification algorithm used to estimate the probability of loan approval.

---

## 📈 Model Performance

### Training Accuracy

| Model                     | Training Accuracy |
| ------------------------- | ----------------: |
| Random Forest             |        **98.04%** |
| K-Nearest Neighbors       |        **78.49%** |
| Support Vector Classifier |        **68.72%** |
| Logistic Regression       |        **80.45%** |

### Testing Accuracy

| Model                     | Testing Accuracy |
| ------------------------- | ---------------: |
| Random Forest             |       **82.50%** |
| K-Nearest Neighbors       |       **63.75%** |
| Support Vector Classifier |       **69.17%** |
| Logistic Regression       |       **80.83%** |

The reported results show that the Random Forest Classifier achieved **82.5% accuracy on the testing dataset**.

> Results may vary depending on the dataset, preprocessing steps, library versions, and model configuration.

---

## 🎯 Prediction

The trained models are used to predict whether a loan application should be classified as:

* **Approved**
* **Not Approved**

The prediction is based on applicant information such as:

* Income
* Education
* Credit History
* Marital Status
* Dependents
* Loan Amount
* Loan Term
* Property Area
* Employment Status

---

## ⚠️ Important Considerations

Loan approval is a real-world financial decision. A Machine Learning model should be treated as a decision-support system rather than the sole basis for approving or rejecting an application.

Model performance can also be affected
