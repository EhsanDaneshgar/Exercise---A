# 📊 Pandas Excel Export Demo

This is a simple Python script that creates a small dataset using the `pandas` library and saves it to an Excel file. The file will be saved to a specific folder on your computer. This demo is ideal for beginners learning how to export tabular data from Python to Excel.

## 💻 What It Does

- Creates a table with 3 columns: **Sales**, **Expenses**, and **Profit**
- Saves the data to an Excel file at:
  
  `C:\Users\ehsan\Desktop\data\sample_data.xlsx`

## 🧪 Sample Code

```python
import pandas as pd

# Create data
data = {
    "Sales": [1500, 2300, 1800, 2700, 3200],
    "Expenses": [500, 800, 600, 900, 1000],
    "Profit": [1000, 1500, 1200, 1800, 2200]
}
df = pd.DataFrame(data)

# Define file path
file_path = r'C:\Users\ehsan\Desktop\data\sample_data.xlsx'

# Save to Excel
df.to_excel(file_path, index=False)

print("Excel file saved to:", file_path)




