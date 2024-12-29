### **Day 1: The Foundations of SQL – "Building the Base"**
**Theme:** Lay a rock-solid foundation by understanding SQL basics and best practices.

#### **Beginner Track: Essential Concepts**
- **Core Topics:**
  - Introduction to SQL and Relational Databases.
  - Basic Query Structure: SELECT, FROM, WHERE, ORDER BY.
  - Filtering Data: Comparison operators and logical conditions.
- **Hands-On Exercise:**
  - Use a `users` table (5,000 rows) to filter and sort based on conditions like `age > 30 AND country = 'USA'`.
- **Code Style:** Introduce SQL formatting and commenting conventions.

#### **Intermediate Track: Enhancing Queries**
- **Core Topics:**
  - Handling NULLs: IS NULL, COALESCE, and NULL-safe comparisons.
  - Introduction to aliases for readability.
- **Exercise:** Identify incomplete data in a `sales` table and use COALESCE to fill missing values.

#### **Advanced Track: Query Optimization**
- **Core Topics:**
  - Query Execution Plans: Reading and interpreting.
  - Basics of indexing and when to use them.
- **Exercise:**
  - Analyze a poorly performing query on a 1M-row `transactions` table. Optimize it using execution plans and indexing.

---

### **SQL Bootcamp: Top 1% Edition – Day 1 (Revised)**  
*Incorporating a deeper dive, advanced topics integration, practical data challenges, and collaborative learning.*  

---

### **Day 1: The Foundations of SQL – "Building the Base"**  
**Theme:** Establish the fundamentals while challenging participants to think critically and interactively, even from Day 1.

---

### **Beginner Track: Essential SQL Concepts**  

#### **Core Topics**  
1. **What is SQL and Why It Matters**  
   - Introduction to relational databases and SQL’s role.  
   - Simple analogy: SQL as the “language of conversations” with your database.  

2. **Core Query Structure**  
   - **SELECT**: Columns to retrieve.  
   - **FROM**: Tables to query.  
   - **WHERE**: Filtering criteria.  
   - **ORDER BY**: Sorting results.  

3. **Basic Aggregations**  
   - Use of `COUNT`, `MIN`, `MAX`, and `AVG` in simple queries.  

#### **Example Dataset:** `users` table (5,000 rows)  
| user_id | name      | age | country      | signup_date | purchases |  
|---------|-----------|-----|--------------|-------------|-----------|  
| 1       | Alice     | 25  | USA          | 2023-01-01  | 5         |  
| 2       | Bob       | 30  | UK           | 2023-02-15  | 3         |  
| 3       | Charlie   | 35  | USA          | 2023-03-01  | 8         |  
| 4       | Diana     | 28  | Australia    | 2023-04-10  | 0         |  

#### **Interactive Exercise 1**:  
1. Find all users aged 30 or older.  
    ```sql
    SELECT name, age  
    FROM users  
    WHERE age >= 30;  
    ```
2. Find the total number of users.  
    ```sql
    SELECT COUNT(*) AS total_users  
    FROM users;  
    ```

#### **Hands-On Task:**  
- Write a query to calculate the **average purchases** for users in the USA.  

#### **Interactive Quiz** (Beginner Level):  
**Q:** If you want to sort users by their signup date, which clause should you use?  
- A) SELECT  
- B) ORDER BY  
- C) WHERE  
- D) GROUP BY  
*(Answer: B)*  

---

### **Intermediate Track: Enhancing Queries**  

#### **Core Topics**  
1. **Null Handling Techniques**  
   - Using `COALESCE` for default values.  
   - Introduction to `CASE WHEN` for conditional logic.  

2. **Aliases for Simplification**  
   - Table and column aliases for better readability.  

3. **Interactive Visualizations**  
   - Use sample query results to generate simple bar charts (e.g., total purchases by country).  

