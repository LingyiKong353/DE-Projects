# Data-Modeling-with-Cassandra

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app. I will create an Apache Cassandra database which can create queries on song play data to answer the questions by creating a database for this analysis and testing the database by running queries given by the analytics team from Sparkify to create the results.

## Files:

- **Data-Modeling-with-Cassandra.ipynb**: The code file.

## Project Steps

1. **Modeling NoSQL database or Apache Cassandra database**
   - Design tables to answer the exact queries.
   - Write Apache Cassandra `CREATE KEYSPACE` and `SET KEYSPACE` statements.
   - Develop the `CREATE` statement for each of the tables to address each question.
   - Load the data with `INSERT` statements for each of the tables.
   - Test by running the proper `SELECT` statements with the correct `WHERE` clause.

2. **Build ETL Pipeline**
   - Implement the logic to iterate through each event file in `event_data` to process and create a new CSV file in Python.
   - Include Apache Cassandra `CREATE` and `INSERT` statements to load processed records into relevant tables in the data model.
   - Test by running `SELECT` statements after running the queries on the database.

## Queries:

1. Give me the artist, song title, and song's length in the music app history that was heard during `sessionId = 338` and `itemInSession = 4`.

2. Give me only the following: name of the artist, song (sorted by `itemInSession`), and user (first and last name) for `userid = 10`, `sessionid = 182`.

3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'.
