import pandas as pd

# Creating a sample dataframe for the Excel file
data = {
    "Sales": [1500, 2300, 1800, 2700, 3200],
    "Expenses": [500, 800, 600, 900, 1000],
    "Profit": [1000, 1500, 1200, 1800, 2200]
}

df = pd.DataFrame(data)

# Save the dataframe to an Excel file
file_path = r'C:\Users\ehsan\OneDrive\Desktop\data\sample_data.xlsx'
df.to_excel(file_path, index=False)

file_path

