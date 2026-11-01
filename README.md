🎵 Music Store Data Analysis | PostgreSQL

Project Overview

An SQL-based analysis of a digital music store database to understand customer purchasing behaviour, sales performance, revenue distribution, and music preferences.

The project addresses 11 business questions using PostgreSQL, progressing from basic queries to advanced analytical techniques.

⸻

🛠️ Tools Used

* PostgreSQL
* pgAdmin 4
* SQL

📊 Database Schema

The database contains interconnected tables covering customers, employees, invoices, tracks, albums, artists, and genres.

⸻

🔍 Business Questions & Approach

1. Easy Level

Q1. Identify the senior-most employee.

→ Sort employee levels in descending order and retrieve the top record.

Q2. Which countries generate the most invoices?

→ Group invoices by country and calculate invoice counts.

Q3. What are the top three invoice values?

→ Sort invoice totals in descending order and retrieve the top three.

Q4. Which city generates the highest revenue?

→ Group invoices by billing city and calculate total revenue using SUM().

Q5. Who is the highest-spending customer?

→ Join customer and invoice tables and calculate total spending per customer.

2. Moderate Level

Q6. Identify customers who listen to Rock music.

→ Join customer, invoice, track, and genre-related tables and filter Rock music listeners.

Q7. Find the top 10 Rock music artists.

→ Join artist, album, track, and genre tables and rank artists by track count.

Q8. Identify tracks longer than average duration.

→ Use a subquery with AVG() to identify tracks exceeding average duration.

3. Advanced Level

Q9. Calculate customer spending on individual artists.

→ Use multiple joins and aggregation to calculate spending by customer and artist.

Q10. Find the most popular genre in each country.

→ Aggregate purchases by country and genre, then apply ranking techniques while accounting for ties.

Q11. Find the highest-spending customer in each country.

→ Calculate customer spending by country and use ranking techniques to identify top customers, including ties.

⸻

📈 Key Findings

Numerical findings from the analysis:

* Senior-most employee: To be added.
* Country with the most invoices: To be added.
* Top three invoice values: To be added.
* Highest-revenue city: To be added.
* Highest-spending customer: To be added.
* Top Rock music artist: To be added.
* Average track duration: To be added.
* Most popular genres by country: To be added.
* Highest-spending customers by country: To be added.

⸻

💡 Business Insights

The analysis helps identify opportunities for:

* Targeted marketing based on customer music preferences.
* Customer retention through identification of high-value customers.
* Geographical sales and promotional strategies.
* Artist and genre-based promotional campaigns.

⸻

💻 SQL Concepts Applied

SELECT · WHERE · DISTINCT · GROUP BY · ORDER BY · JOIN · COUNT() · SUM() · AVG() · Subqueries · Window Functions (where applicable).

⸻

📁 Project Structure

Music-Store-SQL-Analysis/
│
├── Music_Store_Query.sql
├── MusicDatabaseSchema.png
├── Music Store Analysis-Questions (1).pdf
├── music store data.zip
└── README.md

⸻

▶️ How to Run

1. Clone or download this repository.
2. Extract the database ZIP file.
3. Restore the database in PostgreSQL using pgAdmin 4.
4. Open Music_Store_Query.sql.
5. Execute the queries and explore the results.
