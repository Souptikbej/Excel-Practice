# Stage 5 — Date & Time DAX Practice

## Overview

Stage 5 focuses on **Date & Time DAX in Excel Power Pivot**.

The objective is to learn how to use dates for practical business analysis rather than only memorizing functions.

This stage uses **one consistent business dataset** throughout all 25 questions.

## Platform

**Excel Power Pivot**

> This practice is specifically designed for DAX in Excel Power Pivot, not Power BI.

---

## Dataset

**Dataset name:** `Sales_Order_Date_Practice`

The dataset represents customer orders and contains:

| Column | Description |
|---|---|
| OrderID | Unique order identifier |
| OrderDate | Date when the order was placed |
| Customer | Customer name |
| Region | Sales region |
| Product | Product ordered |
| Quantity | Number of units ordered |
| Sales | Sales amount |
| DeliveryDate | Date when the order was delivered |
| PaymentDate | Date when payment was received |

---

## Date & Time Topics Covered

### Basic Date Extraction
- `YEAR()`
- `MONTH()`
- `DAY()`

### Week Analysis
- `WEEKDAY()`
- `WEEKNUM()`

### Date Construction
- `DATE()`

### Current Date & Time
- `TODAY()`
- `NOW()`

### Date Difference
- `DATEDIFF()`

### Date Shifting
- `EOMONTH()`
- `EDATE()`

### Date Formatting
- `FORMAT()`

### Business Date Logic
- `IF()`
- `SWITCH(TRUE())`
- Date-based conditions
- Delivery performance
- Payment performance
- SLA status
- Order aging

---

## Learning Objectives

By completing this stage, you should be able to:

1. Extract year, month, and day from a date.
2. Identify weekday and week number.
3. Construct a date using `DATE()`.
4. Understand the difference between `TODAY()` and `NOW()`.
5. Calculate the number of days between two dates.
6. Calculate delivery and payment durations.
7. Create month-end dates using `EOMONTH()`.
8. Move dates forward or backward using `EDATE()`.
9. Format dates for business reporting.
10. Build practical date-based business classifications.
11. Use date conditions inside `IF()`.
12. Use multiple date conditions with `SWITCH(TRUE())`.

---

## Practice Structure

### Part A — Basic Date Extraction
Questions 1–4

### Part B — Week Analysis
Questions 5–7

### Part C — DATE()
Question 8

### Part D — Current Date & Time
Questions 9–10

### Part E — Date Difference
Questions 11–13

### Part F — Business Date Classification
Questions 14–16

### Part G — EOMONTH()
Questions 17–18

### Part H — EDATE()
Questions 19–20

### Part I — Real Business Problems
Questions 21–25

---

## Important Rules

- Use the same `Sales_Order_Date_Practice` dataset for all questions.
- Work in Excel Power Pivot.
- Create calculated columns for row-level date calculations.
- Use the requested DAX function where specified.
- Pay close attention to date order in `DATEDIFF()`.
- Pay attention to `<`, `<=`, `>`, and `>=`.
- Do not manually type expected answers into calculated columns.
- Do not change the required output labels.
- For `SWITCH(TRUE())`, condition order matters.
- `TODAY()` and `NOW()` are dynamic functions, so their results change with the current date/time.

---

## Completion Standard

A formula is considered correct when:

- DAX syntax is valid.
- The requested function is used correctly.
- The correct date columns are referenced.
- Date arguments are in the correct order.
- Conditions match the question exactly.
- Operators match the requirement.
- Output labels match the required text.
- `SWITCH(TRUE())` conditions are in the correct priority order.
- The formula works for the complete dataset.

---

## Stage 5 Result

**Score: 98/100 — Passed**

One label-level correction was identified during review:

- Q25: `Need Attention` should be `Needs Attention`.

The underlying business logic was correct.

---

## Next Stage

**Stage 6 — Math & Statistical DAX**

The next stage will continue the same learning system:

**One dataset → 25 practical business questions → formula submission → strict review → score → next stage.**
