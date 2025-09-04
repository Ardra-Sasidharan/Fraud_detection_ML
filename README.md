#Credit Card Fraud Detection  

This project detects fraudulent credit card transactions using Machine Learning.  
It includes **Exploratory Data Analysis (EDA)**, **Data Preprocessing**, **Model Training**, **Evaluation**, and a **Tkinter GUI App** for predictions.  

---

# Dataset  
The dataset used is the [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) from Kaggle.  

- **Transactions**: 284,807  
- **Fraud cases**: 492 (~0.17%) → highly imbalanced dataset  
- **Features**: 30 anonymized features + `Amount` + `Time`  

---

---

## ⚙️ Steps in the Notebook  

1. **Exploratory Data Analysis (EDA)**  
   - Checked dataset shape, fraud percentage, missing values  
   - Visualized fraud vs non-fraud transactions  

2. **Data Preprocessing**  
   - Scaled features (`StandardScaler`)  
   - Handled class imbalance using `SMOTE`  

3. **Model Training**  
   - Logistic Regression  
   - Decision Tree  
   - Random Forest (final chosen model)  

4. **Evaluation Metrics**  
   - Accuracy, Precision, Recall, F1-score  
   - ROC-AUC Curve  

5. **Model Saving**  
   - Saved trained Random Forest model using `joblib`  

6. **Tkinter GUI App**  
   - User enters transaction details  
   - Model predicts whether transaction is **Fraud** or **Not Fraud**  

---
📌 Requirements

-Python 3.x

-pandas, numpy, scikit-learn, joblib

-imbalanced-learn (for SMOTE)

-matplotlib, seaborn

-tkinter (built-in with Python)

Results

Random Forest performed best with ~99.9% ROC-AUC score

Achieved strong fraud detection while reducing false negatives


