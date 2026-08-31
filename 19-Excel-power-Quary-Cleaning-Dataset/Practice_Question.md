# Power Query Practice Questions

## Instructions

Use **only the provided dataset**.

Do not create another dataset.

Each question represents a common real-world data cleaning task performed by Data Analysts.

---

# Question 1 — Remove Blank Rows

Remove all rows where:

- Sales is blank
- Phone is blank

---

# Question 2 — Remove Duplicate Records

Remove duplicate rows using:

```
Order ID
```

Only one record should remain for each Order ID.

---

# Question 3 — Trim Extra Spaces

Remove leading and trailing spaces from:

- Customer Name
- Email

---

# Question 4 — Fix Data Types

Assign the correct data type to each column.

| Column | Data Type |
|---------|-----------|
| Order ID | Whole Number |
| Customer Name | Text |
| Product | Text |
| Category | Text |
| Region | Text |
| Order Date | Date |
| Sales | Decimal Number |
| Quantity | Whole Number |
| Month | Text |
| Phone | Text |
| Email | Text |

---

# Question 5 — Replace Missing Values

Replace blank values in the **Sales** column with:

```
0
```

---

# Question 6 — Convert Customer Name

Convert every Customer Name into:

```
Proper Case
```

Example

```
alice
```

↓

```
Alice
```

---

# Question 7 — Convert Email

Convert every email address into:

```
Lowercase
```

---

# Question 8 — Split Email

Split the Email column using:

```
@
```

Create two new columns:

- Username
- Domain

Example

| Username | Domain |
|-----------|----------|
| alice | gmail.com |

---

# Question 9 — Replace Domain

Replace

```
gmail.com
```

with

```
company.com
```

---

# Question 10 — Pivot Data

Create a Pivot Column.

Use:

Rows

```
Month
```

Pivot Column

```
Category
```

Values

```
Sales
```

Aggregation

```
Sum
```

Expected Output

| Month | Electronics | Furniture |
|--------|-------------|------------|

---

# Question 11 — Unpivot Data

Using the Pivot table created in Question 10,

Unpivot:

- Electronics
- Furniture

Final Output

| Month | Category | Sales |
|--------|----------|--------|

---

# Final Challenge

Using the same dataset, perform the complete Power Query workflow:

- Remove blank rows
- Remove duplicates
- Trim text
- Fix data types
- Replace null values
- Convert Customer Name to Proper Case
- Convert Email to Lowercase
- Split Email into Username and Domain
- Replace Domain values
- Create a Pivot table
- Unpivot the Pivot table

---

## Goal

Complete all questions without modifying the original dataset structure.

The objective is to become comfortable with the most common Power Query data cleaning operations used in real business projects and Data Analyst interviews.
