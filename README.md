# 🏢 Predicting Employee Attrition at Salifort Motors

This capstone project aims to support the HR department at **Salifort Motors** in improving employee satisfaction and reducing turnover. Using data collected internally, we explore the question:

**What factors are most likely to make an employee leave the company?**

As a data analytics professional, the goal was to conduct a thorough analysis and develop a machine learning model capable of predicting whether an employee is at risk of leaving, thereby enabling data-driven retention strategies.

---

## 📊 Project Objectives

- Analyse the HR dataset to uncover key trends and patterns related to attrition
- Build a predictive classification model to forecast employee attrition
- Evaluate model performance using industry-standard metrics
- Provide actionable recommendations to support employee retention efforts

---

## 🔍 Data Source

The dataset used in this project is publicly available on [Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv). It includes employee records with features related to workload, performance, satisfaction, tenure, and other workplace conditions.

---

## 🤖 Model Summary

A supervised machine learning model was trained and tested on the dataset. Key performance metrics:

- **Accuracy**: 95% — High overall correctness
- **Precision (Left)**: 81% — Of those predicted to leave, 81% actually did
- **Recall (Left)**: 93% — The model successfully identified 93% of actual leavers
- **F1-score**: 87% — Strong balance between precision and recall
- **AUC**: 0.97 — Excellent discrimination between leavers and stayers

**Error Analysis:**
- False Positives: 88 employees flagged as leavers but stayed
- False Negatives: 35 employees missed who eventually left

These figures are acceptable for the current business needs, though threshold tuning could further improve performance based on company priorities.

![image](https://github.com/user-attachments/assets/1526e9e4-9f97-4421-9b83-f718d75d6e95)

---

## 🧠 Key Predictive Features

The following variables were most influential in predicting employee attrition:

- `number_project` — Number of ongoing projects
- `last_evaluation` — Most recent performance evaluation
- `tenure` — Duration of employment
- `overworked` — Proxy for work-life balance

![image](https://github.com/user-attachments/assets/5c121b8a-5e70-4a49-ab4c-028e2049f56c)


---

## ✅ Conclusion & Recommendations

- The model provides reliable predictions of employee attrition.
- HR should focus on:
  - Monitoring workload and project assignments
  - Offering support after performance evaluations
  - Paying attention to mid-tenure employees (a common churn point)
- Regular retraining of the model is advised to prevent performance drift.
- Consider adjusting classification thresholds to align with the company's risk tolerance:
  - Prioritise **recall** to catch more potential leavers
  - Prioritise **precision** to reduce false alarms

---

## 📈 Next Steps

- Deploy the model in a test environment with real-time monitoring
- Integrate with internal HR dashboards
- Explore SHAP or LIME for model explainability
- Collect feedback from HR managers to validate the model’s recommendations

---

## 📁 Repository Contents

- `employee_attrition_model.ipynb` – Main notebook containing data analysis and model development
- `README.md` – Project overview and summary
- Dataset available on Kaggle (not included directly here)

---

## 👤 Author

**Simone Mezzabotta**  
Former Trainee, European Commission • Data Analyst • Governance & Technology Enthusiast

---

## 📄 License

This project is shared under the [MIT License](LICENSE).
