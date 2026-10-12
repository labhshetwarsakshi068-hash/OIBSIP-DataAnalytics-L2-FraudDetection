# Credit Card Fraud Detection

## Project Overview
This project detects fraudulent credit card transactions using Machine Learning classification algorithms.

## Objectives
- Analyze credit card transaction data.
- Explore the imbalance between legitimate and fraudulent transactions.
- Train and evaluate Logistic Regression and Random Forest models.
- Compare model performance using precision, recall, F1-score, and confusion matrix.

## Dataset
- Total transactions: 284,807
- Total features: 30
- Target column: `Class`
- Legitimate transactions (`Class = 0`): 284,315
- Fraudulent transactions (`Class = 1`): 492
- Missing values: 0

## Data Preprocessing
- Separated features and target variable.
- Split data into 80% training and 20% testing sets.
- Used stratified splitting to preserve the class distribution.
- Applied StandardScaler to the features for Logistic Regression.

## Models Used
1. Logistic Regression
2. Random Forest Classifier

## Model Results

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Logistic Regression | 97.75% | 6.10% | 91.84% | 11.44% |
| Random Forest | 99.95% | 89.53% | 78.57% | 83.70% |

## Conclusion
Random Forest achieved higher precision and F1-score on the test set, while Logistic Regression detected a larger proportion of fraudulent transactions. Since the dataset is highly imbalanced, precision, recall, and F1-score are important evaluation metrics in addition to accuracy.

## Project Files
- `Fraud_Detection.ipynb` — Data analysis, visualization, model training, and evaluation.
- `creditcard.csv` — Dataset.
- `model_comparison.csv` — Model evaluation comparison.
- `README.md` — Project documentation.