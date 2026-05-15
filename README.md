# credit-risk-scorecard-model
End-to-end Credit Risk Scorecard Modeling using WOE, IV, Logistic Regression, KS, AUC, and Scorecard Scaling in Python.


# Credit Risk Scorecard Model

## 📌 Project Overview

This project demonstrates an end-to-end Credit Risk Scorecard Modeling pipeline used in the banking and financial industry to predict customer default risk.

The project includes:
- Data preprocessing
- WOE (Weight of Evidence) transformation
- IV (Information Value) analysis
- Logistic Regression modeling
- KS & AUC evaluation
- Credit score generation

The objective is to classify customers as:
- Good Customers
- Bad Customers (likely to default)

---

## 📊 Dataset

Dataset Used:
- German Credit Risk Dataset

The dataset contains customer demographic and financial information such as:
- Age
- Credit amount
- Duration
- Employment status
- Housing
- Savings accounts
- Checking accounts

Target Variable:
- `1` = Bad Customer
- `0` = Good Customer

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- ScorecardPy
- Matplotlib
- Seaborn

---

## 📂 Project Structure

```text
credit-risk-scorecard-model/
│
├── data/
├── notebooks/
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_woe_binning.ipynb
│   ├── 03_model_building.ipynb
│   └── 04_scorecard_creation.ipynb
│
├── src/
├── README.md
└── requirements.txt
```

---

## 🔄 Project Workflow

### 1. Data Preprocessing
- Data cleaning
- Missing value treatment
- Target variable creation
- Train-test split

### 2. WOE & IV Analysis
- Variable binning
- Weight of Evidence transformation
- Information Value calculation
- Feature selection

### 3. Model Building
- Logistic Regression model training
- Probability prediction

### 4. Model Evaluation
Evaluation metrics used:
- AUC (Area Under Curve)
- KS Statistic
- ROC Curve

### 5. Scorecard Generation
- Score scaling
- Customer credit score generation

---

## 📈 Model Evaluation Metrics

### AUC
Measures the model’s ability to distinguish between good and bad customers.

### KS Statistic
Measures separation between cumulative good and bad distributions.

---

## 📉 Example Scorecard Workflow

1. Raw customer data  
2. WOE transformation  
3. Logistic regression prediction  
4. Probability of default estimation  
5. Credit score generation

---

## 🚀 Key Learning Outcomes

- Understanding of banking scorecard models
- WOE and IV implementation
- Credit risk modeling concepts
- Logistic regression in risk analytics
- Model validation using KS and AUC

---

## 📌 Future Improvements

- Population Stability Index (PSI)
- Model Monitoring Dashboard
- Streamlit deployment
- Hyperparameter tuning
- Reject inference

---

## ▶️ How to Run

### Install dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn scorecardpy
```

### Run notebooks sequentially

1. `01_data_preprocessing.ipynb`
2. `02_woe_binning.ipynb`
3. `03_model_building.ipynb`
4. `04_scorecard_creation.ipynb`

---

## 📷 Sample Outputs

- ROC Curve
- KS Plot
- WOE Binning Tables
- Credit Score Distribution

---

## 💼 Business Use Case

Banks and financial institutions use scorecard models to:
- Approve/reject loans
- Estimate default probability
- Monitor portfolio risk
- Improve lending decisions

---

## 👨‍💻 Author

Suvendu Samanta

Manager | Credit Risk Analytics | Python | PySpark | GenAI Enthusiast
