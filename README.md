# SalaryScope AI 🚀
### Intelligent Developer Compensation & Workflow AI Adoption Analytics Platform
**Stack Overflow Annual Developer Survey 2024 • 65,437 Survey Respondents across 185 Countries**

[![Python 3.12](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/Framework-FastAPI-009688.svg)](https://fastapi.tiangolo.com/)
[![LightGBM](https://img.shields.io/badge/ML%20Engine-LightGBM-brightgreen.svg)](https://lightgbm.readthedocs.io/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.8.0-orange.svg)](https://scikit-learn.org/)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

---

## 👨‍🎓 Project Information
- **Project Title:** SalaryScope AI: Developer Compensation & AI-Tool Adoption Analytics
- **Student Name:** Batchu Girish Kumar
- **Registration Number:** `12506951`
- **Course Code:** INT234 (Predictive Analysis)
- **Programme & Section:** Bachelor of Technology in Computer Science and Engineering & K2P24QR
- **Supervisor / Guide:** Dr. Mrinalini Rana, Assistant Professor (U.Id 22138)
- **School:** Lovely School of Computer Science and Engineering
- **Institution:** Lovely Professional University, Phagwara, Punjab, India – 144411
- **GitHub Repository:** [https://github.com/Girishkumar0315/Salaru_Scope_AI](https://github.com/Girishkumar0315/Salaru_Scope_AI)

---

## 🌟 Executive Overview
**SalaryScope AI** is an end-to-end econometric and predictive machine learning platform that analyzes the global software engineering labor market and the unprecedented rise of AI developer tooling. Built on empirical data from the **Stack Overflow 2024 Annual Developer Survey**, the platform couples rigorous econometric hypothesis testing with production-grade gradient boosting models to solve two primary tasks:

1. **Developer Compensation Forecast (Regression):** Predicts market-clearing annual compensation in USD and local currencies (INR, EUR, GBP, CAD, AUD) accounting for geographic disparity, diminishing returns to experience, role premiums, and remote work dynamics.
2. **Workflow AI Adoption Classifier (Classification):** Accurately classifies whether a software engineer actively utilizes generative AI development tools in their daily coding workflows and quantifies developer trust versus skepticism.

---

## 🎯 6 Primary Research Objectives & Distinct Visualizations

Each core research objective is addressed with statistical tests, effect-size measures, and a **unique, dedicated chart paradigm**:

| Objective | Research Question | Visualization Type | Key Empirical Finding |
| :--- | :--- | :--- | :--- |
| **Objective 1** | Geographic Compensation Disparities & Global Tech Divide | **Lollipop Stem & Bubble Plot** (`fig_distinct_o1_lollipop.png`) | Geography alone explains **51.0% of all global pay variance** ($R^2 = 0.510$). USA median pay sits at **$150,000/yr** vs India at **$17,945/yr** (8.36× global disparity). |
| **Objective 2** | Career Experience Returns & Wage Ceiling Trajectory | **Spline Area & Trajectory Curve** (`fig_distinct_o2_curve.png`) | Strong non-linear returns (**+9.2% annual growth** from entry to 10 yrs), plateauing into a wage ceiling after **24.1 years** due to diminishing marginal utility. |
| **Objective 3** | Key Pay Determinants: Role, Remote Work & Org Size | **Econometric Forest Plot with 95% CIs** (`fig_distinct_o3_forest.png`) | **Remote work delivers the highest adjusted premium (+29.0%)**, enterprise scale pays **+22.4%**, while role premiums are led by Cloud/DevOps (+23.6%) and Engineering Management (+34.5%). |
| **Objective 4** | Workflow AI Adoption Demographics | **2D Demographic Matrix Heatmap** (`fig_distinct_o4_heatmap.png`) | Global adoption stands at **61.8%**. Strong age gradient: younger devs (<25) adopt at **74.2%–76.5%**, while adoption steadily declines to **under 48%** for senior engineers (55+). |
| **Objective 5** | The AI Trust Paradox: Sentiment, Usage, Trust & Job Fear | **Comparative Diagnostic Bar Chart** (`fig_distinct_o5_barchart.png`) | High enthusiasm (**74.2% positive sentiment**) and workflow adoption (**61.8% daily use**), but accuracy trust drops below majority to **43.1%**, demonstrating a **31.1% Trust Deficit**. Only **12.3%** perceive AI as a job threat. |
| **Objective 6** | ML Feature Importance & Predictive Audit | **Proportional Donut Ring Chart** (`fig_distinct_o6_donut.png`) | **Country of Residence dominates with 65.4%** of all model predictive weight, followed by Professional Coding Experience (**16.8%**) and Job Role (**7.5%**). |

---

## 🏆 Machine Learning Benchmark Leaderboard

Models are evaluated using **5-fold Stratified Cross-Validation** on the training set and validated once on an independent **20% held-out test split** (leakage-safe pipelines).

### 📈 Compensation Forecasting (Regression Leaderboard)
| Rank | Model Architecture | Accuracy Score | Holdout $R^2$ | Holdout MAE | MdAPE | Within $\pm 25\%$ | Status |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| 🥇 | **LightGBM (SalaryScope Core)** | **84.6%** | **0.812** | **$24,150** | **15.4%** | **82.5%** | **Champion** |
| 🥈 | HistGradientBoosting | 82.8% | 0.796 | $25,320 | 17.2% | 80.8% | Runner-up |
| 🥉 | Random Forest Ensemble | 81.5% | 0.781 | $26,110 | 18.5% | 79.4% | Benchmark |
| 4 | Regularized Ridge Regression | 80.2% | 0.765 | $27,450 | 19.8% | 78.1% | Linear Baseline |

### 🤖 Workflow AI Adoption (Classification Leaderboard)
| Rank | Model Architecture | Accuracy Score | ROC-AUC | PR-AUC | Balanced Acc. | F1-Score | Status |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| 🥇 | **LightGBM (SalaryScope Core)** | **83.4%** | **0.858** | **0.852** | **82.6%** | **86.1%** | **Champion** |
| 🥈 | HistGradientBoosting | 82.1% | 0.842 | 0.839 | 81.3% | 85.2% | Runner-up |
| 🥉 | Random Forest Classifier | 81.4% | 0.835 | 0.829 | 80.5% | 84.4% | Benchmark |
| 4 | Logistic Regression | 80.3% | 0.821 | 0.816 | 79.4% | 83.2% | Linear Baseline |

---

## 💻 Tech Stack & Architecture

- **Backend:** FastAPI (Python 3.12, Uvicorn ASGI server)
- **Machine Learning:** LightGBM, Scikit-Learn, Joblib, NumPy, Pandas, SciPy, Statsmodels
- **Explainability:** SHAP (TreeExplainer), Permutation Importance, Partial Dependence (PDP)
- **Frontend / UI:** Single-Page Architecture, Tailwind CSS, FontAwesome 6, Google Font Inter
- **Reporting:** Automated DOCX generation (Python-docx, 60+ pages with embedded 300 DPI figures)

---

## 📁 Repository Structure

```
├── README.md                                  # Repository documentation (this file)
├── app.py                                     # FastAPI application & complete web platform
├── extracted_media/                           # Official LPU crest and report assets
│   └── img_00.jpg                             # Lovely Professional University logo
└── proj/
    ├── requirements.txt                       # Python dependencies
    ├── data/
    │   ├── DATASET_DOCUMENTATION.md           # Survey provenance, licensing & schema
    │   └── processed/
    │       └── salary_cohort_clean.csv        # Cleaned developer salary cohort
    ├── models/
    │   ├── best_salary_model.joblib           # Production LightGBM salary regressor
    │   ├── best_ai_adoption_model.joblib      # Production LightGBM AI classifier
    │   └── ai_model_threshold.json            # Calibrated probability decision thresholds
    ├── notebooks/
    │   └── CA2_Predictive_Analysis.ipynb      # Executed Jupyter analysis notebook
    ├── report/
    │   └── Predictive_Analysis_CA2_Report.docx# Formal 60-page academic report (LPU format)
    ├── reports/
    │   ├── figures/                           # 36 research plots + 6 distinct objective figures
    │   │   ├── fig_distinct_o1_lollipop.png
    │   │   ├── fig_distinct_o2_curve.png
    │   │   ├── fig_distinct_o3_forest.png
    │   │   ├── fig_distinct_o4_heatmap.png
    │   │   ├── fig_distinct_o5_barchart.png
    │   │   └── fig_distinct_o6_donut.png
    │   └── results/                           # Model results JSON & statistical tables
    └── src/                                   # Reusable Python analytics package
        ├── config.py                          # Path configuration & global seeds
        ├── data_prep.py                       # Data cleaning & cohort attrition
        ├── features.py                        # Feature engineering & transformers
        ├── modeling.py                        # ML training, cross-validation & tuning
        ├── plotting.py                        # High-resolution figure generators
        └── predict.py                         # Live inference formatting & currency rates
```

---

## 🚀 Quickstart & Setup Guide

### 1. Clone the Repository
```bash
git clone https://github.com/Girishkumar0315/Salaru_Scope_AI.git
cd Salaru_Scope_AI
```

### 2. Set Up Virtual Environment & Dependencies
```bash
# Create virtual environment
python -m venv .venv

# Activate on Windows:
.venv\Scripts\activate

# Activate on Linux/macOS:
source .venv/bin/activate

# Install requirements
pip install -r proj/requirements.txt
```

### 3. Launch the SalaryScope AI Web Platform
```bash
python -m uvicorn app:app --host 127.0.0.1 --port 8000
```

Open your browser and navigate to:
👉 **[http://127.0.0.1:8000](http://127.0.0.1:8000)**

---

## 📡 REST API Endpoints

| Method | Endpoint | Description |
| :---: | :--- | :--- |
| `GET` | `/` | Serves the interactive single-page web dashboard |
| `GET` | `/api/health` | Service health status, model verification & accuracy metrics |
| `GET` | `/api/metadata` | Dataset summaries, cohort counts, and threshold parameters |
| `GET` | `/api/models` | Full regression & classification benchmark leaderboard |
| `POST` | `/api/predict/salary` | Predicts salary in USD and local currencies from developer profile |
| `POST` | `/api/predict/ai` | Predicts AI workflow adoption probability & classification decision |
| `GET` | `/report/download` | Downloads the formal academic Word report (`.docx`) |

---

## 📄 Academic Project Report

The repository includes a comprehensive 60-page academic report formatted to **Lovely Professional University (LPU)** guidelines:
- **Location:** `proj/report/Predictive_Analysis_CA2_Report.docx`
- **Features:** Complete with Declaration, Certificate, Acknowledgement, Table of Contents, 36 high-resolution figures, 28 empirical tables, and full mathematical formulations.
- **Direct Download:** Accessible via browser at `http://127.0.0.1:8000/report/download` while the server is running.

---

## 📜 Citation & Acknowledgements
- **Data Source:** [Stack Overflow Annual Developer Survey 2024](https://survey.stackoverflow.co/2024/)
- **Curation:** Havisha Khurana and the R4DS Online Learning Community (TidyTuesday 2024 Week 36)
- **Academic Framework:** Discipline of CSE/IT, Lovely School of Computer Science and Engineering, Lovely Professional University.

---

<p align="center">
  <b>SalaryScope AI</b> • Designed & Developed by <b>Batchu Girish Kumar</b> (Reg. No: 12506951) • 2026
</p>
