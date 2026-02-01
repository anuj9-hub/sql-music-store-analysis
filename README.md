# SQL Music Store Analysis

## 📌 Project Overview
This project demonstrates **end-to-end ad-hoc data analysis using SQL** on a relational music store database.  
The objective is to answer **real-world business questions** related to sales performance, customer behavior, artist popularity, genre trends, and geographical insights.

The analysis progresses from **basic SQL queries** to **advanced analytical techniques**, reflecting how SQL is used in real-world data analyst roles.

---

## 🗂️ Dataset Description
The dataset represents a digital music store and consists of multiple interrelated tables, including:

- **Customer** – customer details and demographics  
- **Invoice** – transaction-level sales data  
- **InvoiceLine** – item-level purchase details  
- **Track** – song-level metadata  
- **Album** – album information  
- **Artist** – artist details  
- **Genre** – music genre classification  
- **MediaType** – track format details  
- **Playlist / PlaylistTrack** – playlist mapping  
- **Employee** – organizational hierarchy  

The database follows a **normalized relational schema**, enabling efficient storage and complex analytical queries.

---

## 🧩 Database Schema

![Music Store Database Schema]("E:\SQL\MusicDatabaseSchema.png")

The above Entity Relationship Diagram (ERD) illustrates how transactional tables such as **Invoice** and **InvoiceLine**
are connected to descriptive dimension tables like **Customer**, **Track**, **Artist**, and **Genre**.
This structure enables multi-table joins and advanced analytical queries used throughout the project.

### Schema Highlights
- Fully **normalized relational design** to minimize redundancy  
- **Invoice** and **InvoiceLine** act as transactional (fact-like) tables  
- **Customer, Track, Artist, Genre** act as descriptive (dimension-like) tables  
- Foreign key relationships enable complex joins and aggregations  

---

## 🎯 Business Objectives
The analysis answers key business questions such as:
- Who are the **highest-spending customers**?
- Which **cities and countries generate the most revenue**?
- What are the **most popular music genres by country**?
- Which **artists contribute the most to overall sales**?
- How does **customer spending behavior vary geographically**?

---

## 🛠️ Tools & Technologies
- **SQL**
- Relational Database (PostgreSQL / MySQL compatible)
- GitHub for version control and documentation

---

## 🧠 SQL Skills & Concepts Used

### Core SQL
- `SELECT`, `WHERE`, `ORDER BY`
- `GROUP BY`, `HAVING`
- Aggregate functions: `SUM`, `COUNT`, `AVG`
- `LIMIT`

### Joins
- `INNER JOIN`
- Multi-table joins across 5+ tables
- Relationship-based querying using primary and foreign keys

### Subqueries
- Nested subqueries
- Scalar subqueries
- Subqueries for comparisons with aggregated values

### Common Table Expressions (CTEs)
- Non-recursive CTEs using `WITH`
- Query modularization for readability and maintainability

### Recursive CTEs
- Recursive queries to solve **top-N per group** problems
- Handling tie scenarios across countries and customers

### Window Functions
- `ROW_NUMBER()`
- `PARTITION BY`
- Ranking and segmentation within groups

### Business Logic
- Revenue calculation using `unit_price × quantity`
- Country-wise and customer-wise aggregations
- Handling shared maximum values in analytical results

---

## 📊 Analysis Highlights

### Easy-Level Analysis
- Identified the **senior-most employee** based on job hierarchy  
- Found **countries with the highest number of invoices**  
- Retrieved **top invoice values**  
- Determined the **best-performing city** based on total revenue  
- Identified the **highest-spending customer**

### Moderate-Level Analysis
- Identified **Rock music listeners** using multi-table joins and subqueries  
- Determined the **top 10 Rock artists** based on track count  
- Retrieved tracks **longer than the average song duration**

### Advanced-Level Analysis
- Calculated **customer-wise spending on the top-selling artist**  
- Identified the **most popular music genre for each country** using:
  - Window functions
  - Recursive CTEs  
- Determined the **top-spending customer per country**, including tie-handling scenarios

---

## 📈 Key Insights
- Revenue is concentrated among a small group of high-value customers  
- Music preferences vary significantly across different countries  
- Certain genres dominate specific geographical markets  
- Advanced SQL techniques are essential for multi-dimensional business analysis  

---

## 📌 Learning Outcomes
Through this project, I strengthened my ability to:
- Perform **ad-hoc SQL analysis** on relational databases  
- Write **clean, readable, and scalable SQL queries**  
- Apply **CTEs, recursive queries, and window functions**  
- Translate business questions into **actionable data-driven insights**

---

