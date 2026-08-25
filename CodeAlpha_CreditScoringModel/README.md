# Credit Scoring Model

## CodeAlpha Machine Learning Internship

A machine learning project that predicts the likelihood of credit card default using customer demographic, credit limit, repayment history, bill amounts, and payment information.

## Project Objective

The objective is to build a classification model that can identify customers who are likely to default on their credit card payments.

## Dataset

The project uses the Default of Credit Card Clients dataset.

- 30,000 customer records
- 23 input features
- Binary target: 0 = No Default, 1 = Default

The target distribution is:

- No Default: 77.88%
- Default: 22.12%

Because the target classes are imbalanced, class-weighted models were also evaluated.

## Workflow

1. Data loading and exploration
2. Data cleaning
3. Exploratory Data Analysis
4. Feature correlation analysis
5. Data preprocessing
6. Train-test splitting
7. Model training
8. Model evaluation
9. Handling class imbalance
10. Final model analysis
11. Model saving and prediction

## Models Used

The following classification models were evaluated:

- Logistic Regression
- Decision Tree
- Random Forest

Balanced versions using `class_weight="balanced"` were also tested.

## Model Results

### Initial Models

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 0.8125 | 0.7165 | 0.2506 | 0.3713 | 0.7282 |
| Decision Tree | 0.8162 | 0.6500 | 0.3641 | 0.4668 | 0.7522 |
| Random Forest | 0.8162 | 0.6550 | 0.3550 | 0.4605 | 0.7773 |

### Balanced Models

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Balanced Logistic Regression | 0.6812 | 0.3734 | 0.6533 | 0.4752 | 0.7289 |
| Balanced Decision Tree | 0.7883 | 0.5200 | 0.5405 | 0.5301 | 0.7596 |
| **Balanced Random Forest** | **0.7745** | **0.4916** | **0.5958** | **0.5387** | **0.7761** |

## Final Model

The **Balanced Random Forest** was selected as the final model because it provided the best overall balance among the balanced models.

Final performance:

- Accuracy: 77.45%
- Precision: 49.16%
- Recall: 59.58%
- F1-Score: 53.87%
- ROC-AUC: 77.61%

## Feature Importance

The most important features identified by the final Random Forest were:

1. PAY_0 — 0.2509
2. PAY_2 — 0.0935
3. PAY_3 — 0.0575
4. PAY_4 — 0.0540
5. LIMIT_BAL — 0.0482
6. PAY_6 — 0.0455
7. BILL_AMT1 — 0.0416
8. PAY_AMT1 — 0.0413
9. PAY_AMT2 — 0.0394
10. PAY_5 — 0.0364

`PAY_0` was the most important feature.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

## Project Structure

```text
CodeAlpha_CreditScoringModel/
├── data/
├── models/
│   ├── credit_scoring_random_forest.pkl
│   └── credit_scoring_scaler.pkl
├── notebooks/
│   └── Credit_Scoring_Model.ipynb
└── README.md

## How to Run

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn ucimlrepo joblib
```

Open the notebook:

```text
notebooks/Credit_Scoring_Model.ipynb
```

Run the notebook cells from top to bottom.

## Internship

This project was completed as part of the CodeAlpha Machine Learning Internship.