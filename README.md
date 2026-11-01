# Understanding Data & Correlation Using Python

## 📌 Project Overview
This project focuses on understanding a dataset and finding relationships between numerical and categorical features using Python and Pandas.

## 🎯 Objectives
- Understand dataset structure.
- Explore rows and columns.
- Identify numerical and categorical data.
- Calculate correlation between features.
- Visualize relationships using a correlation heatmap.

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📚 Topics Covered

### 1. Load Dataset
```python
import pandas as pd

df = pd.read_csv("dataset.csv")
```

### 2. Explore Dataset
```python
df.head()
df.tail()
df.shape
df.info()
df.describe()
```

### 3. Check Data Types
```python
df.dtypes
```

### 4. Calculate Correlation
```python
df.corr(numeric_only=True)
```

### 5. Encode Categorical Data
```python
df_encoded = pd.get_dummies(df, drop_first=True, dtype=int)
```

### 6. Correlation Matrix
```python
correlation = df_encoded.corr()
print(correlation)
```

### 7. Correlation Heatmap
```python
import seaborn as sns
import matplotlib.pyplot as plt

plt.figure(figsize=(15, 10))
sns.heatmap(correlation, cmap="coolwarm")
plt.show()
```

## 📖 What I Learned
- How to understand a dataset.
- How to identify different data types.
- How to calculate correlation.
- How to find relationships between features.
- How to visualize correlation using a heatmap.

## 🚀 Conclusion
This project helped me understand data exploration and correlation analysis, which are important steps in Machine Learning and Exploratory Data Analysis (EDA).

---
**Author:** AI / Machine Learning Learner
