# SECTION-D-Payments-Order-Status
Practical SQL project for analyzing e-commerce orders and payments using JOINs, GROUP BY, and real-world business logic.
## ## SECTION D: Payments & Order Status

This section focuses on analyzing **order payments and payment status**
using SQL. It represents real-world e-commerce payment scenarios such as
**fully paid orders, partially paid orders, unpaid orders, and multiple
payment transactions**.

The queries demonstrate how payment data can be aggregated and compared
with order values to understand **order completion and financial status**.

---

### 📌 Queries Covered

#### 1️⃣ Display all orders along with their payment status (Paid / Not Paid)

Displays every order and determines whether it is **Paid** or **Not Paid**
based on the presence and total value of associated payment records.

**Concepts used:**

* LEFT JOIN
* Payment status classification
* Handling missing payments using `IS NULL` / `IFNULL`
* Conditional logic

---

#### 2️⃣ Find orders where payment amount is less than order total

Identifies **partially paid or unpaid orders** by comparing the total order
value (calculated from order items) with the total amount paid.

**Concepts used:**

* Multi-table JOINs
* Aggregate functions (`SUM`)
* `GROUP BY` and `HAVING`
* Payment reconciliation logic

---

#### 3️⃣ Identify orders that have multiple payments

Finds orders that were paid using **more than one payment transaction**,
which is common in split payments or installment-based payment flows.

**Concepts used:**

* Aggregation with `COUNT`
* `GROUP BY` and `HAVING`
* Transaction-level payment analysis

---

#### 4️⃣ Calculate total amount paid for each order

Calculates the **total amount paid per order** by summing all related payment
records, including orders that have no payments.

**Concepts used:**

* LEFT JOIN
* `SUM()` aggregation
* Order-wise financial summary
* Handling unpaid orders

---

#### 5️⃣ Find Delivered orders that are not paid yet

Identifies orders that are marked as **Delivered** but have **no payment
records**, highlighting potential payment or data consistency issues.

**Concepts used:**

* LEFT JOIN
* `IS NULL` condition
* Order status filtering
* Real-world exception handling

---

### 🎯 Learning Outcomes

* Understand real-world **payment and order status logic**
* Gain confidence in **aggregate queries and HAVING conditions**
* Learn how to handle **NULL values and missing relationships**
* Apply SQL concepts to **e-commerce financial analysis**

---
This project was independently designed, developed, and implemented by me as part of hands-on SQL learning and practice.

All database schemas, queries, logic, and analysis were created and written by me to demonstrate practical understanding of SQL concepts including JOINs, aggregations, and data analysis.

Authored & Created By:
Sundar V

Technology Used:
SQL (MySQL)

