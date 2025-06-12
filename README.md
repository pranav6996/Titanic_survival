
# 🚢 Titanic Survival Prediction (Random Forest)

This project predicts passenger survival on the Titanic using a complete scikit-learn ML pipeline with preprocessing, feature engineering, and a Random Forest classifier.

---

## 📦 Dataset
We used the Titanic dataset from Seaborn:
### 🎯 Target Variable
- `survived`: 0 = No, 1 = Yes
## 🔧 Preprocessing Steps

### ➕ Numerical Features
- Columns detected automatically using `select_dtypes`
- Preprocessing:
  - `SimpleImputer(strategy='median')` for missing values
  - `StandardScaler()` for scaling

### 🟪 Categorical Features
- Columns detected with `select_dtypes` for object/category
- Preprocessing:
  - `SimpleImputer(strategy='most_frequent')`
  - `OneHotEncoder(handle_unknown='ignore')`

### ⚙️ Combined using `ColumnTransformer`
## 🧠 Model
- **Random Forest Classifier**
```python
## 📈 Evaluation
- `classification_report`
- `confusion_matrix`
- Visualized using `ConfusionMatrixDisplay`
