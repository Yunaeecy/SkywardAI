# 🪅 Pandas DataFrame

Pandas DataFrame is a two-dimensional, tabular data structure in the Python programming language provided by the Pandas library. It is similar to a spreadsheet or SQL table, where data is organized in rows and columns. Each column can have a different data type (e.g., integers, floats, strings), and you can perform various operations on the data, such as filtering, grouping, and aggregation.

Here are some key features and concepts related to Pandas DataFrame:

1. Structure: a DataFrame consists of rows and columns. Each column is a Pandas Series, which is a one-dimentional labeled array.
2. Index: rows and columns are both labeled. The row labels are refered to as the "index", and the column labels are the names of the columns.
3. Creation: you can create a DataFrame from various data structure, such as lists, dictionaries, NumPy arrays, or even other DataFrames.



```python
import pandas as pd

# Creating a DataFrame from a dictionary
data = {'Name': ['Alice', 'Bob', 'Charlie'],
        'Age': [25, 30, 35],
        'City': ['New York', 'San Francisco', 'Los Angeles']}

df = pd.DataFrame(data)

```

Reading and writing data: Pandas supports reading data from various file formats, such as CSV, Excel, SQL databases, and more. It can also write data back to those formats.



```python
# Reading from a CSV file
df = pd.read_csv('example.csv')

# Writing to a CSV file
df.to_csv('output.csv', index=False)

```
