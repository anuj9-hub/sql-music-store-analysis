# SQL Music Store Analysis

## 📌 Project Overview
This project demonstrates **end-to-end ad-hoc data analysis using SQL** on a relational music store database.  
The objective is to answer **real-world business questions** related to sales performance, customer behavior, artist popularity, genre trends, and geographical insights.

The project progresses from **basic SQL queries** to **advanced analytical techniques**, reflecting how SQL is used in real data analyst roles.

---

## 🗂️ Dataset Description
The dataset represents a digital music store and contains multiple interrelated tables:

- **Customer** – customer details and demographics  
- **Invoice** – transaction-level sales data  
- **Invoice_Line** – item-level purchase details  
- **Track** – song metadata  
- **Album** – album information  
- **Artist** – artist details  
- **Genre** – music genre classification  
- **Employee** – organizational hierarchy  

The database follows a **normalized relational schema**, enabling complex joins and analytical queries.

---

## 🎯 Business Objectives
The analysis answers key business questions such as:
- Who are the **highest-spending customers**?
- Which **cities and countries generate the most revenue**?
- What are the **most popular music genres by country**?
- Which **artists contribute the most to total sales**?
- How does **customer spending vary geographically**?

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
- Multi-table joins across multiple entities
- Relationship-based querying using primary and foreign keys

### Subqueries
- Nested subqueries
- Scalar subqueries
- Subqueries for comparison with aggregate values

### Common Table Expressions (CTEs)
- Non-recursive CTEs using `WITH`
- Query modularization for readability and reusability

### Recursive CTEs
- Recursive queries to handle **top-N per group** problems
- Tie-handling scenarios across countries and customers

### Window Functions
- `ROW_NUMBER()`
- `PARTITION BY`
- Ranking and segmentation within groups

### Business Logic
- Revenue calculation using `unit_price × quantity`
- Handling shared maximum values
- Country-level and customer-level aggregations

---

## 📊 Analysis Highlights

### Easy-Level Analysis
- Identified the **senior-most employee** based on job hierarchy  
- Found **countries with the highest number of invoices**  
- Retrieved **top invoice values**  
- Determined the **best-performing city** by total revenue  
- Identified the **highest-spending customer**

### Moderate-Level Analysis
- Identified **Rock music listeners** using multi-table joins  
- Determined **top 10 Rock artists** based on track count  
- Retrieved tracks **longer than the average song length**

### Advanced-Level Analysis
- Calculated **customer-wise spending on the top-selling artist**  
- Identified the **most popular music genre for each country** using:
  - Window functions
  - Recursive CTEs  
- Determined the **top-spending customer in each country**, including tie cases

---

## 📈 Key Insights
- Revenue is concentrated among a small segment of high-value customers  
- Music preferences differ significantly across countries  
- Certain genres dominate specific geographical markets  
- Advanced SQL techniques are critical for multi-dimensional analysis  

---

## 📌 Learning Outcomes
Through this project, I strengthened my ability to:
- Perform **ad-hoc SQL analysis** on relational databases  
- Write **clean, readable, and scalable SQL queries**  
- Apply **CTEs, recursive queries, and window functions**  
- Translate business questions into **data-driven insights**

---


