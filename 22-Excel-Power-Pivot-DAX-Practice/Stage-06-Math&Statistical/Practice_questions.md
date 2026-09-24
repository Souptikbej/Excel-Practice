# Stage 6 — Math & Statistical DAX Practice Questions

## Platform

**Excel Power Pivot**

## Dataset

`Sales_Performance_Analysis`

Use the following dataset exactly as provided.

| EmpID | Employee | Department | Sales | Target | Profit | Customers | Orders | Attendance% | Rating |
|---:|---|---|---:|---:|---:|---:|---:|---:|---:|
| 101 | Rahul | Sales | 120000 | 100000 | 18000 | 45 | 60 | 96 | 4 |
| 102 | Priya | Sales | 85000 | 100000 | 12000 | 32 | 48 | 91 | 3 |
| 103 | Amit | Finance | 95000 | 90000 | 15000 | 28 | 42 | 88 | 4 |
| 104 | Sneha | IT | 140000 | 120000 | 25000 | 52 | 70 | 97 | 5 |
| 105 | Vikas | Marketing | 75000 | 80000 | 9000 | 25 | 35 | 82 | 2 |
| 106 | Neha | Sales | 110000 | 100000 | 16000 | 40 | 55 | 94 | 4 |
| 107 | Anita | IT | 105000 | 120000 | 14000 | 38 | 50 | 90 | 3 |
| 108 | Raj | Finance | 125000 | 110000 | 22000 | 48 | 65 | 95 | 5 |
| 109 | Pooja | HR | 68000 | 70000 | 7000 | 22 | 30 | 86 | 3 |
| 110 | Rohit | Marketing | 92000 | 80000 | 13000 | 35 | 45 | 93 | 4 |
| 111 | Arjun | Sales | 155000 | 130000 | 28000 | 58 | 75 | 98 | 5 |
| 112 | Kavya | Finance | 78000 | 90000 | 10000 | 26 | 38 | 89 | 3 |
| 113 | Suman | IT | 130000 | 120000 | 21000 | 50 | 68 | 96 | 4 |
| 114 | Deepak | HR | 82000 | 70000 | 11000 | 30 | 40 | 92 | 4 |
| 115 | Meera | Marketing | 115000 | 100000 | 19000 | 44 | 58 | 95 | 5 |

---

# Part A — Basic Aggregation

### Q1. Total Sales

Calculate total company sales.

**Concept:** `SUM()`

---

### Q2. Average Sales

Calculate average sales per employee.

**Concept:** `AVERAGE()`

---

### Q3. Minimum Sales

Find the lowest sales value.

**Concept:** `MIN()`

---

### Q4. Maximum Sales

Find the highest sales value.

**Concept:** `MAX()`

---

# Part B — Counting

### Q5. Employee Count

Calculate the total number of employees.

**Concept:** `COUNTROWS()`

---

### Q6. Employees with Sales Data

Count how many numeric Sales values exist.

**Concept:** `COUNT()`

---

### Q7. Employees with Employee Names

Count how many non-blank Employee names exist.

**Concept:** `COUNTA()`

---

# Part C — Business Calculations

### Q8. Total Profit

Calculate total company profit.

**Concept:** `SUM()`

---

### Q9. Average Profit

Calculate average profit per employee.

**Concept:** `AVERAGE()`

---

### Q10. Overall Profit Margin %

Calculate:

```text
Total Profit / Total Sales × 100
```

**Concept:** `DIVIDE()`

---

### Q11. Average Sales per Order

Calculate:

```text
Total Sales / Total Orders
```

**Concept:** `DIVIDE()`

---

# Part D — Difference & Rounding

### Q12. Target Gap

Create a calculated column:

```text
Sales - Target
```

Positive = above target  
Negative = below target.

---

### Q13. Absolute Target Gap

Create a calculated column:

```text
ABS(Sales - Target)
```

The result must always be non-negative.

**Concept:** `ABS()`

---

### Q14. Rounded Profit Margin

Calculate Profit Margin and round the result to 2 decimal places.

**Concept:** `ROUND()`

---

# Part E — Median & Unique Analysis

### Q15. Median Sales

Calculate the median employee sales.

**Concept:** `MEDIAN()`

---

### Q16. Unique Departments

Find the number of unique departments.

**Concept:** `DISTINCTCOUNT()`

---

### Q17. Unique Employees

Find the number of unique employees.

**Concept:** `DISTINCTCOUNT()`

---

# Part F — Numerical Logic

### Q18. Sales Performance Category

Create a calculated column:

```text
Sales >= Target → "Above Target"
Sales < Target  → "Below Target"
```

**Concept:** `IF()`

---

### Q19. Profit per Customer

Calculate:

```text
Profit / Customers
```

**Concept:** `DIVIDE()`

This is a row-level calculation.

---

### Q20. Sales per Order

Calculate:

```text
Sales / Orders
```

**Concept:** `DIVIDE()`

This is a row-level calculation.

---

# Part G — Statistical Analysis

### Q21. Population Standard Deviation of Sales

Calculate the population standard deviation of Sales.

**Concept:** `STDEV.P()`

Business meaning:

> Measures how widely employee sales vary across the complete dataset.

---

### Q22. Sample Standard Deviation of Sales

Calculate the sample standard deviation of Sales.

**Concept:** `STDEV.S()`

Understand the difference between population and sample standard deviation.

---

### Q23. Population Variance of Sales

Calculate population variance of Sales.

**Concept:** `VAR.P()`

---

# Part H — Advanced Numerical Logic

### Q24. Sales Size Category

Create a calculated column using `SWITCH(TRUE())`.

| Sales | Category |
|---:|---|
| >= 130000 | Very High |
| >= 100000 | High |
| >= 80000 | Medium |
| < 80000 | Low |

**Important:** Condition order matters.

---

# Part I — Final Business Problem

### Q25. Overall Performance Score

Create a calculated column using `SWITCH(TRUE())`.

#### Excellent Performer

All conditions must be true:

```text
Sales >= Target
AND Profit >= 20000
AND Rating >= 4
AND Attendance% >= 95
```

Output:

```text
Excellent Performer
```

#### Good Performer

```text
Sales >= Target
AND Profit >= 15000
AND Rating >= 4
```

Output:

```text
Good Performer
```

#### Needs Attention

Any of these conditions:

```text
Sales < Target
OR Rating <= 2
OR Attendance% < 85
```

Output:

```text
Needs Attention
```

#### Otherwise

```text
Average Performer
```

### Required condition order

```text
Excellent Performer
Good Performer
Needs Attention
Average Performer
```

---

# Submission Checklist

Before submitting your answers:

- [ ] Q1–Q25 completed
- [ ] Correct Excel Power Pivot table
- [ ] Correct DAX syntax
- [ ] Correct function for each question
- [ ] Correct aggregation level
- [ ] Correct population/sample functions
- [ ] Correct `SWITCH(TRUE())` order
- [ ] Exact output labels checked

---

# Stage Completion

After completing all 25 questions, submit your DAX formulas for review.

The review will check every question individually and provide:

- Score out of 100
- Correct/incorrect status
- Formula corrections
- Business-logic corrections
- Final Stage 6 status
- Readiness for Stage 7 — Relationship DAX
