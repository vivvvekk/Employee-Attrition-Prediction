# Employee Attrition Prediction using Logistic Regression

This project aims to predict whether an employee is likely to leave the company (attrition) using logistic regression. The model is built using a dataset from IBM HR Analytics and provides valuable insights into employee behavior.

---

## 📁 Dataset

- *Name*: WA_Fn-UseC_-HR-Employee-Attrition.csv
- *Source*: IBM HR Analytics Employee Attrition & Performance dataset
- *Target Variable*: Attrition (Yes/No)

---

## 📌 Objectives

- Predict employee attrition using logistic regression.
- Perform data preprocessing (cleaning, encoding, scaling).
- Visualize feature relationships with attrition.
- Evaluate model performance using various metrics.

---

## 📦 Libraries Used

- pandas - for data manipulation
- numpy - for numerical operations
- seaborn and matplotlib - for data visualization
- sklearn - for model building and evaluation

---

## 🔄 Workflow

### 1. Upload Dataset
```python
from google.colab import files
uploaded = files.upload()
2. Import Libraries
3. Data Preprocessing
Label encoding for categorical variables

Dropping non-informative columns

Feature scaling using StandardScaler

4. Model Training
python
Copy
Edit
model = LogisticRegression(max_iter=1000, random_state=42, class_weight='balanced')
model.fit(X_train, y_train)
5. Model Evaluation
Accuracy Score

Classification Report

Confusion Matrix

ROC Curve and AUC Score

Precision-Recall Curve

📊 Visualizations
Confusion Matrix Heatmap

ROC Curve

Precision-Recall Curve

Class Distribution

KDE Plots for features like Age, MonthlyIncome, DistanceFromHome, YearsAtCompany with respect to attrition

✅ Results
Evaluated using accuracy, precision, recall, F1-score, AUC.

Balanced class weights were used to address class imbalance.

📚 Future Work
Try other classification models like Random Forest, SVM, or XGBoost.

Perform hyperparameter tuning.

Use SMOTE for handling class imbalance.

Deploy model using Flask/Streamlit.

🙌 Acknowledgements
Dataset by IBM Watson Analytics

Implemented on Google Colab using Python
