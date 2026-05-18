# 🏦 Enterprise Credit Risk Analytics & Scorecard Modeling System

An end-to-end enterprise-style Credit Risk Modeling project built using the Home Credit Default Risk dataset.  
This project demonstrates real-world banking analytics workflows including:

- Credit Risk Modeling
- WOE & IV Analysis
- Logistic Regression Scorecards
- XGBoost Benchmarking
- KS & AUC Evaluation
- Credit Score Generation
- Population Stability Index (PSI)
- Drift Monitoring Framework

---

# 📌 Business Problem

Financial institutions need to assess whether a customer is likely to default on a loan.

This project builds a complete scorecard-based credit risk system that:
- predicts probability of default
- generates customer credit scores
- segments customers into risk bands
- monitors model stability over time

---

# 🧠 Project Objectives

- Build an interpretable banking-style scorecard model
- Compare traditional scorecards vs modern ML models
- Generate business-friendly customer risk scores
- Implement enterprise monitoring metrics like PSI
- Simulate production drift monitoring

---

# 📊 Dataset

Dataset Used:
- Home Credit Default Risk Dataset

Source:
- Kaggle Competition Dataset

The dataset contains:
- demographic information
- income details
- loan information
- employment history
- behavioral credit features

Target Variable:
- `TARGET = 1` → Customer Default
- `TARGET = 0` → Non-default

---

# 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| ML Models | Logistic Regression, XGBoost |
| Scorecard Modeling | ScorecardPy |
| Monitoring | PSI, Drift Analysis |
| Environment | Google Colab |

---

# 📂 Project Structure

```text
credit-risk-analytics-system/
│
├── data/
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning_feature_engineering.ipynb
│   ├── 03_woe_iv_analysis.ipynb
│   ├── 04_model_building_evaluation.ipynb
│   ├── 05_scorecard_generation.ipynb
│   └── 06_psi_monitoring.ipynb
│
├── outputs/
│   ├── customer_credit_scores.csv
│   ├── model_monitoring_report.csv
│
├── README.md
└── requirements.txt
```

---

# 🔄 End-to-End Workflow

## 1️⃣ Data Understanding
- Dataset exploration
- Missing value analysis
- Target imbalance analysis
- Correlation analysis

---

## 2️⃣ Data Cleaning & Feature Engineering

### Missing Value Treatment
- threshold-based removal
- median imputation
- categorical missing handling

### Feature Engineering
Created business-driven features such as:

- Credit Income Ratio
- Annuity Income Ratio
- Employment Stability
- Credit Term

---

## 3️⃣ WOE & IV Analysis

Implemented:
- monotonic binning
- Weight of Evidence (WOE)
- Information Value (IV)
- scorecard-ready transformation

### WOE Formula

\[
WOE = \ln\left(\frac{\%Good}{\%Bad}\right)
\]

### IV Formula

\[
IV = \sum (\%Good - \%Bad) \times WOE
\]

---

# 🤖 Model Development

## Logistic Regression
Traditional interpretable banking scorecard model.

## XGBoost
Modern machine learning benchmark model.

---

# 📈 Model Performance

| Model | AUC |
|---|---|
| Logistic Regression | 0.7412 |
| XGBoost | 0.7390 |

### KS Statistic
- KS = 0.3618

---

# 📊 Key Insights

- Logistic Regression slightly outperformed XGBoost
- WOE transformation improved model interpretability
- Scorecard achieved strong risk separation
- Higher scores corresponded to lower default rates

---

# 💳 Credit Scorecard Generation

Converted probability of default into business-friendly credit scores.

### Risk Segmentation

| Risk Band | Default Rate |
|---|---|
| High Risk | 10.0% |
| Medium Risk | 2.2% |
| Low Risk | 0.0% |

---

# 📉 Score Distribution

The generated score distribution showed:
- stable bell-shaped behavior
- effective customer risk separation
- realistic portfolio distribution

---

# 🛡️ Model Monitoring & PSI

Implemented enterprise monitoring framework including:

- Population Stability Index (PSI)
- Score Drift Monitoring
- Feature Drift Analysis
- Risk Band Stability Tracking

### PSI Formula

\[
PSI = \sum (Actual\% - Expected\%) \times \ln\left(\frac{Actual\%}{Expected\%}\right)
\]

### PSI Interpretation

| PSI | Interpretation |
|---|---|
| <0.1 | Stable Population |
| 0.1–0.25 | Moderate Shift |
| >0.25 | Significant Drift |

---

# 📌 Business Impact

This system can help banks:
- reduce credit losses
- improve loan approval decisions
- monitor portfolio quality
- detect model drift
- prioritize low-risk customers

---

# 🚀 Future Improvements

- Streamlit deployment
- SHAP explainability
- Hyperparameter tuning
- IFRS9 probability of default modeling
- Real-time monitoring dashboard
- Automated retraining pipeline

---

# ▶️ How to Run

## Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost scorecardpy
```

---

## Run Notebooks Sequentially

1. `01_data_understanding.ipynb`
2. `02_data_cleaning_feature_engineering.ipynb`
3. `03_woe_iv_analysis.ipynb`
4. `04_model_building_evaluation.ipynb`
5. `05_scorecard_generation.ipynb`
6. `06_psi_monitoring.ipynb`

---

# 📷 Sample Outputs

- ROC Curve
- KS Statistic
- WOE Binning Plots
- Credit Score Distribution
- Risk Band Analysis
- PSI Monitoring Charts

---

# 👨‍💻 Author

## Suvendu Samanta

Manager | Credit Risk Analytics | Python | PySpark | GenAI Enthusiast

---

# ⭐ Project Highlights

✅ Enterprise-style scorecard modeling  
✅ Banking-grade WOE/IV implementation  
✅ Model monitoring framework  
✅ PSI drift analysis  
✅ Credit score generation  
✅ Business-focused analytics workflow
