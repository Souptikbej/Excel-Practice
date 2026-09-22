# Stage 5 — Date & Time DAX Practice Questions

## Dataset: `Sales_Order_Date_Practice`

Use this **single dataset for all 25 questions**.

| OrderID | OrderDate | Customer | Region | Product | Quantity | Sales | DeliveryDate | PaymentDate |
|---:|---|---|---|---|---:|---:|---|---|
| 2001 | 05-Jan-2026 | Rahul | East | Laptop | 2 | 100000 | 09-Jan-2026 | 12-Jan-2026 |
| 2002 | 08-Jan-2026 | Priya | West | Mouse | 5 | 5000 | 11-Jan-2026 | 15-Jan-2026 |
| 2003 | 12-Jan-2026 | Amit | South | Chair | 3 | 12000 | 18-Jan-2026 | 20-Jan-2026 |
| 2004 | 20-Jan-2026 | Sneha | North | Monitor | 2 | 50000 | 25-Jan-2026 | 28-Jan-2026 |
| 2005 | 28-Jan-2026 | Raj | East | Keyboard | 4 | 8000 | 02-Feb-2026 | 05-Feb-2026 |
| 2006 | 03-Feb-2026 | Anita | West | Laptop | 1 | 55000 | 07-Feb-2026 | 10-Feb-2026 |
| 2007 | 10-Feb-2026 | Vikas | South | Printer | 2 | 30000 | 15-Feb-2026 | 18-Feb-2026 |
| 2008 | 18-Feb-2026 | Neha | North | Table | 2 | 16000 | 23-Feb-2026 | 26-Feb-2026 |
| 2009 | 25-Feb-2026 | Rohit | East | Monitor | 3 | 75000 | 02-Mar-2026 | 05-Mar-2026 |
| 2010 | 02-Mar-2026 | Pooja | West | Laptop | 2 | 110000 | 06-Mar-2026 | 09-Mar-2026 |
| 2011 | 10-Mar-2026 | Arjun | South | Chair | 4 | 16000 | 15-Mar-2026 | 18-Mar-2026 |
| 2012 | 18-Mar-2026 | Kavya | North | Printer | 1 | 15000 | 23-Mar-2026 | 26-Mar-2026 |
| 2013 | 25-Mar-2026 | Suman | East | Laptop | 1 | 60000 | 30-Mar-2026 | 02-Apr-2026 |
| 2014 | 05-Apr-2026 | Deepak | West | Monitor | 2 | 52000 | 10-Apr-2026 | 13-Apr-2026 |
| 2015 | 15-Apr-2026 | Meera | South | Keyboard | 6 | 12000 | 20-Apr-2026 | 23-Apr-2026 |

---

# Part A — Basic Date Extraction

## Q1 — Order Year

Create a calculated column that extracts the **year** from `OrderDate`.

Use:

`YEAR()`

---

## Q2 — Order Month Number

Create a calculated column that extracts the **month number** from `OrderDate`.

Use:

`MONTH()`

---

## Q3 — Order Day

Create a calculated column that extracts the **day number** from `OrderDate`.

Use:

`DAY()`

---

## Q4 — Order Quarter

Create a calculated column that classifies each order into:

- `Q1`
- `Q2`
- `Q3`
- `Q4`

based on the month of `OrderDate`.

Use the month number in your logic.

---

# Part B — Week Analysis

## Q5 — Day of Week Number

Create a calculated column using:

`WEEKDAY()`

Use the default DAX `WEEKDAY()` return behavior.

Return the weekday number for each `OrderDate`.

---

## Q6 — Day Type

Create a calculated column:

- Saturday or Sunday → `Weekend`
- Otherwise → `Weekday`

Use `WEEKDAY()` with the appropriate logical conditions.

---

## Q7 — Week Number

Create a calculated column using:

`WEEKNUM()`

Return the week number of each `OrderDate`.

---

# Part C — DATE()

## Q8 — Constructed Date

Create a calculated column called `Constructed Date`.

Using `OrderDate`, reconstruct the same date using:

`DATE()`

The formula should use the:

- Year
- Month
- Day

from `OrderDate`.

---

# Part D — Current Date & Time

## Q9 — Current Date

Create a calculated column using:

`TODAY()`

Return today's date.

**Note:** The result changes depending on the date when the workbook is calculated.

---

## Q10 — Current Date/Time

Create a calculated column using:

`NOW()`

Return the current date and time.

**Note:** `NOW()` includes both date and time.

---

