# Stage 6 — Math & Statistical DAX

## Overview

Stage 6 focuses on **Math & Statistical DAX in Excel Power Pivot**.

The goal is to move from basic calculations to practical numerical and statistical analysis used in real-world Data Analyst work.

**Platform:** Excel Power Pivot  
**Dataset:** `Sales_Performance_Analysis`  
**Practice Type:** Practical business problems using one consistent dataset

---

## Learning Objectives

By completing this stage, you will practice:

- Aggregation functions
- Counting functions
- Safe division
- Difference calculations
- Rounding
- Median and unique-value analysis
- Standard deviation
- Variance
- Numerical business logic
- `SWITCH(TRUE())`
- Business performance classification

---

## Functions Covered

### Aggregation

- `SUM()`
- `AVERAGE()`
- `MIN()`
- `MAX()`

### Counting

- `COUNT()`
- `COUNTA()`
- `COUNTROWS()`
- `DISTINCTCOUNT()`

### Mathematical

- `DIVIDE()`
- `ABS()`
- `ROUND()`
- `ROUNDUP()`
- `ROUNDDOWN()`
- `INT()`
- `MOD()`
- `SQRT()`

### Statistical

- `MEDIAN()`
- `STDEV.P()`
- `STDEV.S()`
- `VAR.P()`
- `VAR.S()`
- `PERCENTILE.INC()`

### Logical / Business Analysis

- `IF()`
- `SWITCH(TRUE())`

> `RANKX()` is introduced conceptually but full ranking practice is reserved for Stage 9 — Ranking DAX.

---

## Dataset

### Table Name

`Sales_Performance_Analysis`

### Columns

| Column | Description |
|---|---|
| EmpID | Employee ID |
| Employee | Employee name |
| Department | Employee department |
| Sales | Employee sales |
| Target | Sales target |
| Profit | Employee profit |
| Customers | Number of customers |
| Orders | Number of orders |
| Attendance% | Attendance percentage |
| Rating | Performance rating |

---

## Dataset Rules

Use the dataset exactly as provided in `Practice_questions.md`.

Do not change:

- Employee values
- Sales values
- Target values
- Profit values
- Customers
- Orders
- Attendance%
- Rating
- Column names

The purpose of using one consistent dataset is to make the exercises comparable and business-focused.

---

## Important Concepts

### COUNT vs COUNTA vs COUNTROWS

- `COUNT()` → counts numeric values
- `COUNTA()` → counts non-blank values
- `COUNTROWS()` → counts rows in a table

### DIVIDE()

Prefer `DIVIDE()` for safe division:

```DAX
DIVIDE(Numerator, Denominator, 0)
```

### ABS()

Returns the absolute value:

```DAX
ABS(Data[Sales] - Data[Target])
```

### Population vs Sample

`STDEV.P()` and `VAR.P()` are used when the dataset represents the complete population.

`STDEV.S()` and `VAR.S()` are used when the dataset represents a sample.

### SWITCH(TRUE())

Conditions are evaluated from top to bottom.

Therefore, condition order matters.

---

## Practice Structure

The 25 questions are divided into:

1. Basic Aggregation
2. Counting
3. Business Calculations
4. Difference & Rounding
5. Median & Unique Analysis
6. Numerical Logic
7. Statistical Analysis
8. Advanced Numerical Logic
9. Final Business Problem

---

## Completion Standard

To complete Stage 6 successfully:

- Solve all 25 questions.
- Use Excel Power Pivot.
- Follow the requested DAX function/concept.
- Keep the same dataset.
- Check calculated-column vs aggregated calculation requirements carefully.
- Pay attention to aggregation level.
- Verify `SWITCH(TRUE())` condition order.
- Use exact requested output labels.

---

## Stage 6 Result

**Final Score: 96/100**

### Corrections

Q19 and Q20 were conceptually correct as aggregate ratios but did not match the requested row-level calculations.

### Q19 — Profit per Customer

Required:

```DAX
Profit per Customer :=
DIVIDE(
    Data[Profit],
    Data[Customers],
    0
)
```

### Q20 — Sales per Order

Required:

```DAX
Sales per Order :=
DIVIDE(
    Data[Sales],
    Data[Orders],
    0
)
```

The key lesson is to distinguish between:

```DAX
SUM(Profit) / SUM(Customers)
```

and:

```DAX
Profit / Customers
```

The first is an overall aggregate ratio; the second is a row-level calculation.

---

## Stage 6 Status

**PASSED — 96/100**

Next stage:

**Stage 7 — Relationship DAX**

---

## Recommended GitHub Structure

```text
Stage_6_Math_Statistical_DAX/
├── README.md
├── Practice_questions.md
└── Sales_Performance_Analysis_DAX.xlsx
```

For GitHub, include the Excel workbook and the two Markdown files. Screenshots can be added separately to demonstrate selected calculations and results.
