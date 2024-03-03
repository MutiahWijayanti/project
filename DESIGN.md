# Overview
**Groovy KalBar** is a web-based application developed with Python, HTML, CSS, and JavaScript. The main modules used to develop **Groovy KalBar** is Flask (https://palletsprojects.com/p/flask/) and CS50 Library for Python (https://cs50.readthedocs.io/libraries/cs50/python/), while the database engine used in **Groovy KalBar** is SQLite (https://www.sqlite.org/index.html). 
The application is free for use and is available in: 

# Database Schema
The database is designed using sqlite>.schema

....CREATE TABLE IF NOT EXISTS 'user' ('id' INTEGER PRIMARY KEY NOT NULL, 'username' TEXT, 'hash' ....TEXT);
....CREATE TABLE IF NOT EXISTS 'aksi' ('id' INTEGER PRIMARY KEY NOT NULL, 'user_id' INTEGER, ....'nilai' INTEGER);

# Structure
All the assets and resources used in this application are located inside the static folder. Meanwhile, the templates keep all the HTML files that render results returned by app.py. The backbone of **Groovy KalBar** is in app.py, where records from the database are retrieved and modified, user inputs are processed, and results are rendered to the templates. helpers.py provides several functions to help with multi-level authentication and the adaptation of the famous CS50's apology from finance.
