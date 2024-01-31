# Movie Correlation Project


### Project Overview
This project aims to identify and understand the factors of success in the movie industry through data analysis. By analyzing the correlations between various variables, it seeks to provide useful insights for what variables effect the gross revenues from movies.

### Data Sources

Movie Industry Data (https://www.kaggle.com/datasets/danielgrijalvas/movies)

### Tools

- Python(Pandas, Seaborn, Matplotlib, Numpy)
- Jupyter

```python
import pandas as pd
import seaborn as sns
import numpy as np

import matplotlib
import matplotlib.pyplot as plt
plt.style.use('ggplot')
from matplotlib.pyplot import figure

%matplotlib inline
matplotlib.rcParams['figure.figsize']=(12,8)
```

### Data Cleaning/Preparation

- Handling missing values and correcting data types in the dataset.

### Data Analysis

[Python Code- Click!](https://github.com/MingyuTheAnalyst/Movie-Correlation-Project/blob/main/Movie%20Correlation%20Project.ipynb)

- Data Display: Repeated use of df.head() for inspecting the data frame after each manipulation.

- Year Correction: A new column yearcorrect is created by extracting the year from the released column.

- Sorting Data: The data frame is sorted by the gross column in descending order.

- Handling Duplicates: There's a line of code for dropping duplicates in the company column, although it's not clear if this is applied to the entire dataset or just an exploration of the unique companies.

- Correlation Notes: There are brief notes on high correlation between budget and gross earnings, and between the company and some other variable (not specified).

- Scatter Plot Visualization: A scatter plot is created to visualize the relationship between the film's budget and its gross earnings.

### Data Visualization
Included some of visualization

```python
sns.regplot(x='budget', y='gross', data=df, scatter_kws={"color":"red"}, line_kws={"color":"blue"})
```
<img width="600" alt="Screenshot 2024-01-30 at 10 21 19 PM" src="https://github.com/MingyuTheAnalyst/Movie-Correlation-Project/assets/88122148/8254ff84-b8be-463e-ab14-fc5d1493cd38">

```python
correlation_matrix = df_numerized.corr(method='pearson', numeric_only=True)

sns.heatmap(correlation_matrix, annot=True)

plt.title('Correlation Matric for Numeric Features')

plt.xlabel('Movie Features')

plt.ylabel('Movie Features')

plt.show()
```
<img width="805" alt="Screenshot 2024-01-30 at 10 23 13 PM" src="https://github.com/MingyuTheAnalyst/Movie-Correlation-Project/assets/88122148/2425b438-4356-471c-83a0-454db806f764">



### Results/Findings

- The analysis showed that there's a strong link between how much a movie earns (its Gross) and how much money was spent to make it (its Budget). In simple terms, movies with bigger budgets often make more money. Also, the number of Votes a movie gets, which shows how much people are interested in it, is another key factor that affects how much money a movie makes.

### Limitations

- A key limitation of this analysis is that it mainly focuses on quantitative factors like Budget and Votes, potentially overlooking other important elements that contribute to a movie's success, such as film quality, cast and crew reputation, or marketing strategies. Additionally, the correlation does not imply causation, so while there's a link between budget and earnings, it doesn't necessarily mean a higher budget directly causes higher earnings.
