# Task 4: Binary Classification with Logistic Regression

## Internship Objective
Build a **binary classifier** using **Logistic Regression** to identify whether a tumor is malignant or benign using the **Breast Cancer Wisconsin Dataset**.

---

##  Dataset
- **Source**: Breast Cancer Wisconsin (Diagnostic)
- **Shape**: 569 rows × 32 columns (after removing ID & null column)
- **Target Feature**: `diagnosis`
  - `M` → Malignant (1)
  - `B` → Benign (0)

---

##  Tools & Libraries Used
- Python
- `pandas`, `numpy`
- `scikit-learn`
- `matplotlib`, `seaborn`

---

##  Steps Performed

1. **Data Cleaning**
   - Dropped unnecessary columns: `id`, `Unnamed: 32`
   - Encoded target labels (M → 1, B → 0)

2. **Train-Test Split**
   - 80% training, 20% testing

3. **Feature Scaling**
   - Applied `StandardScaler` to normalize input features

4. **Model Training**
   - Used `LogisticRegression()` with `max_iter=1000`

5. **Evaluation Metrics**
   - Confusion Matrix
   - Classification Report (Precision, Recall, F1-Score)
   - ROC-AUC Score & Curve
   - Threshold tuning example (0.6)

6. **Sigmoid Function**
   - Plotted sigmoid curve to explain logistic function behavior

---

##  Evaluation Results

| Metric      | Score     |
|-------------|-----------|
| Accuracy    | 97%       |
| Precision   | 98%       |
| Recall      | 95%       |
| ROC-AUC     | 0.99+     |

---

## Custom Threshold (0.6)

Tuned the threshold to 0.6 instead of the default 0.5 to evaluate how prediction sensitivity changes.

---

##  Visualizations Included

-  Confusion Matrix
-  ROC Curve
-  Sigmoid Function
