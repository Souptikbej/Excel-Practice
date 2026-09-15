# Power Pivot DAX Practice --- Stage 3: Filter Functions

## Overview

This practice set is designed for a Data Analyst fresher learning
**Power Pivot DAX** through realistic business problems.

### Learning sequence

1.  Aggregation Functions
2.  Text Functions
3.  **Filter Functions ← Current Stage**
4.  Logical Functions
5.  Date & Time
6.  Math & Statistical
7.  Relationship Functions
8.  Iterator (X) Functions
9.  Ranking
10. Time Intelligence
11. Advanced DAX

------------------------------------------------------------------------

## Stage 3 Objective

The goal is **not** to memorize DAX formulas.

The goal is to learn how to identify:

> **Business requirement → Filter behavior → Appropriate DAX function →
> Measure**

You should be able to recognize when a requirement needs:

-   `CALCULATE()`
-   `FILTER()`
-   `ALL()`
-   `REMOVEFILTERS()`
-   `ALLEXCEPT()`
-   `VALUES()`
-   `SELECTEDVALUE()`

------------------------------------------------------------------------

## Dataset

Dataset name:

**Sales_Filter_Practice**

Columns:

  Column     Meaning
  ---------- -------------------------
  OrderID    Unique order identifier
  Date       Order date
  Customer   Customer name
  Product    Product purchased
  Category   Product category
  Region     Sales region
  Sales      Sales amount
  Profit     Profit amount
  Quantity   Quantity sold

Use the exact dataset provided in `Practice_Files.md`.

------------------------------------------------------------------------

## Important Rules

### Rule 1 --- Write DAX, not just the answer

For each question, submit the DAX measure.

Example:

``` dax
Total Sales =
SUM(Sales_Filter_Practice[Sales])
```

### Rule 2 --- Identify the filter behavior first

Before writing a formula, ask:

1.  What is the base metric?
2.  Which filter should be applied?
3.  Should an existing filter be preserved?
4.  Should an existing filter be removed?
5.  Should the measure respond dynamically to the current report
    selection?

### Rule 3 --- Avoid unnecessary hard-coding

For percentage-of-total questions, prefer dynamic measures.

For example, do not build a measure that works only for `East` if the
business requirement is intended to work for any selected region.

------------------------------------------------------------------------

## Functions Covered

### `CALCULATE()`

Used to evaluate an expression in a **modified filter context**.

Typical pattern:

``` dax
CALCULATE(
    [Measure],
    Table[Column] = "Value"
)
```

### `FILTER()`

Returns a filtered table based on a condition.

Typical pattern:

``` dax
CALCULATE(
    [Measure],
    FILTER(
        Table,
        Table[Sales] > 40000
    )
)
```

### `ALL()`

Removes filters from a table or column.

Typical use:

``` dax
CALCULATE(
    [Total Sales],
    ALL(Sales_Filter_Practice[Region])
)
```

### `REMOVEFILTERS()`

Explicitly removes filters.

Typical use:

``` dax
CALCULATE(
    [Total Sales],
    REMOVEFILTERS(Sales_Filter_Practice[Region])
)
```

### `ALLEXCEPT()`

Removes filters from a table except the specified columns.

Typical use:

``` dax
CALCULATE(
    [Total Sales],
    ALLEXCEPT(
        Sales_Filter_Practice,
        Sales_Filter_Practice[Region]
    )
)
```

### `VALUES()`

Returns the distinct values visible in the current filter context.

Typical pattern:

``` dax
COUNTROWS(
    VALUES(Sales_Filter_Practice[Region])
)
```

### `SELECTEDVALUE()`

Returns the selected value when there is one distinct value in the
current context.

Typical pattern:

``` dax
SELECTEDVALUE(
    Sales_Filter_Practice[Region],
    "Multiple/No Selection"
)
```

------------------------------------------------------------------------

## Completion Standard

Do not move to Stage 4 until you can explain:

-   Why `CALCULATE()` is required.
-   When a simple filter argument is enough.
-   When `FILTER()` is appropriate.
-   Why `ALL()` changes the result.
-   Difference between `ALL()` and `REMOVEFILTERS()`.
-   What `ALLEXCEPT()` preserves.
-   What `VALUES()` returns.
-   Why `SELECTEDVALUE()` is useful in dynamic reports.
-   Why percentage-of-total measures often require filter removal.

------------------------------------------------------------------------

## Submission Standard

Submit all **25 DAX measures** from `Practice_Files.md`.

For each answer, the reviewer should be able to determine:

-   Correct function
-   Correct column
-   Correct filter condition
-   Correct filter context behavior
-   Correct business logic
-   Dynamic behavior where required

------------------------------------------------------------------------

## Interview Focus

A good Data Analyst should be able to explain the business meaning of a
measure, not only its syntax.

Example interview question:

> "Why did you remove the Region filter from the denominator?"

Expected reasoning:

> "Because the numerator represents the current region's sales, while
> the denominator represents total company sales across all regions.
> Removing the Region filter allows the measure to calculate the
> region's contribution to total company sales."
