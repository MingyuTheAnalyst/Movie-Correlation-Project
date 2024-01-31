# Movie Correlation Project


### Project Overview
This project aims to identify and understand the factors of success in the movie industry through data analysis. By analyzing the correlations between various variables, it seeks to provide useful insights for movie production and marketing strategies.


### Data Sources

Movie Industry Data (https://www.kaggle.com/datasets/danielgrijalvas/movies)

### Tools

- Python(Pandas, Seaborn, Matplotlib, Numpy)


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

<img width="600" alt="Screenshot 2024-01-30 at 10 21 19 PM" src="https://github.com/MingyuTheAnalyst/Movie-Correlation-Project/assets/88122148/8254ff84-b8be-463e-ab14-fc5d1493cd38">
<img width="600" alt="Screenshot 2024-01-30 at 10 21 28 PM" src="https://github.com/MingyuTheAnalyst/Movie-Correlation-Project/assets/88122148/64265896-dcb8-42a0-b0d9-624ab0f3bd7a">



### Results/Findings

- The analysis showed that there's a strong link between how much a movie earns (its Gross) and how much money was spent to make it (its Budget). In simple terms, movies with bigger budgets often make more money. Also, the number of Votes a movie gets, which shows how much people are interested in it, is another key factor that affects how much money a movie makes.

### Limitations

- A key limitation of this analysis is that it mainly focuses on quantitative factors like Budget and Votes, potentially overlooking other important elements that contribute to a movie's success, such as film quality, cast and crew reputation, or marketing strategies. Additionally, the correlation does not imply causation, so while there's a link between budget and earnings, it doesn't necessarily mean a higher budget directly causes higher earnings.
