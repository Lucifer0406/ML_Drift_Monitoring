# Customer Churn Monitoring with Data Drift Detection

This project demonstrates an end-to-end machine learning workflow:  
model training, simulated production data drift, statistical drift detection, and automated model risk assessment.

---

## 🔍 Project Overview

The goal is not only to predict customer churn, but to monitor whether the data environment changes over time and whether such changes impact model behavior.

The system:
- Trains a churn prediction model
- Simulates real-world data drift
- Detects feature-level data drift statistically
- Measures prediction shift
- Produces an automated **MODEL_OK / MODEL_AT_RISK** decision

---

## 📁 Structure

```
customer-churn-drift/
│
├── model_training.ipynb
├── data_drift_simulation.ipynb
├── model_monitoring.ipynb
│
├── data/
├── models/
├── reports/
├── requierments.txt
└── README.md
```

---

## 🚀 How to Run

=>Firstly, get all the requirements:
```bash
pip install -r requirements.txt
```

1. Train the model:
```bash
python model_training.ipynb
```

2. Simulate data drift:
```bash
python data_drift_simulation.ipynb
```

3. Run monitoring:
```bash
python model_monitoring.ipynb
```

This generates:
- `reports/monitoring_summary.csv`
- `reports/feature_drift_report.csv`

---

## 🧠 Key Concepts Demonstrated

- Data drift detection (KS test, Chi-square)
- Prediction shift analysis
- Threshold-based model risk alerts
- Reusable monitoring pipeline

---

## 📌 Outcome

The system automatically determines whether the deployed model is still reliable based on both data distribution changes and their impact on predictions.

---

## 👨‍💻 Author

Built as a portfolio project to demonstrate production-style machine learning monitoring and MLOps fundamentals.
