# DAX Stage 2 — Text Functions Practice

## Overview

This practice set is designed for a Data Analyst fresher learning **Power Pivot / DAX**.

The focus of Stage 2 is **Text Functions in DAX** using a realistic Employee Master dataset.

The goal is not only to write formulas, but also to learn:

- Which column should be used
- Which DAX text function is appropriate
- Whether the result should be text, number, or TRUE/FALSE
- How text functions are used in practical data-analysis work

> **Important:** This stage uses DAX functions only. `PROPER()` is **not a DAX function**, so it is not included.

---

## Dataset

### Table Name
`Employee_Master`

| EmpID | Employee Name | Email | Department | City | Employee Code | Mobile |
|---:|---|---|---|---|---|---|
| 101 | Rahul Sharma | rahul.sharma@abc.com | Sales | Kolkata | EMP-1001 | 9876543210 |
| 102 | Priya Das | priya.das@abc.com | HR | Mumbai | EMP-1002 | 9123456789 |
| 103 | Amit Roy | amit.roy@abc.com | Finance | Delhi | EMP-1003 | 9988776655 |
| 104 | Sneha Paul | sneha.paul@abc.com | IT | Pune | EMP-1004 | 9012345678 |
| 105 | Vikas Singh | vikas.singh@abc.com | Marketing | Bangalore | EMP-1005 | 8899776655 |
| 106 | Neha Gupta | neha.gupta@abc.com | Sales | Chennai | EMP-1006 | 9988112233 |
| 107 | Anita Bose | anita.bose@abc.com | IT | Hyderabad | EMP-1007 | 9871234567 |
| 108 | Raj Verma | raj.verma@abc.com | Finance | Jaipur | EMP-1008 | 9123987654 |
| 109 | Pooja Sen | pooja.sen@abc.com | HR | Lucknow | EMP-1009 | 9000011111 |
| 110 | Rohit Ghosh | rohit.ghosh@abc.com | Sales | Patna | EMP-1010 | 9998887776 |

---

## Functions Covered

### Core Text Functions
- `LEFT()`
- `RIGHT()`
- `MID()`
- `LEN()`
- `UPPER()`
- `LOWER()`
- `TRIM()`
- `SEARCH()`
- `FIND()`
- `SUBSTITUTE()`
- `REPLACE()`
- `REPT()`
- `EXACT()`
- `FORMAT()`

### Text Combination
- `&` concatenation

### Supporting Logic
- `IF()`

---

## Learning Rules

1. Use the supplied table and column names.
2. Solve each question using **DAX**.
3. Prefer a calculated column when the question is row-by-row.
4. Do not introduce columns that are not present in the supplied dataset unless you explicitly create them first.
5. For `Mobile`, treat the value as a **Text** field because phone numbers are identifiers, not quantities.
6. `FORMAT()` returns **text**, even when formatting a number.
7. `EXACT()` performs a **case-sensitive** text comparison.
8. `PROPER()` must not be used because it is not a DAX function.
9. For text extraction, pay attention to spaces and character positions.
10. Do not move to the next stage until the current stage has been checked.

---

## Expected Learning Outcome

After completing Stage 2, you should be able to handle common text-cleaning and text-transformation requirements such as:

- Extracting names, IDs, usernames, and domains
- Creating employee labels
- Standardizing text case
- Searching for characters or text
- Replacing or removing characters
- Validating text patterns
- Creating display-friendly labels
- Performing case-sensitive comparisons
- Repeating text dynamically

---

## Stage 2 Completion Standard

A strong Data Analyst candidate should be able to:

- Identify the correct source column
- Select the correct DAX function
- Write syntactically correct DAX
- Produce the expected output
- Explain why that function was selected
- Understand whether the result is Text, Number, or Boolean

**Target:** 90%+ correct before moving to Stage 3.