# Part E — Date Difference

## Q11 — Delivery Days

Management wants to know:

> How many days did each order take to deliver?

Calculate:

`DeliveryDate - OrderDate`

Use:

`DATEDIFF()`

Return the number of days.

---

## Q12 — Payment Collection Days

Management wants to know:

> How many days after delivery did we receive payment?

Calculate:

`PaymentDate - DeliveryDate`

Use:

`DATEDIFF()`

Return the number of days.

---

## Q13 — Total Order-to-Payment Days

Calculate:

`PaymentDate - OrderDate`

Use:

`DATEDIFF()`.

This represents the total time from order placement to payment receipt.

---

# Part F — Business Date Classification

## Q14 — Delivery Performance

The company considers:

- Delivery in **4 days or less** → `Fast Delivery`
- More than 4 days → `Slow Delivery`

Create a calculated column using `IF()` and the delivery duration.

---

## Q15 — Payment Performance

The company considers:

- Payment received within **5 days or less after delivery** → `Quick Payment`
- More than 5 days → `Delayed Payment`

Create the calculated column.

---

## Q16 — Order Month Name

Create a calculated column that returns the month name:

- January
- February
- March
- April
- etc.

Use:

`FORMAT()` with `OrderDate`.

---

# Part G — EOMONTH()

## Q17 — Month End Date

Create a calculated column called `Month End Date`.

For each `OrderDate`, return the last date of that month.

Examples:

- 05-Jan-2026 → 31-Jan-2026
- 18-Feb-2026 → 28-Feb-2026
- 25-Mar-2026 → 31-Mar-2026

Use:

`EOMONTH()`

---

## Q18 — Next Month End Date

Create a calculated column that returns the last date of the following month.

Examples:

- 05-Jan-2026 → 28-Feb-2026
- 18-Feb-2026 → 31-Mar-2026

Use:

`EOMONTH()`.

---

# Part H — EDATE()

## Q19 — Three Months Later

Create a calculated column that returns the date exactly **3 months after `OrderDate`**.

Use:

`EDATE()`

Example:

05-Jan-2026 → 05-Apr-2026

---

## Q20 — One Month Earlier

Create a calculated column that returns the date exactly **1 month before `OrderDate`**.

Use:

`EDATE()`.

---

# Part I — Real Business Problems

## Q21 — Delivery SLA Status

The company's delivery SLA is **5 days**.

Create a calculated column:

- Delivery Days <= 5 → `SLA Met`
- Delivery Days > 5 → `SLA Breached`

Use the appropriate date calculation and `IF()`.

---

## Q22 — Payment Status

Create a calculated column:

- Payment Collection Days <= 5 → `On Time`
- Payment Collection Days > 5 → `Delayed`

Base the calculation on:

`PaymentDate - DeliveryDate`

---

## Q23 — Order Age

Create a calculated column that calculates the number of days between:

`OrderDate`

and:

`TODAY()`

Use:

`DATEDIFF()`

Return the number of days.

**Note:** Because this uses `TODAY()`, the result changes over time.

---

## Q24 — Business Order Category

Create a calculated column using:

- Order is **30 days old or less** → `Recent Order`
- Order is more than 30 days old → `Older Order`

Use:

- `TODAY()`
- `DATEDIFF()`
- `IF()`

---

## Q25 — Overall Order Performance

Create a calculated column called `Order Performance`.

Use `SWITCH(TRUE())` with these rules **in this exact order**:

### Excellent

- Delivery Days <= 4
- AND Payment Collection Days <= 5

Return:

`Excellent`

### Good

- Delivery Days <= 5
- AND Payment Collection Days <= 7

Return:

`Good`

### Needs Attention

- Delivery Days > 5
- OR Payment Collection Days > 7

Return:

`Needs Attention`

**Important:** Condition order matters.

---

# Submission Format

When you finish, submit all 25 DAX formulas together:

```text
Q1: [DAX formula]
Q2: [DAX formula]
Q3: [DAX formula]
...
Q25: [DAX formula]
```

## Review Criteria

Every formula will be checked for:

- DAX syntax
- Correct Excel Power Pivot usage
- Correct function
- Correct column references
- Correct date order
- Correct operators
- Correct business logic
- Correct output labels
- Correct `SWITCH(TRUE())` order
- Formula consistency across the dataset

## Stage 5 Completion Target

The goal is not merely to get the answer.

You should be able to look at a business requirement and recognize:

**Which date function? → Which columns? → What date relationship? → What condition? → What output?**
