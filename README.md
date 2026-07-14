# 🏦 Loan Approval Prediction using Machine Learning

> An end-to-end Machine Learning project for predicting loan approval decisions using applicant financial information. This project demonstrates a complete ML workflow, including data preprocessing, exploratory data analysis, handling class imbalance with SMOTE, model development, evaluation, and comparative analysis.

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge&logo=scikitlearn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-black?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?style=for-the-badge&logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-green?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-purple?style=for-the-badge)

---

# 📌 Project Overview

Loan approval is one of the most critical decision-making processes in the banking and financial sector. Financial institutions evaluate multiple applicant characteristics such as annual income, CIBIL score, loan amount, assets, and employment status before approving a loan.

The objective of this project is to build Machine Learning models capable of predicting whether a loan application should be **Approved** or **Rejected** while following an industry-standard ML pipeline.

Rather than focusing only on model accuracy, this project emphasizes:

- Data quality assessment
- Business-oriented exploratory data analysis
- Proper preprocessing without data leakage
- Comparison of multiple classification algorithms
- Evaluation using multiple performance metrics
- Investigation of class imbalance using SMOTE

---

# 🎯 Project Objectives

- Predict loan approval status using applicant information
- Perform comprehensive Exploratory Data Analysis (EDA)
- Handle missing values and categorical variables
- Build baseline and advanced classification models
- Compare Logistic Regression and Decision Tree
- Evaluate the impact of SMOTE on model performance
- Select the best-performing model based on multiple evaluation metrics

---

# 📂 Dataset Information

The dataset contains applicant demographic and financial information, including:

- Number of Dependents
- Education Level
- Self Employment Status
- Annual Income
- Loan Amount
- Loan Term
- CIBIL Score
- Residential Asset Value
- Commercial Asset Value
- Luxury Asset Value
- Bank Asset Value
- Loan Status (Target Variable)

**Target Variable**

- Approved
- Rejected

---

# 🛠️ Project Workflow

```
Business Problem
        │
        ▼
Dataset Loading
        │
        ▼
Data Quality Assessment
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Data Preprocessing
        │
        ▼
Train-Test Split
        │
        ▼
Feature Scaling (Logistic Regression)
        │
        ▼
Model Development
        │
        ▼
Model Evaluation
        │
        ▼
SMOTE Experiment
        │
        ▼
Model Comparison
        │
        ▼
Final Model Selection
```

---

# 📊 Exploratory Data Analysis

The project includes a comprehensive EDA covering:

- Target Variable Analysis
- Class Distribution Analysis
- Missing Value Analysis
- Duplicate Detection
- Numerical Feature Distribution
- Categorical Feature Analysis
- Correlation Analysis
- Outlier Detection
- Business Interpretation of Findings

---

# ⚙️ Data Preprocessing

The preprocessing pipeline includes:

- Removal of identifier columns
- Binary encoding of categorical variables
- Feature scaling using StandardScaler
- Proper Train-Test Split
- Prevention of Data Leakage
- Controlled preprocessing pipeline

---

# 🤖 Machine Learning Models

The following classification algorithms were implemented:

### 1️⃣ Logistic Regression

- Baseline Linear Classifier
- Standardized Features
- L2 Regularization
- Gradient-Based Optimization

### 2️⃣ Decision Tree

- Controlled Tree Depth
- Regularized Decision Tree
- Non-linear Classification
- Feature Importance Analysis

---

# ⚖️ Handling Class Imbalance

To investigate the effect of class imbalance:

- SMOTE (Synthetic Minority Over-sampling Technique) was applied
- SMOTE was used **only on the training data**
- Performance before and after SMOTE was compared

This follows industry best practices and prevents data leakage.

---

# 📈 Model Performance

| Model | Accuracy | Precision | Recall | F1 Score |
|-------|----------:|----------:|--------:|---------:|
| Logistic Regression | **91.33%** | **92.08%** | **94.16%** | **93.11%** |
| Logistic Regression + SMOTE | **91.92%** | **94.42%** | **92.47%** | **93.43%** |
| Decision Tree | **97.42%** | **98.66%** | **97.18%** | **97.91%** |
| Decision Tree + SMOTE | **97.19%** | **98.29%** | **97.18%** | **97.73%** |

---

# 🏆 Best Performing Model

🥇 **Decision Tree**

Final Performance:

- Accuracy: **97.42%**
- Precision: **98.66%**
- Recall: **97.18%**
- F1 Score: **97.91%**

The Decision Tree consistently outperformed Logistic Regression across all evaluation metrics while maintaining excellent generalization performance.

---

# 📌 Key Findings

- Decision Tree achieved the highest predictive performance.
- Logistic Regression served as a strong baseline classifier.
- Proper preprocessing significantly improved model reliability.
- SMOTE produced only marginal improvements due to the dataset's mild class imbalance.
- The selected Decision Tree demonstrated excellent generalization with minimal evidence of overfitting.

---

# 📁 Repository Structure

```
loan-approval-prediction-ml/
│
├── data/
│   └── loan_approval_dataset.csv
│
├── figures/
│   ├── correlation_heatmap.png
│   ├── confusion_matrix_logistic_regression.png
│   ├── confusion_matrix_decision_tree.png
│   ├── decision_tree_feature_importance.png
│   ├── model_comparison.png
│   ├── smote_comparison.png
│  
│
├── notebooks/
│   └── Loan_Approval_Prediction.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# 💻 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Imbalanced-learn

---

# 🚀 How to Run

Clone the repository

```bash
git clone https://github.com/yourusername/loan-approval-prediction-ml.git
```

Navigate to the project

```bash
cd loan-approval-prediction-ml
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
Loan_Approval_Prediction.ipynb
```

---

# 🎓 Learning Outcomes

This project strengthened practical understanding of:

- Binary Classification
- Machine Learning Pipeline Design
- Data Cleaning
- Feature Engineering Concepts
- Exploratory Data Analysis
- Logistic Regression
- Decision Tree Classification
- SMOTE for Imbalanced Learning
- Model Evaluation
- Business-Oriented Machine Learning

---

# 📌 Internship Information

**Internship:** Elevvo Machine Learning Internship

**Task:** Task 04 — Loan Approval Prediction

---

# 👨‍💻 Author

**Md Delwar Husen**

Machine Learning | Deep Learning | Computer Vision | NLP

Passionate about building practical AI solutions through data-driven problem solving.

---

## ⭐ If you found this project useful, consider giving it a Star!
