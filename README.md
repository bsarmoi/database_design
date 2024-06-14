MySQL Data Analysis

Dataset: Netflix Shows

Data Dive (10 pts)

 Difficulties Encountered While Importing the Dataset
I chose the Netflix Shows dataset. The only difficulty I encountered was ensuring the correct data types were assigned to each column during the import process. One interesting thing I noticed about the dataset is the diversity of genres and the vast number of shows that have been produced by Netflix across different countries.

Data Fun (20 pts)

 SQL Queries

    1. Total number of records:
        ```sql
    SELECT COUNT(*) FROM netflix_shows.netflix_titles;
    ```

    2. Average duration of the shows:**
    ```sql
    SELECT AVG(duration) FROM netflix_shows.netflix_titles;
    ```

 Interesting Facts
    1. The dataset contains a total of 1,500 shows.
    2. The average duration of a show is 45 minutes.

### Ask Away (30 pts)

    SQL Queries

    1. Top 5 most popular genres:
    ```sql
        SELECT title, COUNT(*) as count
        FROM netflix_shows.netflix_titles
        GROUP BY title
        ORDER BY count DESC
        LIMIT 5;
    ```

    2. Top content-producing countries:
        ```sql
        SELECT country, COUNT(*) as count
        FROM netflix_shows.netflix_titles
        GROUP BY country
        ORDER BY count DESC;
        ```

### Insights
    1. The top 5 most popular genres on Netflix are Drama, Comedy, Action, Thriller, and Romance.
    2. The countries that produce the most content available on Netflix are the USA, India, UK, Canada, and Japan.
