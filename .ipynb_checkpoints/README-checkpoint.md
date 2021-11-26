# Purpose of the Sparkify

Information is a key to make important business decisions. This information should be available in real time and in different contexts. The data a company especially a startup holds about its customers and their usage patterns is vital to build this information. By having a database, the information can be built using various reporting tools and in near real time. A startup is dynamic and course corrections and strategy changes happen on a daily basis and the decisions a startup take can decide its fate. These decisions are as good as their information and information is a good as the data they have.

# Justification of Database schema design and ETL pipeline

The schema is designed to have meaningful information in different tables. These tables can be joined to provide important insights about the customer usage patterns and analysis. An ETL pipeline is necessary to convert raw log data into relational tables where these can be easily stored and analyzed. The star schema optimized fact and dimension tables allow for an intuitive view of the listening patterns.

# Example queries and results for song play analysis.

A simple analysis like this can help Spotify find which gender listens more to their songs

SELECT gender, count(*) FROM users GROUP BY gender;

# how to run the Python scripts

 1. Go To Tabs>Launcher
 2. From Launcher Dashboard open Terminal and run>python create_tables.py.
 3. To Load data into tables from logs run > python etl.py from terminal.

# An explanation of the files in the repository.

## create_tables.py
Main python program that creates the postgress database and calls the ETL functions and SQL queries.

## etl.ipynb
A jupyter notebook that helps to build the process for ETL.

## etl.py
Main etl program that identified files of songs and logs and loads the data into tables.

## sql_queries.py
Creates postgress database tables for creating tables,inserting data and searching data.

## test.ipynb
Test script to verify whether data has loaded correctly.
