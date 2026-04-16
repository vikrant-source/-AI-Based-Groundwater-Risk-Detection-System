# 🌊 AI-Based Groundwater Risk Detection System
### INT-375 Data Science Project | Lovely Professional University

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-orange)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 📌 Project Overview

This project analyzes **India's groundwater levels from 2015–2022** using the
Atal Jal Scheme dataset. It builds a complete **Risk Detection Pipeline** to
classify groundwater zones as Safe, Moderate, or High Risk using statistical
analysis, data visualization, and machine learning.

---

## 🎯 Objectives

| # | Objective |
|---|-----------|
| 1 | Analyze groundwater level trends across Indian states (2015–2022) |
| 2 | Detect outliers using IQR and Z-Score methods |
| 3 | Compute a Risk Score and classify regions into Safe / Moderate / High Risk |
| 4 | Perform Statistical Hypothesis Testing (T-test, Z-test) |
| 5 | Build a Linear Regression model to predict Pre-monsoon 2022 levels |

---

## 🧮 Risk Score Formula

Risk Score = (Pre_norm + Post_norm + Trend_norm + Depth_norm) / 4

| Score Range | Zone       |
|-------------|------------|
| 0 – 30      | ✅ Safe    |
| 30 – 60     | ⚠️ Moderate |
| 60+         | 🔴 High Risk |

---

## 📊 Visualizations

- Correlation Heatmap
- District-wise Risk Score Ranking (Bar Chart)
- Boxplot Outlier Detection (by State & Risk Zone)
- Histogram Distribution (with Mean line)
- Risk Zone Pie Chart
- Missing Values Heatmap
- State Comparison Bar Graph
- Pairplot (by Well Type)
- Linear Regression — Actual vs Predicted
- Scatter Plot (Pre vs Post Monsoon by Risk Zone)

---

## 🔬 Statistical Tests

| Test | Purpose | Result |
|------|---------|--------|
| One-sample T-test | GW level vs national benchmark | Significant |
| Two-sample T-test | Safe vs High Risk zones | Significant |
| Z-test | Risk Score vs safe benchmark 30 | Significant |

---

## 🤖 ML Model

- **Algorithm:** Linear Regression
- **Features:** Pre/Post monsoon levels 2019–2021
- **Target:** Pre-monsoon 2022 groundwater level
- **Metrics:** MAE, MSE, R²

---

## 💻 Tech Stack

| Library | Usage |
|---------|-------|
| Pandas | Data loading, cleaning, manipulation |
| NumPy | Numerical operations, outlier detection |
| Matplotlib | Bar charts, pie charts, scatter plots |
| Seaborn | Heatmap, boxplot, pairplot, violin plot |
| SciPy | T-test, Z-test hypothesis testing |
| Scikit-learn | Linear Regression, train-test split, metrics |

---

## 📁 Project Structure
groundwater-risk-analysis-system/
│
├── INT375_Groundwater_Project.ipynb   ← Main Jupyter Notebook
├── groundwater_cleaned.csv            ← Cleaned dataset
├── charts/                            ← All generated visualizations
│   ├── 01_correlation_heatmap.png
│   ├── 02_district_ranking.png
│   ├── 03_boxplot_outliers.png
│   ├── 04_histogram_distribution.png
│   ├── 05_risk_zone_pie.png
│   ├── 06_missing_values_heatmap.png
│   ├── 07_state_comparison.png
│   ├── 08_pairplot.png
│   └── 09_linear_regression.png
└── README.md

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/groundwater-risk-analysis-system.git

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter

# 3. Open the notebook
jupyter notebook INT375_Groundwater_Project.ipynb
```

---

## 📝 Git Commit History

Initial project setup — README and folder structure
Added dataset — groundwater 2015-2022 India data
Added data cleaning — fillna, dropna, replace Dry values
Added risk score formula — Safe/Moderate/High Risk classification
Added EDA — state comparison and aquifer analysis
Added visualizations — heatmap, boxplot, histogram, pairplot
Added outlier detection — IQR and Z-Score methods
Added statistical tests — T-test and Z-test with conclusions
Added ML model — Linear Regression with R2 and Actual vs Predicted
Final notebook — conclusion and project documentation

---

## 🔑 Key Findings

- **Rajasthan & Punjab** are in the High Risk zone with severely depleted groundwater
- **Bihar & Kerala** show relatively stable and shallow groundwater levels
- **Strong correlation** exists between consecutive years — historical data reliably predicts future levels
- **Unconfined aquifers** are most vulnerable, dominating ~50% of the dataset
- Linear Regression model confirms groundwater trends are **temporally consistent**

---

## 👨‍💻 Author

**Vikrant Verma**
B.Tech CSE | Lovely Professional University
📧 vikrant377.vr@gmail.com
🔗 www.linkedin.com/in/vikrant-verma-5a7614274

---

#Python #DataScience #MachineLearning #Groundwater #LPU #INT375
