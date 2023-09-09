# Data Modeling With Postgres



## Introduction / Context

A startup has a new mustic streaming app called Sparkify. The company wants to analyze the data they've been collecting on songs and user activity on the app. Most importantly, the analytics team needs to understand which songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

The goal of this project is to create a Postgres database with tables designed to optimize queries on song play analysis.This will encompass creating a database schema and ETL pipeline for the analysis. 

## Schema Design / ETL Pipeline

The project is designed on a star schema. The fact table is the songplays table and the dimension tables are the users, songs, artists, and time tables.

The ETL pipeline is executed by implementing etl.py and consists of two primary functions, process_song_file and process_log_file. 

Connection to the Sparkify database must be established in order to extract the log_data and song_data, transform the data where necessary and then load the data into the fact and dimension tables.


