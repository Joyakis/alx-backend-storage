# Advanced MySQL: Backend Storage & Optimization

## 📌 Project Overview
This repository contains a collection of advanced SQL scripts developed during the ALX Backend Storage module. The project focuses on moving logic from the application layer to the database layer to improve data integrity, security, and performance.

## 🛠️ Key Technical Implementations

### 1. Data Integrity & Constraints
* **Unique Constraints:** Implemented strictly enforced unique requirements for user data to prevent duplication at the schema level.
* **Email Validation:** Created boolean logic to track and validate email updates.

### 2. Automation with Triggers & Stored Procedures
* **Automated Calculations:** Developed stored procedures (e.g., `ComputeAverageScoreForUser`) to perform complex arithmetic on the fly.
* **Business Logic Automation:** Used **Triggers** to automatically update related tables (like inventory/store levels) whenever an order is placed, ensuring real-time data consistency.

### 3. Performance Tuning (Indexing)
* **Optimization:** Implemented multi-column indexes (`index_name_score`) to significantly reduce query execution time on large datasets.
* **Search Efficiency:** Created prefix indexes to speed up string-based searches.

### 4. Complex Analytics
* **Weighted Averages:** Scripted custom logic to calculate weighted scores across different project categories—critical for accurate ranking systems.

## 📂 File Breakdown

| File | Feature | Description |
| :--- | :--- | :--- |
| `0-uniq_users.sql` | Table Creation | Implements `UNIQUE` and `NOT NULL` constraints. |
| `4-store.sql` | Triggers | Decreases quantity of an item after adding a new order. |
| `7-average_score.sql` | Stored Procedures | Computes and stores average scores for students. |
| `8-index_my_names.sql` | Indexing | Creates an index on the first letter of a name for search optimization. |
| `100-weighted_score.sql` | Advanced Analytics | Calculates a user's average weighted score. |

## 🚀 How to Run
Ensure you have a MySQL server installed.
```bash
cat <file_name>.sql | mysql -uroot -p <database_name>Advanced SQL
