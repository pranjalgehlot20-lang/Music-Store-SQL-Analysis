Music Store Data Analysis | PostgreSQL

Project Overview

An SQL-based analysis of a digital music store database to understand customer purchasing behaviour, sales performance, geographical revenue distribution, and music preferences.

The project uses PostgreSQL to answer 11 business questions across three difficulty levels, translating raw transactional data into actionable business insights.

Business Objectives

* Identify high-value customers and revenue-generating locations.
* Understand customer purchasing behaviour.
* Identify popular music genres and artists.
* Analyze sales distribution across countries.
* Explore opportunities for targeted marketing and customer engagement.

Tools Used

* PostgreSQL
* pgAdmin 4
* SQL

Database Schema

The database contains interconnected tables covering customers, employees, invoices, tracks, albums, artists, and genres.

Business Questions & Analytical Approach

Easy

Business Question	Analytical Approach
Identify the senior-most employee.	Sorting employee levels in descending order.
Which countries generate the most invoices?	GROUP BY, COUNT(), and ORDER BY.
What are the top three invoice values?	Sorting invoice totals and LIMIT.
Which city generates the highest revenue?	GROUP BY billing city and SUM() on invoice totals.
Who is the highest-spending customer?	JOIN customer and invoice tables, followed by aggregation.

Moderate

Business Question	Analytical Approach
Identify customers who listen to Rock music.	Multiple JOIN operations, filtering by genre, and DISTINCT.
Find the top 10 Rock music artists.	JOIN artist, album, track, and genre tables; COUNT() and ranking.
Identify tracks longer than average duration.	AVG() with a subquery.

Advanced

Business Question	Analytical Approach
Calculate customer spending on individual artists.	Multiple JOINs and SUM() with customer and artist grouping.
Find the most popular genre in each country.	Aggregation by country and genre, followed by ranking and tie handling.
Find the highest-spending customer in each country.	Customer-level spending aggregation and ranking within countries, including ties.

Key Findings

Numerical findings to be finalized using the query outputs.

Metric	Result
Senior-most employee	To be confirmed
Country with highest invoice count	To be confirmed
Top three invoice values	To be confirmed
Highest-revenue city	To be confirmed
Highest-spending customer	To be confirmed
Top Rock music artist	To be confirmed
Average track duration	To be confirmed
Most popular genre by country	To be confirmed
Highest-spending customer by country	To be confirmed

Business Insights

The analysis helps identify opportunities to:

* Focus retention strategies on high-value customers.
* Target promotional campaigns towards high-revenue cities.
* Develop genre-based marketing strategies.
* Identify popular artists and customer music preferences.
* Understand geographical differences in purchasing behaviour.

SQL Concepts Applied

SELECT · WHERE · DISTINCT · GROUP BY · ORDER BY · JOIN · COUNT() · SUM() · AVG() · Subqueries · Window Functions (where applicable).

Project Structure

Music-Store-SQL-Analysis/
│
├── Music_Store_Query.sql
├── MusicDatabaseSchema.png
├── Music Store Analysis-Questions (1).pdf
├── music store data.zip
└── README.md

How to Run

1. Download or clone the repository.
2. Extract the database ZIP file.
3. Restore the database in PostgreSQL using pgAdmin 4.
4. Open Music_Store_Query.sql.
5. Execute the queries and explore the results.
