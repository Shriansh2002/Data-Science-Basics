# Seaborn Functions

Seaborn is a powerful visualization library for Python that is built on top of Matplotlib. It provides a high-level interface for creating informative and attractive statistical graphics.

## Installation

You can install Seaborn using pip, the Python package manager, by running the following command in your terminal:

```bash
pip install seaborn
```

## List of Seaborn Functions

-   `sns.scatterplot()`: A scatter plot is a simple plot that shows the relationship between two variables. It is useful for exploring the relationship between two continuous variables.
-   `sns.lineplot()`: A line plot is a type of plot that displays information as a series of data points connected by straight line segments. It is useful for showing trends in data over time.
-   `sns.barplot()`: A bar plot is a type of plot that displays categorical data with rectangular bars. It is useful for comparing values across categories.
-   `sns.countplot()`: A count plot is a type of plot that shows the number of occurrences of each categorical variable. It is useful for exploring the distribution of categorical data.
-   `sns.boxplot()`: A box plot is a type of plot that displays the distribution of data based on five summary statistics: minimum, first quartile, median, third quartile, and maximum. It is useful for identifying outliers and visualizing the spread of data.
-   `sns.violinplot()`: A violin plot is a type of plot that combines a box plot with a kernel density plot. It is useful for visualizing the distribution of data and comparing the distributions of different variables.
-   `sns.heatmap()`: A heatmap is a type of plot that shows the relationship between two variables using color. It is useful for visualizing patterns in data and identifying correlations between variables.
-   `sns.pairplot()`: A pair plot is a type of plot that shows the pairwise relationships between variables in a dataset. It is useful for exploring the relationships between multiple variables in a dataset.
-   `sns.jointplot()`: A joint plot is a type of plot that shows the relationship between two variables using both a scatter plot and a histogram. It is useful for exploring the relationship between two continuous variables.
-   `sns.regplot()`: A regression plot is a type of plot that shows the relationship between two variables and the linear regression line that best fits the data. It is useful for exploring the relationship between two continuous variables and identifying any linear relationships.

## Usage

You can then use any of the Seaborn functions by calling them and passing in the appropriate arguments. For example:

```python
import seaborn as sns
import pandas as pd

# Load data
balance = pd.read_csv('data.csv')

# Create a scatter plot
sns.scatterplot(x='total_balance', y='balance', data=balance)
```

This will create a scatter plot of the `total_balance` and `balance` columns from the data.csv.

## Conclusion

Seaborn is a powerful visualization library that makes it easy to create informative and attractive statistical graphics in Python. By using the functions provided in this repository, you can quickly create a wide variety of plots and charts for your data.
