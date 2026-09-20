# Stage 4 — Logical DAX Practice

## Overview

Stage 4 focuses on **Logical DAX functions** in Excel Power Pivot.

The goal of this stage is not only to memorize functions, but to learn how to convert real business rules into DAX logic.

### Functions Covered

- `IF()`
- `AND()`
- `OR()`
- `NOT()`
- `SWITCH()`
- `IFERROR()`
- `SWITCH(TRUE())`

---

## Dataset

**Dataset name:** `Employee_Performance`

The dataset contains employee performance information.

| Column | Description |
|---|---|
| EmpID | Employee ID |
| Employee | Employee name |
| Department | Employee department |
| Sales | Employee sales amount |
| Target | Sales target |
| Profit | Profit generated |
| Attendance% | Employee attendance percentage |
| ExperienceYears | Years of experience |
| Rating | Performance rating from 1–5 |

---

## Learning Objectives

By completing this stage, you should be able to:

1. Create business conditions using `IF()`.
2. Combine multiple conditions using `AND()`.
3. Handle alternative conditions using `OR()`.
4. Reverse a logical condition using `NOT()`.
5. Create multiple categories using `SWITCH()`.
6. Use `SWITCH(TRUE())` for business-rule classification.
7. Handle calculation errors using `IFERROR()`.
8. Understand condition priority when multiple business rules overlap.
9. Translate business requirements into DAX calculated columns.

---

## Practice Structure

### Part A — IF()
Basic business decisions using a single condition.

### Part B — IF with Business Conditions
Using `IF()` for target and performance decisions.

### Part C — AND()
Checking whether multiple conditions are simultaneously true.

### Part D — OR()
Checking whether at least one condition is true.

### Part E — NOT()
Reversing a logical condition.

### Part F — SWITCH()
Creating categories from rating and performance values.

### Part G — Combined Business Logic
Combining multiple logical conditions using `SWITCH(TRUE())`.

### Part H — IFERROR()
Creating safe percentage calculations.

### Part I — Real Business Problems
Applying multiple business rules and understanding rule priority.

---

## Important Rules

- Use the exact dataset provided for this stage.
- Use the function requested in each question.
- Do not change the required output labels.
- Pay attention to `>`, `>=`, `<`, `<=`, and `=`.
- In `SWITCH(TRUE())`, **condition order matters**.
- Do not hard-code employee-specific answers.
- Build formulas that work for every row in the dataset.
- For calculated columns, use the appropriate table column references.
- For percentage calculations, use `IFERROR()` where requested.

---

## Completion Standard

A formula is considered correct only when:

- The syntax is valid.
- The requested function is used correctly.
- All conditions match the question.
- Operators match the requirement exactly.
- Output labels match the requested text.
- Multiple conditions are evaluated in the correct order.
- The formula works correctly for the complete dataset.

---

## Stage 4 Result

**Score: 98/100 — Passed**

Two issues were identified during review:

- Q5: Output label should be `Not Eligible`, not `No Bonus`.
- Q22: Output label should be `Needs Improvement`, not `Need Improvement`.

Both were label-level mistakes; the underlying logical conditions were correct.

---

## Next Stage

**Stage 5 — Date & Time DAX**

The next stage will focus on date-based business analysis and DAX date/time functions.
