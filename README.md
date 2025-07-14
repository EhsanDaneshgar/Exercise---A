# 🐼 Exporting a Pandas DataFrame to Excel

This mini demo shows how to create a simple pandas DataFrame and export it to an Excel file using Python. It’s a basic but essential operation in data analysis workflows.

---

## 📄 What the Script Does

1. Creates a DataFrame with sample `Sales`, `Expenses`, and `Profit` data.
2. Saves the DataFrame to an Excel file using `pandas.to_excel()`.

---

## 🧪 Sample Code

```python
import pandas as pd

# Creating a sample dataframe
data = {
    "Sales": [1500, 2300, 1800, 2700, 3200],
    "Expenses": [500, 800, 600, 900, 1000],
    "Profit": [1000, 1500, 1200, 1800, 2200]
}

df = pd.DataFrame(data)

# Saving to Excel
file_path = r'C:\Users\ehsan\OneDrive\Desktop\data\sample_data.xlsx'
df.to_excel(file_path, index=False)

file_path

