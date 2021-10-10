# Movies - Extract, Transform, Load (ETL)

## Overview of Movies-ETL
The purpose of the Movies-ETL analysis was to implement an automated way to "extract" data from existing data files, "transform" the data by creating and implementing several functions to clean multiple columns of data, and "load" the data into a PostgresSQL database. Below are the steps of the data analysis procedure for this app:

  - An ETL function was created to read in three data files, i.e., Kaggle metadata and MovieLensratings CSV files as well as Wikipedia JSON data. 
  - The Wikipedia data was transformed in numerous ways, i.e., filtering data, streamlining columns through renaming and organizing them, refine the data by minimizing the     
    amount of null values in the dataset, parsing data using regular expressions to standardize formatting within columns where necessary
  - The Kaggle metadata was cleaned and merged with the Wikipedia data to create a new DataFrame, i.e., movies_df 
  - The MovieLens ratings counts were cleaned and merged with the movies_df to create a new DataFrame, i.e., movies_with_ratings_df
  - A Movie Database was created in PostgreSQL and the cleaned movies_df as well as the MovieLens ratings data were loaded into this SQL database as tables
  - Two queries were generated to ensure that the data had been loaded correctly into the SQL database
    

## Resources
- Data Sources: movies_metadata.csv, ratings.csv, wikipedia_movies.json
- Software: Python 3.7.10, Anaconda 1.7.2, Jupyter Notebook, Pandas, NumPy, SqlAlchemy, Psycopg2

