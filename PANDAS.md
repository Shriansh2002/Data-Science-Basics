# Pandas Functions

Pandas is an open-source data manipulation library for Python. It is built on top of the NumPy library and provides easy-to-use data structures and data analysis tools for handling tabular, time-series, and statistical data.

## Installation

You can install pandas using pip:

```bash
pip install pandas
```

## Basic Usage

Once you have installed Pandas, you can start using it in your Python programs. Here are some basic examples of how to use Pandas:

```python
import pandas as pd

# create a DataFrame
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Charlie', 'David'],
    'Age': [25, 30, 35, 40],
    'City': ['New York', 'Paris', 'London', 'Tokyo']
})

# display the DataFrame
print(df)
```

This will create a DataFrame with three columns (Name, Age, and City) and four rows of data, and then display the DataFrame in the console.

## Reading and Writing Data

Pandas provides functions for reading and writing data to and from various file formats, such as CSV, Excel, and SQL databases. Here are some examples:

```python
import pandas as pd

# read data from a CSV file
df = pd.read_csv('data.csv')

# write data to an Excel file
df.to_excel('data.xlsx', index=False)

# read data from a SQL database
import sqlite3
conn = sqlite3.connect('example.db')
df = pd.read_sql('SELECT * FROM my_table', conn)
conn.close()
```

## Data Selection and Filtering

Pandas provides powerful tools for selecting and filtering data from DataFrames. Here are some examples:

```python
import pandas as pd

# create a DataFrame
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Charlie', 'David'],
    'Age': [25, 30, 35, 40],
    'City': ['New York', 'Paris', 'London', 'Tokyo']
})

# select a column
ages = df['Age']

# filter rows
londoners = df[df['City'] == 'London']

# select rows and columns
subset = df.loc[[0, 2], ['Name', 'Age']]
```

## Data Aggregation and Grouping

Pandas provides functions for aggregating and grouping data in various ways. Here are some examples:

```python
import pandas as pd

# create a DataFrame
df = pd.DataFrame({
    'Name': ['Alice', 'Bob', 'Charlie', 'David'],
    'Age': [25, 30, 35, 40],
    'City': ['New York', 'Paris', 'London', 'Tokyo']
})

# calculate the mean age
mean_age = df['Age'].mean()

# group by city and calculate the mean age for each city
mean_age_by_city = df.groupby('City')['Age'].mean()
```

## Conclusion

Pandas is a powerful data manipulation library for Python that provides easy-to-use tools for working with tabular, time-series, and statistical data. This README file has provided some basic examples of how to use Pandas, but there is much more to explore. To learn more, check out the official [Pandas Documentaion](https://pandas.pydata.org/docs/).
