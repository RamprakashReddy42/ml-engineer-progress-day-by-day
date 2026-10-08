# 💳 Credit Card Fraud Detection — Machine Learning

A Machine Learning project for detecting **fraudulent credit card transactions** using Python and Machine Learning techniques.

This project follows a step-by-step Machine Learning workflow, starting with **Data Understanding** and gradually moving toward preprocessing, model training, evaluation, and prediction.

---

# 📌 PHASE 1 — DATA UNDERSTANDING

## ✅ Progress

| Step | Task                  | Status      |
| ---- | --------------------- | ----------- |
| 1    | Load Dataset          | ✅ Completed |
| 2    | Understand Dataset    | ✅ Completed |
| 3    | Check Shape           | ✅ Completed |
| 4    | Check Columns         | ✅ Completed |
| 5    | Check Data Types      | ✅ Completed |
| 6    | Check Missing Values  | ✅ Completed |
| 7    | Handle Missing Values | ✅ Completed |

---

## 1️⃣ Load Dataset

The Credit Card Fraud Detection dataset was loaded using Pandas.

```python
import pandas as pd

df = pd.read_csv("creditcard.csv")

print(df.head())
```

---

## 2️⃣ Understand Dataset

The dataset was initially inspected to understand its structure, features, and statistical information.

```python
df.head()
df.info()
df.describe()
```

These functions help us understand:

* Dataset structure
* Number of features
* Data types
* Statistical information
* Possible data-quality issues

---

## 3️⃣ Check Dataset Shape

The number of rows and columns was checked using:

```python
df.shape
```

The output represents:

```text
(number_of_rows, number_of_columns)
```

This helps us understand the size of the dataset.

---

## 4️⃣ Check Columns

The names of all columns were checked using:

```python
df.columns
```

Typical columns in the Credit Card Fraud Detection dataset include:

```text
Time
V1
V2
V3
...
V28
Amount
Class
```

The target variable is:

```text
Class
```

where:

```text
0 → Legitimate Transaction
1 → Fraudulent Transaction
```

---

## 5️⃣ Check Data Types

The data types of all columns were checked using:

```python
df.dtypes
```

This helps identify whether the columns contain:

* Integer values
* Floating-point values
* Other data types

Correct data types are important for further Machine Learning processing.

---

## 6️⃣ Check Missing Values

Missing values were checked using:

```python
df.isnull().sum()
```

This step helps identify whether any feature contains missing or null values.

The result was examined for every column in the dataset.

---

## 7️⃣ Handle Missing Values

After checking for missing values, the dataset was cleaned accordingly.

If missing values are present, they can be handled using techniques such as:

```python
df["column_name"] = df["column_name"].fillna(
    df["column_name"].median()
)
```

After handling the missing values, the dataset was verified again:

```python
df.isnull().sum()
```

### ✅ Result

```text
Missing values checked and handled successfully.
```

---

# 🎯 Project Objective

The main objective of this project is to build a Machine Learning model that can classify credit card transactions as:

```text
0 → Legitimate
1 → Fraudulent
```

---

# 🗂️ Dataset Features

| Feature    | Description                       |
| ---------- | --------------------------------- |
| `Time`     | Time elapsed between transactions |
| `V1`–`V28` | Anonymized transaction features   |
| `Amount`   | Transaction amount                |
| `Class`    | Target variable indicating fraud  |

---

# 🛠️ Technologies Used

* 🐍 Python
* 🐼 Pandas
* 🔢 NumPy
* 🤖 Scikit-learn
* 📊 Matplotlib
* 📈 Seaborn
* 📓 Jupyter Notebook
* 🔧 Git & GitHub

---

# 📊 Phase 1 Progress

```text
PHASE 1 — DATA UNDERSTANDING

1. Load Dataset          ✅
2. Understand Dataset    ✅
3. Check Shape           ✅
4. Check Columns         ✅
5. Check Data Types      ✅
6. Check Missing Values  ✅
7. Handle Missing Values ✅
```

### Progress: `7 / 7` ✅

---

# 🔜 Next Phase

**Phase 2 — Exploratory Data Analysis (EDA)**

The next phase will analyze the dataset and identify important patterns and relationships between transaction features and fraud.

---

## 👨‍💻 Author

**Ram Prakash Reddy**

B.Tech — Artificial Intelligence & Data Science

**Skills:** Python | SQL | Machine Learning | Power BI | Data Analysis
