# Movies-ETL
Created a data pipeline from movie datasets using Python, Pandas, Jupyter Notebook and PostgreSQL. Implemented (ETL) - Extract, Transform, Load - to complete
Within the scope of the Amazing Prime Hackathon, this project will create an automated pipeline that takes in new data, from Wikipedia data, Kaggle metadata and the MovieLens rating data. It then performs the appropriate transformations and loads the data into an existing PostgreSQL database.

For this analysis, we used the following breakdown:
1. write an ETL function to read three data files,
2. extract and transform the Wikipedia data,
3. extract and transform the Kaggle and rating data,
4. load the data to a PostgreSQL Movie Database.

## Resources
- Software: Python 3.7.10, Conda 4.10.1, Jupyter Notebook 6.3, PostgreSQL 13, pgAdmin 4

## Results

### Write an ETL function to read three data files
The function takes the Wikipedia JSON, the Kaggle metadata and MovieLens csv files and creates three separate DataFrames.

### Extract and Transform the Wikipedia data
We filtered out the TV shows, consolidated the redundant data, removed the duplicates and formatted the Wikipedia data.

### Extract and Transform the Kaggle and rating data
Again, we consolidated the redundant data, removed the duplicates, formatted and grouped the data.\
The Kaggle and rating data were then merged with the Wikipedia movies DataFrame.

### Load the data to a PostgreSQL Movie Database
<img width="568" alt="ETL" src="https://user-images.githubusercontent.com/82069038/121946579-14b6b600-cd23-11eb-84bc-69b972615846.png">

<img width="1324" alt="moviesdf" src="https://user-images.githubusercontent.com/82069038/121946621-213b0e80-cd23-11eb-9fc5-69e7bd31fd65.png">

## Summary
The ETL function created collects and cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings csv files). It transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the hackathon participants for their analysis.
