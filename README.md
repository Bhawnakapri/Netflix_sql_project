# Netflix Movies and TV Shows Data Analysis using SQL

![](https://github.com/najirh/netflix_sql_project/blob/main/logo.png)

# Project Overview
This project involves exploratory data analysis of Netflix Movies and TV Shows using PostgreSQL. The objective is to solve real-world business questions and extract meaningful insights from structured entertainment data using advanced SQL techniques.
The project demonstrates strong command over data querying, transformation, aggregation, and analytical problem-solving using SQL.

# Business Objectives
-Analyze the distribution of Movies vs TV Shows
-Identify the most common content ratings by type
-Examine content trends across years and countries
-Identify top-performing actors and directors
-Analyze genre distribution
-Categorize content based on keyword-based sentiment logic
-Extract time-based insights using date operations

# Tech Stack
-PostgreSQL
-pgAdmin 4
-SQL
-Visual Studio Code

# Dataset
Source:  [Movies Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows?resource=download)
-Records: ~8,800+ titles
-Attributes: 12 columns including content type, director, cast, country, rating, release year, duration, genre, and description.

## Schema

'''sql
DROP TABLE IF EXISTS netflix;
CREATE TABLE netflix
(
    show_id      VARCHAR(5),
    type         VARCHAR(10),
    title        VARCHAR(250),
    director     VARCHAR(550),
    casts        VARCHAR(1050),
    country      VARCHAR(550),
    date_added   VARCHAR(55),
    release_year INT,
    rating       VARCHAR(15),
    duration     VARCHAR(15),
    listed_in    VARCHAR(250),
    description  VARCHAR(550)
);
'''

# Key Analytical Problems Solved

-✔ Counted total Movies vs TV Shows
-✔ Identified most frequent ratings using window functions
-✔ Extracted top 5 content-producing countries
-✔ Determined the longest movie using string parsing & casting
-✔ Analyzed content added in the last 5 years
-✔ Identified actors with highest appearances in Indian productions
-✔ Categorized content using conditional keyword logic
-✔ Calculated year-wise contribution percentage for Indian content

# SQL Concepts Demonstrated
Aggregate Functions (COUNT, ROUND)
Grouping & Sorting (GROUP BY, ORDER BY)
Window Functions (RANK() OVER)
Common Table Expressions (CTE)
String Functions (STRING_TO_ARRAY, UNNEST, SPLIT_PART)
Type Casting
Date Functions (TO_DATE, INTERVAL)
Conditional Logic (CASE WHEN)
Filtering (ILIKE, LIKE, WHERE)

# Business Insights
Movies dominate the Netflix catalog compared to TV Shows.
A small set of ratings account for a majority of content.
The United States and India contribute significantly to the platform’s library.
Content growth accelerated in specific peak years.
Keyword-based classification helps identify potentially sensitive content.

# Key Learning Outcomes
Applied SQL to solve structured business problems
Worked with semi-structured string fields (multiple countries, multiple actors)
Used analytical functions for ranking-based insights
Performed data transformation within PostgreSQL
Improved query optimization and logical structuring

# Conclusion
This project showcases practical SQL skills applied to a real-world dataset. It reflects the ability to translate business questions into efficient database queries and extract actionable insights — a core requirement for Data Analyst roles.

# Author

Bhawana Kapri
B.Tech CSE – Data Science
