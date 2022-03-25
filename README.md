# Movies Extract - Transform - Load

## Overview of Project

In this project, I am working on an ETL Movies Analysis bu utilizing Python, VS Code, RegEx and SQL Databases .
Raw data exists in multiple places and forms. In order to perform any kind of data analysis, this data needs to be cleaned and structured. Data pipeline process ETL – Extract, Transform, and Load is a core concept in data engineering, ensuring that data is consistent, maintains its integrity, and nonetheless strives for automatization of data wrangling. Without a consistent and robust data structure, it’s nearly impossible to perform any meaningful analysis.
<p align="center">
<img height="200" src="https://user-images.githubusercontent.com/98676400/160135715-8dc613dc-08af-424d-ac2d-76ca457803be.png"
</p>
<p align="center">
<b>Extract - Transform - Load  </b> </p> 

### Purpose of Movies ETL :

The Amazing Prime, a video streaming company, decided to sponsor a Hackathon, where participants trying to predict which low budget movies being released will become popular. Participants of a Hackathon need a clean data in order to perform analyses for their algorithms. In order to provide organized and clean dataset, this project focuses on ETL<b> Extract, Transform and Load </b> process and includes the following:

1-Extracting data from two different sources.
    A source from Wikipedia in <code>Json</code> format for all movies released since 1990
    A csv file  from Kaggle website for rating data.

2-Transforming data with Python, Pandas and Python RegEx module.

3-Loading data using PostgreSQL and pgAdmin.


## Analysis

My goal is to create an automated pipeline that extracts, transform and loads data. In order to reach my goal, I have breakdown the analysis in four major steps as follow:

1- Function Test :

* WikiMovies.json and MetaData.csv captured from website.
* MetaData is transformed into Pandas data frames.
* JSON file :
   * Loading file 
   * Transforming into data frame.

2- Function for cleaning WikiMovies data:

This function combines data of alternative languages into a new column alt_titles then help me to reduce number of columns in the dataset. 

The functions contains following methods :
    Python list comprehensions.
    <code>apply() and map() </code> methods in combination with lambda functions.
    <code>Regex</code> Regular expressions

3-Function for cleaning MetaData:

This function helps me to clean the data by applying following methods:
* Reestablish data-types by <code> pd.to_numeric, astype() </code> and  comparison operators for Boolean types.
* Find missing/unknown values and fill with correspond data and drop extra columns.
* Lastly merging data frames using <code> pd_merge</code> method.

4- Function -> Loading 
    
* In this final step, the function connects to the database by Sqlalchemy library and <code>to_sql method.</code>




