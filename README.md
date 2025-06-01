# Data Science Python Tasks

This repository contains Python scripts to clean employee data and perform analysis such as average salaries, identifying youngest and most experienced employees, and department-wise insights.

## Files

- `data_cleaning.py` - Functions to clean raw CSV-like employee data.
- `analysis.py` - Function `Analysis(data)` to perform analytics on cleaned data.

## How to Use in JupyterLab (Anaconda)

1. Prepare your raw data as a list of dictionaries (e.g., from CSV or manual input).
2. Import the cleaning and analysis functions into your Jupyter notebook or lab.
3. Clean your raw data using `clean_data()`.
4. Run analysis using `Analysis()` on the cleaned data.
5. Visualize or print results as needed.

## Example in Jupyter Notebook

```python
# Import the functions from your local scripts
from data_cleaning import clean_data
from analysis import Analysis

# Example raw data with potential inconsistencies
raw_data = [
    {"id": "1", "name": "Alice", "age": "30", "department": "Sales", "salary": "60000", "experience_years": "5"},
    {"id": "2", "name": "Bob", "age": " ", "department": "HR", "salary": "75000", "experience_years": "20"},
    {"id": "3", "name": "Charlie", "age": "25", "department": "IT", "salary": "$50000", "experience_years": "2"},
    # Add more data rows here
]

# Clean the raw data
cleaned = clean_data(raw_data)

# Perform analysis
result = Analysis(cleaned)

# Optionally: print or visualize the `result`
