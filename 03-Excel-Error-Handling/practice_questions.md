# 📝 IFERROR & IFNA Practice Questions

## Dataset

| Order ID | Salesperson | Sales | Target | Units Sold | Customer Email |
|----------|-------------|-------:|-------:|-----------:|----------------|
| O101 | Amit | 50000 | 45000 | 25 | amit@gmail.com |
| O102 | Priya | 42000 | 42000 | 0 | priya@gmail.com |
| O103 | Rahul | 38000 | 40000 | 18 | rahulgmail.com |
| O104 | Sneha | 62000 | 50000 | 31 | sneha@gmail.com |
| O105 | Vikash | 0 | 35000 | 0 | vikash@gmail.com |
| O106 | Riya | 56000 | 55000 | 28 | riya@gmail.com |
| O107 | Arjun | 47000 | 50000 | 20 | arjunmail.com |
| O108 | Neha | 39000 | 39000 | 15 | neha@gmail.com |

---

# Part 1 — IFERROR Practice

## Problem 1

Calculate:

```
Sales / Units Sold
```

If an error occurs, display:

```
No Sales
```

---

## Problem 2

Calculate commission:

```
Sales / Units Sold × 5
```

If an error occurs, display:

```
0
```

---

## Problem 3

Extract the username from the email.

Example:

```
amit@gmail.com
```

Output:

```
amit
```

If the email is invalid, display:

```
Invalid Email
```

Hint:

- LEFT
- FIND
- IFERROR

---

## Problem 4

Calculate:

```
Sales / Units Sold × 100
```

If an error occurs, display:

```
Pending
```

---

## Problem 5

Calculate:

```
Sales / Target × 1000
```

If an error occurs, return a blank cell.

---

## Problem 6

Extract the email domain.

Example:

```
amit@gmail.com
```

Output:

```
gmail.com
```

If invalid, display:

```
No Domain
```

Hint:

- MID
- FIND
- LEN
- IFERROR

---

## Problem 7

Calculate:

```
(Sales / Units Sold) + 10
```

If an error occurs, return:

```
0
```

---

## Problem 8

Return the first letter of the email domain.

Example:

```
gmail.com
```

Output:

```
g
```

If invalid:

```
NA
```

---

# Mini Challenge

Create the following columns.

---

## 1. Average Revenue Per Unit

```
Sales / Units Sold
```

If an error occurs:

```
Check Units
```

---

## 2. Email Status

If the email is valid:

```
Valid
```

Otherwise:

```
Invalid Email
```

---

## 3. Bonus Eligibility

If Average Revenue is greater than **2000**

Display:

```
Eligible
```

Otherwise:

```
Not Eligible
```

---

# Part 2 — IFNA Practice

Assume the worksheet already contains the following data.

| Employee | Rating |
|----------|--------|
| Amit | A |
| Priya | B |
| Rahul | #N/A |
| Sneha | A |
| Vikash | #N/A |

---

## Problem 1

Replace

```
#N/A
```

with

```
Not Rated
```

---

## Problem 2

Replace

```
#N/A
```

with

```
0
```

---

## Problem 3

Replace

```
#N/A
```

with

```
Review Pending
```

---

## Problem 4

Replace

```
#N/A
```

with

```
Missing Data
```

while keeping all other values unchanged.

---

## Problem 5

Create a Status column.

If the rating is

```
#N/A
```

display

```
Needs Review
```

Otherwise display

```
Completed
```

---

# 🎯 Challenge Yourself

Without using Google, try to solve every problem using only:

- IFERROR
- IFNA
- IF
- LEFT
- RIGHT
- MID
- FIND
- LEN

---

## Learning Outcome

After completing these exercises, you should be able to:

- Handle common Excel errors
- Create user-friendly reports
- Prevent formulas from displaying error messages
- Understand when to use IFERROR vs IFNA
- Prepare for Lookup functions like VLOOKUP and XLOOKUP
