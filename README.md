---

````markdown
# 🧹 Loan Data Cleaning & Preprocessing

This project focuses on cleaning, transforming, and preparing a loan dataset for machine learning models. It includes handling missing values, fixing categorical variables, and applying encoding techniques like OneHotEncoder.

## 📌 Objective

Prepare a raw loan dataset for ML-ready analysis by:
- Cleaning inconsistencies
- Handling missing values
- Converting data types
- Encoding categorical variables

---

## 📁 Dataset Info

The dataset includes common loan-related features like:

- `Loan_ID`
- `Gender`
- `Married`
- `Dependents`
- `Education`
- `Self_Employed`
- `ApplicantIncome`
- `CoapplicantIncome`
- `LoanAmount`
- `Loan_Amount_Term`
- `Credit_History`
- `Property_Area`
- `Loan_Status`

---

## 🔧 Data Cleaning Steps

- Replaced `'3+'` with `3` in `Dependents`
- Converted `Dependents` to numeric type
- Handled `NaN` using mean or mode as appropriate
- Removed or filled missing data in other columns
- Checked and dropped duplicates if any
- Verified correct data types

---

## 🔠 Categorical Encoding

Used **OneHotEncoding** on key categorical columns:
- `Gender`
- `Married`
- `Education`
- `Self_Employed`
- `Property_Area`
- `Loan_Status`

```python
from sklearn.preprocessing import OneHotEncoder
encoder = OneHotEncoder()
encoded = encoder.fit_transform(df[['Married']]).toarray()
````

---

## 📊 Tools & Libraries

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

## ▶️ How to Run

1. Clone the repo:

```bash
git clone https://github.com/alokbhateshwar/lean-data-pipeline-.git
```

2. Open `main.ipynb` in Jupyter Notebook

3. Follow through the notebook to understand each step

---

## 📌 Future Enhancements

* Feature scaling (StandardScaler / MinMaxScaler)
* Imbalanced target handling (SMOTE)
* Model training (Logistic Regression, Random Forest)
* Deployment as a Streamlit app

---

## 📄 License

This project is under the MIT License.

---

Built with ❤️ by [Alok Bhateshwar](https://github.com/alokbhateshwar)

```

