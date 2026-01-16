# CreditWise – Loan Approval Prediction System

CreditWise is a machine learning project that analyzes applicant financial and demographic data to predict whether a loan will be approved or not.  
The project follows a complete ML pipeline , from data cleaning and EDA to feature engineering, model training, and evaluation.

---

## 🚀 Project Overview

Banks and financial institutions rely heavily on credit risk assessment.  
This project builds a **classification-based decision support system** to help predict loan approval outcomes using historical applicant data.

---

## 📂 Dataset Overview

- Total Records: **1000**
- Target Variable: **Loan_Approved**
- Features include:
  - Applicant & Co-applicant Income
  - Credit Score
  - DTI Ratio
  - Employment Status
  - Education Level
  - Property Area
  - Loan Amount & Term
  - Savings & Collateral Value

Missing values were handled using:
- **Mean imputation** for numerical features
- **Most frequent value** for categorical features

---

## 🧠 Machine Learning Workflow

### 1️⃣ Data Preprocessing
- Removed irrelevant features (Applicant_ID)
- Handled missing values
- Encoded categorical variables:
  - Label Encoding
  - One-Hot Encoding
- Feature Scaling using **StandardScaler**

---

### 2️⃣ Exploratory Data Analysis (EDA)
- Class imbalance analysis
- Income distribution analysis
- Category-wise approval trends
- Box plots for outlier detection
- Correlation heatmap

**Key Insight:**
- Credit Score is the most influential factor
- DTI Ratio negatively impacts approval chances

---

### 3️⃣ Feature Engineering
- Polynomial features added:
  - `Credit_Score²`
  - `DTI_Ratio²`
- Improved model performance after transformation

---

### 4️⃣ Models Implemented

| Model              | Accuracy | Precision |
|-------------------|----------|-----------|
| Logistic Regression | 88%      | 0.78      |
| KNN               | 77%      | 0.67      |
| Naive Bayes       | 86%      | **0.81**  |

📌 **Best Model (Precision-based): Naive Bayes**

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📁 Project Structure
credit_wise_project/
│
├── credit_wise_project.ipynb
├── loan_approval_data.csv
├── README.md
└── requirements.txt



---

## 📈 Results & Conclusion

- Credit Score and DTI Ratio dominate loan approval decisions
- Feature engineering improves recall and F1-score
- Naive Bayes performs best when **precision is the priority**

---

## 🔮 Future Enhancements

- Deploy using MERN stack (React + Node + Express)
- Add REST API for real-time predictions
- Integrate explainability (SHAP / LIME)
- Convert to end-to-end production pipeline

---

## 👨‍💻 Author

**Prajwal**  
B.Tech – AI & ML  
Machine Learning & Full Stack Enthusiast

