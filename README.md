# 🎧 Spotify SQL Analytics & Query Optimization

> Advanced PostgreSQL project focused on business analytics, SQL optimization, and database performance engineering using real-world Spotify streaming data.

![Banner](https://github.com/parrithi/Spotify-Analytics/blob/main/Spotify.png)

---

# 🚀 Project Overview

This project analyzes Spotify's streaming dataset using PostgreSQL to answer business-driven questions while demonstrating advanced SQL techniques and query optimization strategies.

Unlike traditional SQL practice projects, this repository focuses on two equally important areas:

- Business Analytics
- Database Performance Optimization

The project explores streaming trends, artist performance, audience engagement, and audio characteristics while showcasing production-level SQL techniques such as Window Functions, CTEs, Indexing, and EXPLAIN ANALYZE.

---

# ✨ Highlights

✔ Advanced SQL

✔ PostgreSQL

✔ Window Functions

✔ CTEs

✔ Query Optimization

✔ Indexing

✔ Execution Plan Analysis

✔ Business Insights

✔ Performance Engineering

---

# 🛠 Tech Stack

| Technology | Purpose |
|------------|----------|
| PostgreSQL | Database |
| SQL | Data Analysis |
| EXPLAIN ANALYZE | Query Profiling |
| Indexes | Performance Optimization |
| Window Functions | Advanced Analytics |
| CTEs | Query Structuring |

---

# 📂 Dataset

Spotify Music Dataset

Contains information about

- Artists
- Albums
- Tracks
- Streams
- Likes
- Views
- Audio Features
- Platform Statistics

---

# 📊 Business Analysis

The project answers analytical questions including:

- Most streamed songs
- Most popular artists
- Top viewed albums
- Songs with highest engagement
- Danceability analysis
- Energy distribution
- YouTube vs Spotify comparison
- Audio feature exploration
- Album performance
- Artist ranking

---

# ⚡ Advanced SQL Concepts

- Window Functions

- Common Table Expressions (CTEs)

- Aggregate Functions

- CASE Statements

- Nested Queries

- Ranking Functions

- String Functions

- Filtering

- GROUP BY

- HAVING

- Performance Tuning

---

# ⚙ Query Optimization

One of the major objectives of this project was improving SQL query performance using PostgreSQL indexing.

The same query was executed before and after creating an index on the **artist** column.

This demonstrates how indexing drastically reduces execution time by avoiding expensive sequential scans.

---

## Before Optimization

**Execution Time**

12.401 ms

**Planning Time**

0.154 ms

![EXPLAIN Before Index](https://github.com/parrithi/Spotify-Analytics/blob/main/Query_Before_Index.png)

---

## Query Plan (Before)

![EXPLAIN Before Index](https://github.com/parrithi/Spotify-Analytics/blob/main/Analysis_Before_index.png)
![EXPLAIN Before Index](https://github.com/parrithi/Spotify-Analytics/blob/main/Graphical.png)

---

## Applying Index

```sql
CREATE INDEX artist_index
ON spotify(artist);
```

---

## After Optimization

Execution Time

0.151 ms

Planning Time

2.055 ms

![EXPLAIN After Index](https://github.com/parrithi/Spotify-Analytics/blob/main/Query_After_Index.png)

---

## Query Plan (After)

![EXPLAIN After Index](https://github.com/parrithi/Spotify-Analytics/blob/main/Analysis_Index.png)
![EXPLAIN After Index](https://github.com/parrithi/Spotify-Analytics/blob/main/Graphical_Index.png)


---

# 📈 Performance Comparison

| Metric | Before | After |
|---------|--------|-------|
| Execution Time | 12.401 ms | 0.151 ms |
| Query Scan | Sequential Scan | Bitmap Index Scan |
| Index Used | ❌ No | ✅ Yes |
| Performance | Slow | Optimized |

---

# 💡 Key Learning

Creating an index on a frequently filtered column reduced query execution time by approximately **98.8%**, replacing a costly Sequential Scan with a Bitmap Index Scan.

This demonstrates the practical importance of indexing in improving analytical query performance on larger datasets.

---

# 📁 Repository Structure

Spotify-SQL-Analytics/

├── README.md

├── spotify_dataset.csv

├── schema.sql

├── business_queries.sql

├── optimization.sql

├── assets/

│ ├── explain-before.png

│ ├── explain-after.png

│ ├── graph-before.png

│ ├── graph-after.png

│ └── spotify-banner.png

---

# 🎯 Skills Demonstrated

- PostgreSQL

- Advanced SQL

- Window Functions

- CTEs

- Query Optimization

- Indexing

- Execution Plan Analysis

- Performance Tuning

- Business Analytics

- Exploratory Data Analysis

- Data Interpretation

---

# ⭐ If you found this project useful, consider giving 
