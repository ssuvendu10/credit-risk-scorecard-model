# 🏦 Enterprise Credit Risk Scorecard Modeling System

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-green)
![Banking Analytics](https://img.shields.io/badge/Domain-Credit_Risk-orange)
![Project Status](https://img.shields.io/badge/Project-Completed-brightgreen)

An end-to-end enterprise-style Credit Risk Analytics project built using the Home Credit Default Risk dataset.

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

✅ predicts probability of default  
✅ generates customer credit scores  
✅ segments customers into risk bands  
✅ monitors model stability over time  

---

# 📈 Final Model Performance

| Metric | Value |
|---|---|
| Logistic Regression AUC | 0.7412 |
| KS Statistic | 0.3618 |
| XGBoost AUC | 0.7390 |

---

# 📊 Risk Band Default Rates

| Risk Band | Default Rate |
|---|---|
| High Risk | 10.0% |
| Medium Risk | 2.2% |
| Low Risk | 0.0% |

---

# 🔄 End-to-End Workflow

```text
Data Collection
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
WOE & IV Analysis
        ↓
Logistic Regression
        ↓
Scorecard Generation
        ↓
Risk Segmentation
        ↓
PSI Monitoring
        ↓
Drift Analysis
```

---

# 🏦 Banking Concepts Implemented

- Weight of Evidence (WOE)
- Information Value (IV)
- Scorecard Scaling
- Logistic Regression Scorecards
- KS Statistic
- Population Stability Index (PSI)
- Risk Band Segmentation
- Drift Monitoring
- Credit Risk Analytics

---

# 📊 Dataset

Dataset Used:
- Home Credit Default Risk Dataset

Dataset Source:
- Kaggle Competition Dataset

The dataset contains:
- customer demographic information
- income details
- credit history
- employment history
- loan information
- behavioral credit variables

### Target Variable
- `TARGET = 1` → Customer Default
- `TARGET = 0` → Non-default Customer

---

# 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Logistic Regression, XGBoost |
| Scorecard Modeling | ScorecardPy |
| Monitoring | PSI, Drift Monitoring |
| Environment | Google Colab |

---

# 📂 Project Structure

```text
credit-risk-scorecard-model/
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
│   └── model_monitoring_report.csv
│
├── screenshots/
│
├── README.md
└── requirements.txt
```

---

# 🧠 Feature Engineering

Created business-driven financial features including:

- Credit Income Ratio
- Annuity Income Ratio
- Employment Stability
- Credit Term

These features improved model interpretability and risk segmentation.

---

# 🔍 WOE & IV Analysis

Implemented monotonic binning using Weight of Evidence transformation.

### WOE Formula

\[
WOE = \ln\left(\frac{\%Good}{\%Bad}\right)
\]

### IV Formula

\[
IV = \sum (\%Good - \%Bad) \times WOE
\]

### IV Interpretation

| IV | Predictive Strength |
|---|---|
| <0.02 | Weak |
| 0.02–0.1 | Medium |
| 0.1–0.3 | Strong |
| >0.3 | Very Strong |

---

# 🤖 Model Development

## Logistic Regression
Traditional interpretable banking scorecard model.

## XGBoost
Modern machine learning benchmark model used for comparison.

---

# 📈 Model Evaluation

### ROC-AUC
Measures model discrimination capability.

### KS Statistic
Measures separation between good and bad customer distributions.

### Key Insights
- Logistic Regression slightly outperformed XGBoost
- WOE transformation improved interpretability
- Scorecard achieved strong risk separation

---

# 💳 Credit Scorecard Generation

Converted probability of default into business-friendly credit scores.

### Scorecard Benefits
- easy customer risk ranking
- interpretable business scoring
- lending decision support

---

# 📷 Project Visualizations

## ROC Curve

![ROC Curve](screenshots/roc_curve.png)

---

## WOE Binning

![WOE Plot](screenshots/woe_binning.png)

---

## Score Distribution

![Score Distribution](screenshots/score_distribution.png)

---

## Risk Band Analysis

![Risk Band Analysis](screenshots/risk_band_analysis.png)

---

## PSI Monitoring

![PSI Monitoring](screenshots/psi_monitoring.png)

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

✅ reduce credit losses  
✅ improve loan approval decisions  
✅ monitor portfolio quality  
✅ detect model drift  
✅ identify high-risk customers  
✅ prioritize low-risk borrowers  

---

# 🚀 Future Improvements

- Streamlit Deployment
- SHAP Explainability
- MLflow Tracking
- Real-time Monitoring Dashboard
- Automated Retraining Pipeline
- IFRS9 Probability of Default Modeling

---

# ▶️ How to Run

## Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost scorecardpy joblib
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

# 👨‍💻 Author

## Suvendu Samanta

Senior Analyst | Credit Risk Analytics | Python | PySpark | GenAI Enthusiast

---

# ⭐ Project Highlights

✅ Enterprise-style Credit Risk Modeling  
✅ Banking-grade WOE & IV Analysis  
✅ Logistic Regression Scorecards  
✅ KS & AUC Evaluation  
✅ Credit Score Generation  
✅ PSI Monitoring & Drift Detection  
✅ Business-focused Risk Segmentation  
✅ End-to-End Banking Analytics Workflow
