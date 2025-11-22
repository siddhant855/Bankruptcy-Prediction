# 📘 Bankruptcy Prediction Using Logistic Regression

This project implements a **manual Logistic Regression model** to predict corporate bankruptcy using financial ratios. All computations — including gradient descent, loss calculation, and prediction — are implemented **from scratch in NumPy** inside a single Jupyter Notebook.

The notebook demonstrates a complete ML pipeline:

* ✔ Data preprocessing
* ✔ Mini-batch gradient descent
* ✔ Hyperparameter tuning
* ✔ Threshold optimization
* ✔ Performance evaluation
* ✔ Prediction on new company inputs

---

## 📂 Repository Contents

```
📄 Bankruptcy_Prediction.ipynb     # Main notebook (full implementation)
📄 best_model_summary.csv          # Best hyperparameters + test metrics
📄 data.csv (optional)             # Dataset
🖼️ plots/ (optional)               # Confusion matrix, PR curve, loss curve, etc.
```

---

## 📊 Project Highlights

### 🔹 Manual Logistic Regression (No sklearn model)

Implemented entirely from scratch:

* Sigmoid activation
* Weight & bias initialization
* Mini-batch gradient descent
* Cost (loss) monitoring
* Custom prediction + threshold decision

### 🔹 Hyperparameter Search

Grid search over:

* Learning rates
* Epoch counts
* Batch size

Best configuration is saved in **best_model_summary.csv**.

### 🔹 Threshold Tuning

Bankruptcy datasets are **highly imbalanced**, so accuracy alone is misleading. Threshold tuning improves:

* Recall (ability to catch bankrupt firms)
* Overall risk detection
* Real-world applicability

---

## 📈 Model Results

Extracted from `best_model_summary.csv`:

| Metric              | Value        |
| ------------------- | ------------ |
| Learning Rate       | 0.0005       |
| Epochs              | 1500         |
| Batch Size          | 64           |
| Validation Accuracy | 0.964809384  |
| Test Accuracy       | 0.958944281  |
| Precision           | 0.354838709  |
| Recall              | 0.333333333  |




## 🖼️ Visualizations (Generated in Notebook)

* Confusion Matrix
* Precision–Recall Curve
* Loss (Cost) vs Epochs
* Accuracy vs Precision vs Recall vs Threshold

Include them in `/plots` for GitHub previews.

---

## 🚀 Running the Notebook

### 1️⃣ Install dependencies

```bash
pip install numpy pandas matplotlib scikit-learn
```

### 2️⃣ Launch Jupyter

```bash
jupyter notebook
```

### 3️⃣ Open and run

Open:

```
Bankruptcy_Prediction.ipynb
```

Run all cells (**Kernel → Restart & Run All**).

---

## 🧪 Predicting Bankruptcy on New Data

Paste your inputs:

```python
input1 = [ ... feature values ... ]
input2 = [ ... feature values ... ]
```

The notebook outputs:

* Standardized input
* Probability of bankruptcy
* Final prediction (0 = safe, 1 = bankrupt)

---

## 📌 Interpretation Summary

* Logistic Regression provides transparent and explainable predictions.
* Threshold tuning improves detection of high-risk companies.
* Acts as an **early-warning financial risk system**.
* Provides meaningful and practical insights for analysts, auditors, and regulators.

---
