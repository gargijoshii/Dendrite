# **Machine Learning Pipeline with JSON Configuration**

This repository contains a Python implementation of a dynamic machine learning pipeline that performs end-to-end data processing, feature handling, model building, and evaluation. The code is designed to be flexible, allowing different JSON configurations to control the pipeline behavior. The solution supports both classification and regression tasks with hyperparameter tuning.

---

## **Features**
1. **JSON-driven Pipeline**:
   - Parses the configuration JSON (`algoparams_from_ui`) to dynamically control pipeline steps such as feature handling, feature reduction, and model building.
   - Supports any JSON format following the predefined schema.

2. **Feature Handling**:
   - Encodes categorical variables.

3. **Feature Reduction**:
   - No Reduction.
   - PCA (Principal Component Analysis).
   - Correlation with Target.
   - Tree-based feature importance.

4. **Model Building**:
   - Dynamically selects models based on the task (`classification` or `regression`).
   - Supports multiple models with `GridSearchCV` for hyperparameter tuning.

5. **Evaluation**:
   - Logs model performance using appropriate metrics:
     - **Classification**: Accuracy, F1 Score.
     - **Regression**: Mean Squared Error (MSE).

---

## **Technologies Used**
- **Python 3.x**
- **Libraries**:
  - `scikit-learn`: For machine learning and pipelines.
  - `pandas`: For data manipulation.
  - `xgboost`: For XGBoost models.
  - `striprtf`: For parsing RTF files.

---