#### **Example Dataset:** `orders` table (10,000 rows)  
| order_id | user_id | order_amount | order_date  |  
|----------|---------|--------------|-------------|  
| 1        | 1       | 100.50       | 2023-01-10  |  
| 2        | 2       | NULL         | 2023-02-20  |  
| 3        | 1       | 200.00       | 2023-03-05  |  
| 4        | 3       | 50.00        | 2023-04-12  |  

#### **Interactive Exercise 2:**  
1. Replace NULL order amounts with `0`.  
    ```sql
    SELECT order_id, COALESCE(order_amount, 0) AS adjusted_amount  
    FROM orders;  
    ```
2. Categorize orders as "High", "Medium", or "Low" based on the `order_amount`:  
    ```sql
    SELECT order_id,  
           CASE  
               WHEN order_amount >= 150 THEN 'High'  
               WHEN order_amount BETWEEN 50 AND 149 THEN 'Medium'  
               ELSE 'Low'  
           END AS order_category  
    FROM orders;  
    ```

#### **Hands-On Task:**  
- Combine the `users` and `orders` tables to calculate the **total spending per user**.  

#### **Interactive Quiz** (Intermediate Level):  
**Q:** What does `COALESCE(order_amount, 0)` do?  
- A) Replaces NULL values with 0.  
- B) Replaces all order amounts with 0.  
- C) Returns rows without NULL values.  
*(Answer: A)*  

---

### **Advanced Track: Query Optimization**  

#### **Core Topics**  
1. **Query Execution Plans**  
   - Understanding `EXPLAIN`: Identifying table scans, join types, and filter operations.  
   - Analyzing execution costs and optimization opportunities.  

2. **Indexing Basics**  
   - Importance of indexes for speeding up queries.  
   - Trade-offs of indexing small tables vs. large tables.  

#### **Example Dataset:** `transactions` table (1M rows)  
| transaction_id | user_id | amount  | transaction_date |  
|----------------|---------|---------|------------------|  
| 1              | 1       | 150.00 | 2023-01-10       |  
| ...            | ...     | ...     | ...              |  

#### **Interactive Exercise 3:**  
1. Analyze a slow query:  
    ```sql
    SELECT user_id, SUM(amount) AS total_spent  
    FROM transactions  
    WHERE transaction_date >= '2023-01-01'  
    GROUP BY user_id;  
    ```
2. Use `EXPLAIN` to identify performance issues.  

3. Optimize the query by adding an index:  
    ```sql
    CREATE INDEX idx_transaction_date ON transactions (transaction_date);  
    ```

#### **Hands-On Task:**  
- Optimize a multi-table join query with execution plan analysis and indexing.  

#### **Interactive Quiz** (Advanced Level):  
**Q:** What does an execution plan show?  
- A) Query result.  
- B) Steps the database takes to execute the query.  
- C) Table names.  
*(Answer: B)*  

---

### **New Enhancements for Day 1**

1. **Dynamic Visual Aids:**  
   - Use simple visual tools (like bar charts) to demonstrate query results.  

2. **Real-World Data Challenges:**  
   - Introduce slightly messy data with missing values to replicate real-world conditions.  

3. **Advanced Topics Teaser:**  
   - Brief introduction to transactions and ACID properties to spark curiosity.  

4. **Collaborative Learning:**  
   - Pair up learners to solve tasks together and review each other’s code.  

5. **Leaderboard:**  
   - Gamify the learning experience by awarding points for completing tasks.  

---

### **Day 1 Wrap-Up Challenges**  

#### **Beginner Task:**  
Write a query to find users with no purchases and sort them by signup date.  

#### **Intermediate Task:**  
Write a query that categorizes orders and calculates the total amount per category.  

#### **Advanced Task:**  
Analyze and optimize a slow query on the `transactions` table using an execution plan and indexing strategies.  

---

By the end of Day 1, learners will have a solid grasp of SQL basics, practical experience with real-world challenges, and a taste of advanced optimization techniques. Onward to **Joins and Relationships** in Day 2!  
