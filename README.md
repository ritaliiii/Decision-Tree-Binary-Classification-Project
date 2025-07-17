# Decision Tree Binary Classification Project

This project applies the **Decision Tree Classifier** on a binary classification dataset in two settings — **with and without a depth limit** — and compares their evaluation metrics to assess performance trade-offs.

---

## Objective

Evaluate two Decision Tree models:
1. **No depth limit**
2. **Max depth = 1**

For each model, the following metrics are assessed:
- Accuracy
- Precision & Recall
- Classification Report
- Confusion Matrix
- ROC Curve
- Precision-Recall Curve

---

## Dataset

The dataset (`data.csv`) contains labeled fraud detection data, where the target variable `Fraud` is binary:
- `"Yes"` → `1` (Fraudulent)
- `"No"` → `0` (Not Fraudulent)

### Features:
All columns excluding `Fraud` are used as features (`X`).

---

## Methodology

1. **Preprocessing**
   - Categorical label mapped to binary (0 and 1).
   - Split into train/test (80/20).
2. **Model Training**
   - Train two DecisionTreeClassifier models:
     - `max_depth=None` (default)
     - `max_depth=1` (shallow tree)
3. **Model Evaluation**
   - Accuracy, Precision, Recall
   - Classification Report
   - Confusion Matrix
   - ROC and Precision/Recall curves

## Visualization Excerpts
