# Disease Prediction

## CodeAlpha Machine Learning Internship

This project uses machine learning to predict the presence of heart disease based on patient medical information.

A Random Forest Classifier is trained on the UCI Heart Disease dataset and evaluated using accuracy, classification metrics, and a confusion matrix.

## Dataset

The project uses the **UCI Heart Disease Dataset**.

- Dataset: UCI Heart Disease Dataset
- Records: 303
- Features: 13
- Target: Presence or absence of heart disease

The original target values are converted into a binary classification:

- `0` → No Heart Disease
- `1` → Heart Disease

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

## Project Structure

```text
DiseasePrediction/
│
├── data/
│   └── heart_disease.csv
│
├── models/
│   └── disease_prediction_random_forest.pkl
│
├── notebooks/
│   └── Disease_Prediction.ipynb
│
├── README.md
└── requirements.txt
```

## Methodology

The project follows these steps:

1. Load the heart disease dataset.
2. Explore the dataset and identify missing values.
3. Handle missing values using the mode.
4. Convert the target into a binary classification problem.
5. Split the data into training and testing sets.
6. Train a Random Forest Classifier.
7. Evaluate the model using accuracy and a classification report.
8. Generate a confusion matrix.
9. Save the trained model using Joblib.
10. Load the saved model and verify its predictions.

## Model Performance

The trained Random Forest model achieved:

- **Test Accuracy:** 88.52%
- **Model:** Random Forest Classifier
- **Dataset:** UCI Heart Disease Dataset

### Classification Results

| Class | Precision | Recall | F1-Score |
|------|-----------|--------|----------|
| No Disease | 0.93 | 0.85 | 0.89 |
| Disease | 0.84 | 0.93 | 0.88 |

## How to Run

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
notebooks/Disease_Prediction.ipynb
```

Run the notebook cells from top to bottom.

## Model

The trained model is saved as:

```text
models/disease_prediction_random_forest.pkl
```

The saved model can be loaded using Joblib for future predictions.

## Internship

This project was completed as part of the **CodeAlpha Machine Learning Internship**.