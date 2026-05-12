# 🏦 Musa National Bank

## 📌 Project Brief

As a Data Scientist in the risk management department, we have access to financial information for thousands of bank customers including outstanding debt, payment behavior, credit history, and more. Our mission:

1. **Explore & visualize** the data
2. **Prepare** the data for modeling
3. **Apply classification algorithms** to the data
4. **Evaluate** how well your models fit
5. **Select** the best model and interpret it

---

## 📁 Repository Structure

```
├── Data/                           # ⚠️ Not tracked in git — see download links below
│   ├── income.csv
│   ├── creditcard.csv
│   ├── credit_train_clean.csv
│   ├── Loan_Default.csv
│   └── Social_Network_Ads.csv
│
├── Notebooks/
│   ├── 01_Data_Prep___EDA.ipynb            # Data cleaning & exploratory analysis
│   ├── 01_EDA_assignments.ipynb            # EDA practice assignments
│   ├── 02_KNN.ipynb                        # K-Nearest Neighbors
│   ├── 02_KNN_assignments.ipynb            # KNN practice assignments
│   ├── 03_Logistic_Regression.ipynb        # Logistic Regression
│   ├── 04_Evaluation_Metrics.ipynb         # Model evaluation (AUC, ROC, F1, etc.)
│   ├── 04_metrics_assignments.ipynb        # Metrics practice assignments
│   ├── 05_Imbalanced_Data.ipynb            # Handling class imbalance (SMOTE, etc.)
│   ├── 05_Imbalanced_data_assignments.ipynb
│   ├── 06_decision_tree.ipynb              # Decision Trees
│   ├── 06_decision_tree_assignment.ipynb
│   ├── 07_Ensemble_Models.ipynb            # Random Forest & Gradient Boosting
│   ├── 07_ensemble_method_assignments.ipynb
│   ├── 07_ensemble_method_solutions.ipynb  # Assignment solutions
│   ├── 08_Pipeline_Scoring.ipynb           # Sklearn pipelines & model scoring
│   ├── 08_Pipeline.ipynb
│   └── project_credit_classification.ipynb # 🎯 Capstone project notebook
│
└── README.md
```

---

## 📊 Datasets

> **⚠️ Data files are not included in this repository** (combined size ~214MB). Download each dataset from the links below and place the files inside a `Data/` folder at the project root.

| Dataset | Rows | Features | Target | Use | Download |
|---|---|---|---|---|---|
| `credit_train_clean.csv` | 100,000 | 28 | `Credit_Score` (Good/Standard/Poor) | Main capstone project | [Kaggle →](https://www.kaggle.com/datasets/parisrohan/credit-score-classification) |
| `creditcard.csv` | 284,807 | 31 | `Class` (fraud / not fraud) | Imbalanced data module | [Kaggle →](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) |
| `income.csv` | 31,978 | 13 | `SalStat` (≤$50k / >$50k) | EDA, KNN, Logistic Reg, Ensemble modules | [Kaggle →](https://www.kaggle.com/datasets/wenruliu/adult-income-dataset) |
| `Loan_Default.csv` | 148,670 | 34 | `Status` (default / no default) | Pipeline & evaluation modules | [Kaggle →](https://www.kaggle.com/datasets/yasserh/loan-default-dataset) |
| `Social_Network_Ads.csv` | 400 | 5 | `Purchased` (0/1) | KNN introduction | [Kaggle →](https://www.kaggle.com/datasets/rakeshrau/social-network-ads) |

### Key Features in the Credit Dataset
- **Demographics:** Age, Occupation
- **Financial health:** Annual Income, Monthly Salary, Outstanding Debt, Credit Utilization Ratio
- **Credit behavior:** Num of Delayed Payments, Delay from Due Date, Payment of Minimum Amount
- **Credit profile:** Credit Mix, Credit History Age, Num of Credit Cards, Num of Loans, Interest Rate

---

## 🤖 Algorithms Covered

| Module | Algorithm | Key Concepts |
|---|---|---|
| 02 | K-Nearest Neighbors | Distance metrics, feature scaling, choosing K |
| 03 | Logistic Regression | Regularization (L1/L2), probability thresholds |
| 04 | Evaluation Metrics | Confusion matrix, precision, recall, F1, ROC-AUC |
| 05 | Imbalanced Data | SMOTE, class weighting, undersampling |
| 06 | Decision Trees | Gini impurity, max depth, pruning |
| 07 | Ensemble Methods | Random Forest, Gradient Boosting, Voting Classifier |
| 08 | Pipelines | Sklearn `Pipeline`, `GridSearchCV`, model persistence |

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn jupyter
```

### Run Locally

```bash
git clone https://github.com/your-username/musa-national-bank-credit-risk.git
cd musa-national-bank-credit-risk
```

**Set up the data** — download each CSV from the links in the Datasets table above and place them in a `Data/` folder at the project root:

```bash
mkdir Data
# move your downloaded CSVs into Data/
```

Then launch Jupyter:

```bash
jupyter notebook
```

Start with `01_Data_Prep___EDA.ipynb` if following the course progression, or jump straight to `project_credit_classification.ipynb` for the capstone.

---

## 📈 Project Workflow

```
Raw Data → EDA → Preprocessing → Feature Engineering
    → Model Training → Hyperparameter Tuning
        → Evaluation (AUC, F1, ROC) → Best Model Selection
```

The capstone notebook (`project_credit_classification.ipynb`) ties together all techniques to build a production-ready credit risk classifier, including:
- Handling missing values and outliers
- Encoding categorical variables
- Addressing class imbalance
- Comparing multiple classifiers
- Selecting and interpreting the final model

---

## 🛠️ Tech Stack

- **Python 3.11**
- **pandas** & **NumPy** — data manipulation
- **scikit-learn** — modeling, pipelines, evaluation
- **imbalanced-learn** — SMOTE and resampling strategies
- **matplotlib** & **seaborn** — visualization

---

## 📝 License

This project is for educational purposes. Dataset usage is subject to their respective sources' terms.
