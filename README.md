# Movies - Extract, Transform, Load (ETL)

## Overview of Movies-ETL
The purpose of the Movies-ETL analysis was to implement a procedure to "extract" data from existing movie data files, "transform" the data through creating and implementing several functions, and "load" the data into a PostgreSQL database. Below are the steps of this ETL data analysis procedure:

  - An ETL function was created to read in three data files, i.e., Kaggle metadata and MovieLensratings CSV files as well as Wikipedia JSON data. 
  - The Wikipedia data was transformed in numerous ways, e.g., filtering data, streamlining columns through renaming and organizing them, refining the data by minimizing the amount of null values in the dataset, and parsing data using regular expressions to standardize formatting within columns where necessary
  - The Kaggle metadata was cleaned and merged with the Wikipedia data to create a new DataFrame, i.e., movies_df 
  - The MovieLens ratings counts were cleaned and merged with the movies_df to create a new DataFrame, i.e., movies_with_ratings_df
  - A Movie Database was created in PostgreSQL and the cleaned movies_df as well as the MovieLens ratings data were loaded into this SQL database as tables
  - Two queries were generated to ensure that the data had been loaded correctly into the SQL database
    

## Resources
- Data Sources: movies_metadata.csv, ratings.csv, wikipedia_movies.json
- Software: Python 3.7.10, Anaconda 1.7.2, Jupyter Notebook, Pandas, NumPy, SqlAlchemy, Psycopg2, PostgreSQL, pgAdmin4

