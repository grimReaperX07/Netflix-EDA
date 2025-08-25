📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on a Netflix dataset using PostgreSQL.
The goal is to clean the data, structure it into relational tables, and run SQL queries to 
answer business questions about content distribution, genres, directors, durations, and trends.



📂 Dataset

The dataset used is the Netflix Titles Dataset (commonly available on Kaggle).
It contains information about TV shows and movies available on Netflix, including:

show_id → Unique identifier

type → Movie / TV Show

title → Name of the show/movie

director → Director(s)

cast → Actors involved

country → Country of production

date_added → Date when added to Netflix

release_year → Original release year

rating → Content rating (e.g., PG-13, TV-MA)

duration → Duration in minutes or number of seasons

listed_in → Genre(s)

description → Short summary




🛠 Data Cleaning & Transformation

The dataset was cleaned and normalized into relational tables:

netflix_cleaned → Core details about shows & movies

netflix_directors → Director mapping

netflix_country → Country mapping

netflix_listed_in → Genre mapping

Key Transformations

Converted date_added to DATE format.

Split director, country, and listed_in (genres) into separate mapping tables.

Cleaned duration column → extracted numeric values (minutes/seasons).

Removed leading/trailing whitespaces.




🔍 Key Business Questions & SQL Queries

1.Which country has the highest number of comedy movies?

2.For each year, which director has the maximum number of movies added to Netflix?

3.For each director, count of Movies vs TV Shows

4.What is the average duration of movies in each genre?

5.Find the list of directors who have created horror and comedy movies both.
Display director names along with number of comedy and horror movies directed by them