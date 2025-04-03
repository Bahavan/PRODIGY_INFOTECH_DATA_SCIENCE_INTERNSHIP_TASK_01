# PRODIGY_INFOTECH_DATA_SCIENCE_INTERNSHIP_TASK_01

# Task-01: Data Visualization (Bar Chart & Histogram)

## Task Description
Create a bar chart or histogram to visualize the distribution of a categorical or continuous variable, such as the distribution of ages or genders in a population.

## Dataset
For this task, you can use the sample dataset provided by the World Bank:
[World Bank Population Data](https://data.worldbank.org/indicator/SP.POP.TOTL)

## Instructions
1. Download or extract relevant population data from the World Bank dataset.
2. Use Python libraries like `matplotlib` and `seaborn` to create visualizations.
3. Choose either:
   - A **Bar Chart** (for categorical data like gender distribution).
   - A **Histogram** (for continuous data like age distribution).
4. Ensure the chart is labeled properly with a title, axis labels, and a legend if necessary.

## Requirements
- Python 3.x
- Libraries:
  - `pandas`
  - `matplotlib`
  - `seaborn`

## Example Code
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Sample data: Age distribution
ages = [10, 12, 14, 16, 18, 18, 20, 22, 25, 30, 30, 35, 40, 45, 50, 55, 60, 65]

# Create a histogram
plt.figure(figsize=(8,5))
sns.histplot(ages, bins=8, kde=True)
plt.xlabel('Age')
plt.ylabel('Count')
plt.title('Age Distribution in Population')
plt.show()
