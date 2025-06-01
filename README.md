# EL_Task4

# Logistic Regression Binary Classification

This project demonstrates how to build and evaluate a Logistic Regression model for binary classification using the Breast Cancer Wisconsin (Diagnostic) dataset.

## 📂 Dataset

The dataset contains features extracted from digitized images of breast masses. Each instance is labeled as:

- **M** = Malignant (cancerous)
- **B** = Benign (non-cancerous)

### Features

- 30 numerical features (e.g., `radius_mean`, `texture_mean`, `concavity_worst`, etc.)
- 1 target column: `diagnosis`

## 🧪 Project Workflow

### 1. Data Preprocessing
- Dropped irrelevant columns
- Encoded diagnosis labels
- Standardized feature values

### 2. Train-Test Split
- 80% training, 20% test split
- Stratified to preserve class balance

### 3. Model Training
- Logistic Regression from `scikit-learn`

### 4. Evaluation Metrics
- **Confusion Matrix**
- **Precision** and **Recall**
- **AUC (Area Under Curve)**

### 5. Threshold Tuning
- Explored model behavior with different classification thresholds (default = 0.5, e.g., adjusted to 0.58)
- Explained the **sigmoid function**:
  \[
  \sigma(z) = \frac{1}{1 + e^{-z}}
  \]

## 📈 Performance

| Metric        | Value (default threshold) |
|---------------|---------------------------|
| Precision     | e.g., 0.98                 |
| Recall        | e.g., 0.98                 |
| ROC-AUC       | e.g., 1.00                 |

> Values will vary slightly depending on the threshold and train/test split.

## 📊 Visualization

- ROC curve plotted to visualize performance over all thresholds
- Showcased trade-off between TPR and FPR

## 🧠 Interpretation
- Logistic Regression is ideal for interpretable binary classification.

- ROC-AUC is a robust metric, especially for imbalanced datasets.

- Threshold tuning can significantly impact performance (e.g., recall vs precision trade-off).
