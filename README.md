# Aim: Exploring statistical and specialized data visualization techniques
## Theory:
The primary goal of EDA is to understand the data's structure, identify outliers, detect patterns, and test underlying assumptions before formal modeling. By combining statistical summaries with various plots—such as box plots for detecting distribution spread and scatter plots for relationship mapping—analysts can gain a comprehensive view of the dataset’s health and trends. A critical component of data analysis used to transform complex datasets into visual representations like charts and graphs to uncover patterns, trends, and correlations.

import seaborn as sns: Imports the Seaborn library, which is built on top of Matplotlib and used for creating attractive and informative statistical graphics.

import matplotlib.pyplot as plt: Imports the Matplotlib sub-module used for generating static, interactive, and animated visualizations in Python.

pd.read_csv(): Loads data from a comma-separated values (CSV) file into a structured DataFrame.

df.head(): Displays the first five rows of the DataFrame to provide a quick glimpse of the data structure and values.

df.info(): Prints a concise summary of the DataFrame, including the number of non-null entries and the data type of each column.

df.describe(): Generates descriptive statistics that summarize the central tendency, dispersion, and shape of a dataset’s distribution.

df.isnull().sum(): Checks for missing values across the dataset and returns the total count of null entries for each column.

df.drop(): Removes specified labels (rows or columns) from the DataFrame to clean or simplify the dataset.

sns.histplot(): Plots a univariate histogram to visualize the distribution of a single numerical variable.

sns.boxplot(): Creates a box-and-whisker plot to show the distribution of data and identify potential outliers.

sns.scatterplot(): Draws a scatter plot to represent the relationship between two numerical variables using dots.

plt.figure(figsize=...): Specifies the width and height of the plotting area in inches to ensure the chart is readable.

plt.title(): Adds a descriptive title to the top of the visualization for better context.

plt.show(): Displays the created plots and clears the current figure buffer.

## Conclusion:
Through this experiment, it is concluded that Exploratory Data Analysis (EDA) is an indispensable step in the data pipeline. By using functions for statistical description and visual plotting, we can effectively identify data quality issues like missing values and outliers, while simultaneously discovering meaningful correlations between variables that guide further analysis.
