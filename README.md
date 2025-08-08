# credit-default-risk-model
ML models (XGBoost, Random Forest, Logistic Regression) to predict credit default risk using financial data and loan details 
# **Target variable:** `default` (1 = defaulter, 0 = non-defaulter)
## Models & Results

| Model                | Accuracy | ROC AUC | Precision (Class 0) | Recall (Class 0) | Precision (Class 1) | Recall (Class 1) |
|----------------------|----------|---------|---------------------|------------------|---------------------|------------------|
| Logistic Regression  | 0.796    | 0.905   | 0.49                | 0.81             | 0.95                | 0.79             |
| Random Forest        | 0.8883   | 0.903   | 0.95                | 0.46             | 0.88                | 0.99             |
| XGBoost              | 0.8886   | 0.907   | 0.92                | 0.48             | 0.89                | 0.93             |

## Key Insights
- **Logistic Regression**: Balanced recall for non-defaulters but lower accuracy overall.
- **Random Forest**: Excellent at catching defaulters, but low recall for non-defaulters.
- **XGBoost**: Slightly better balance than Random Forest; best ROC AUC.
- For **risk prevention**, RF and XGBoost are strong, but may reject many good customers.

## Tech Stack
- Python (Pandas, NumPy, scikit-learn, XGBoost)
- Jupyter Notebook for experimentation & visualization
