# Excel Data Cleaning Practice Questions

This practice set simulates real business scenarios faced by Data Analysts.

Use the provided dataset to solve all questions.

---

# Topic 1 — Remove Duplicates

## Problem 1

Remove all duplicate employee records from the dataset.

---

## Problem 2

Before removing duplicates, determine how many duplicate employee records exist.

---

## Problem 3

Remove duplicate records using only:

- Full_Name
- Email

---

## Problem 4

Remove duplicate records based only on Phone Number.

---

## Problem 5

After removing duplicate records, calculate:

- Total Sales
- Average Sales

---

# Topic 2 — Find & Replace

## Problem 1

Replace:

```
Laptop
```

with

```
Notebook
```

---

## Problem 2

Replace:

```
Inactive
```

with

```
Active
```

---

## Problem 3

Replace:

```
East
```

with

```
Eastern
```

---

## Problem 4

Replace:

```
gmail.com
```

with

```
company.com
```

---

## Problem 5

Replace Manager Name:

```
Raj Mehta
```

with

```
Rajesh Mehta
```

---

# Topic 3 — Text to Columns

## Problem 1

Split **Full_Name** into:

- First_Name
- Last_Name

---

## Problem 2

Split **City_State** into:

- City
- State

using comma delimiter.

---

## Problem 3

Split Email into:

- Username
- Domain

using @ delimiter.

---

## Problem 4

Split Join_Date into:

- Day
- Month
- Year

using "-" delimiter.

---

## Problem 5

Split Phone Number using Fixed Width.

Example:

```
9876543210

↓

98765 | 43210
```

---

# Topic 4 — Merge / Consolidate / Append

## Problem 1 — Merge

Merge the Bonus_Data table with Employee data using:

```
Emp_ID
```

Expected Output:

Employee table should contain a new Bonus column.

---

## Problem 2 — Append

Create another worksheet named:

```
New_Employees
```

Add five employee records.

Append the new worksheet below the existing Employee dataset.

---

## Problem 3 — Consolidate

Create separate worksheets for:

- East
- West
- North
- South

Use Consolidate to calculate the total Sales from all four worksheets into a Summary worksheet.

---

## Problem 4 — Append

Create two datasets:

- Employee_2023
- Employee_2024

Append both into a single Master Employee table.

---

## Problem 5 — Merge + Calculation

Merge Employee data with Bonus_Data.

Create a new column:

```
Total_Earnings = Sales + Bonus
```

Calculate Total Earnings for every employee.

---

# Bonus Challenge

Without using formulas:

✔ Remove duplicates

✔ Replace text

✔ Split text into columns

✔ Merge Bonus data

✔ Append new employees

✔ Consolidate regional sales

using only Excel's built-in Data tools (Power Query allowed).

---

# Expected Skills

- Remove Duplicates
- Find & Replace
- Text to Columns
- Fixed Width
- Delimited Split
- Merge Queries
- Append Queries
- Consolidate
- Power Query
- Data Cleaning

---

## Difficulty

🟢 Beginner

Estimated Completion Time:

**45–60 Minutes**

Happy Practicing! 🚀
