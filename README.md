# Customer Churn Prediction using Random Forest

**Dataset:** Telco Customer Churn (Kaggle, by blastchar)
Source: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

**Problem:** Binary classification, predicting whether a customer churns (Yes/No)
**Model:** Random Forest Classifier (100 trees, 80/20 stratified split)
**Metrics:** Accuracy, Precision, Recall, F1-Score, Confusion Matrix

## Preprocessing
- Converted `TotalCharges` to numeric and filled missing values with the median
- Dropped `customerID`
- Label-encoded categorical columns

## Files
- Random_Forest_Churn_Prediction.ipynb`: source code
- Random_Forest_Churn_Prediction_Report.pdf


## Model file
The trained model (`random_forest_churn_model.pkl`) is not included because of its size.
Run the last cell of the notebook to generate it:

    joblib.dump(rf, "random_forest_churn_model.pkl", compress=3)

## How to run
1. Download the dataset from the Kaggle link above and place the CSV in the same folder
2. Install dependencies: `pip install pandas numpy matplotlib seaborn scikit-learn joblib`
3. Open the notebook and run all cells
