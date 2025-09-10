# 📊 Workplace Equality Dataset

## Overview

This repository contains a dataset analyzing **workplace equality across different job roles and factories**.
The dataset provides an **Equality Score** and a classification into **Fairness categories** for each job role.

### Columns

* **Factory** → Name of the factory/organization.
* **Job Role** → Position or designation (e.g., C-Level, VP, Manager).
* **Equality Score** → Numerical score representing workplace equality.
* **Equality Class** → Categorized fairness level:

  * `Fair` → Equality Score within ±10
  * `Unfair` → Equality Score less than -10 or greater than 10
  * `Highly Discriminative` → Equality Score below -20 or above 20

### Sample Data

| Factory               | Job Role | Equality Score | Equality Class        |
| --------------------- | -------- | -------------- | --------------------- |
| Daikibo Factory Meiyo | C-Level  | -25            | Highly Discriminative |
| Daikibo Factory Meiyo | VP       | -26            | Highly Discriminative |
| Daikibo Factory Meiyo | Director | -19            | Unfair                |

## 🚀 Usage

You can use this dataset for:

* **Data analysis & visualization** of workplace fairness.
* **Machine learning models** predicting fairness classification.
* **Reports & dashboards** on HR and equality monitoring.

### Example (Python - Pandas)

```python
import pandas as pd

# Load dataset
df = pd.read_excel("c5915a2c-fd4d-41f3-a536-84280cce776f.xlsx")

# Show summary
print(df.head())

# Count job roles by equality class
print(df["Equality class"].value_counts())
```

## 📌 Next Steps

* Build **visualizations** (bar charts, pie charts) for equality distribution.
* Compare factories to find **patterns of fairness**.
* Extend dataset with **demographics** (gender, age, region) for deeper insights.

---
