# Aim: Exploring statistical and specialized data visualization techniques
## Theory:
While basic charts such as line plots, bar charts, histograms, and scatter plots are used for general data exploration, statistical and specialized visualizations provide deeper analytical insights. They help reveal distribution spread, outliers, correlations between multiple variables, and proportional breakdowns that simpler charts cannot express. Python's Matplotlib and Seaborn libraries together provide a comprehensive suite for these advanced chart types. By combining statistical summaries with various plots—such as box plots for detecting distribution spread and scatter plots for relationship mapping—analysts can gain a comprehensive view of the dataset’s health and trends. A critical component of data analysis used to transform complex datasets into visual representations like charts and graphs to uncover patterns, trends, and correlations.

Dataset Creation:

np.random.seed(0) df = pd.DataFrame({ 'Category': ['A', 'B', 'C', 'D', 'E'], 'Values': [0, 70, 30, 90, 60], 'Sales': np.random.randint(100, 500, 5), 'Profit': np.random.randint(10, 100, 5) })

np.random.seed(0): Sets the random seed to 0, ensuring that every run of the notebook produces the same random values. This makes the experiment reproducible — a requirement for academic and scientific work.
np.random.randint(100, 500, 5): Generates 5 random integers in the range [100, 500), used as the Sales column.
np.random.randint(10, 100, 5): Generates 5 random integers in the range [10, 100), used as the Profit column.
The Category column acts as a categorical x-axis label, and Values is a manually assigned numerical column used primarily for area fill charts and proportional (pie/donut) charts.

Commands:

import seaborn as sns: Imports the Seaborn library, which is built on top of Matplotlib and used for creating attractive and informative statistical graphics.

import matplotlib.pyplot as plt: Imports the Matplotlib sub-module used for generating static, interactive, and animated visualizations in Python.

pd.read_csv(): Loads data from a comma-separated values (CSV) file into a structured DataFrame.

df.head(): Displays the first five rows of the DataFrame to provide a quick glimpse of the data structure and values.

df.info(): Prints a concise summary of the DataFrame, including the number of non-null entries and the data type of each column.

df.describe(): Generates descriptive statistics that summarize the central tendency, dispersion, and shape of a dataset’s distribution.

df.isnull().sum(): Checks for missing values across the dataset and returns the total count of null entries for each column.

df.drop(): Removes specified labels (rows or columns) from the DataFrame to clean or simplify the dataset.

sns.histplot(): Plots a univariate histogram to visualize the distribution of a single numerical variable.

sns.scatterplot(): Draws a scatter plot to represent the relationship between two numerical variables using dots.

plt.figure(figsize=...): Specifies the width and height of the plotting area in inches to ensure the chart is readable.

plt.title(): Adds a descriptive title to the top of the visualization for better context.

plt.gcf(): Returns the current active Figure object.

fig.gca(): Returns the current active Axes within the figure.

axes.add_artist(artist): Adds a drawable artist object directly to the axes.

sns.boxplot(x= or y=): Renders a box-and-whisker plot with automatic quartile computation and outlier detection.

df.corr(): Computes the Pearson correlation coefficient matrix.

sns.heatmap(data, annot, cmap): Renders a color-encoded matrix heatmap with optional cell annotations and colormap.

s= in plt.scatter(): Controls marker size per data point (bubble encoding).

size=, sizes=, hue= in sns.scatterplot(): Seaborn parameters for bubble size and color encoding.

plt.show(): Displays the created plots and clears the current figure buffer.



## Conclusion:
Through this experiment, it is concluded that Exploratory Data Analysis (EDA) is an indispensable step in the data pipeline. By using functions for statistical description and visual plotting, we can effectively identify data quality issues like missing values and outliers, while simultaneously discovering meaningful correlations between variables that guide further analysis.
