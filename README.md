
# Breast Cancer Classification with Logistic Regression

This project uses the Breast Cancer Wisconsin dataset to build a binary classification model that predicts whether a tumor is malignant or benign. The pipeline includes data preprocessing, model training, evaluation using key metrics, and threshold tuning for optimal performance.

## Dataset
- Source: Kaggle - [Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

- Features: 30 numeric features derived from digitized images of fine needle aspirate (FNA) of breast mass.

- Target: diagnosis — Malignant (M) or Benign (B)
## Workflow Summary
- Load and clean dataset (drop ID, handle missing values)
- Encode target labels (M → 1, B → 0)
- Train-test split (80/20)
- Standardize features using StandardScaler
- Fit Logistic Regression model
- Evaluate with confusion matrix, precision, recall, ROC-AUC
- Tune decision threshold and visualize ROC curve
## Evaluation Metrics
- Confusion Matrix
- Precision & Recall
- ROC-AUC Score
- Threshold Tuning: Adjusted to improve recall for malignant cases
## Dependencies
```python
pip install pandas numpy scikit-learn matplotlib seaborn
```
## File Structure
```python
breast_cancer_logistic/
│
├── data.csv
├── breast_cancer_logistic.ipynb
├── README.md
```
