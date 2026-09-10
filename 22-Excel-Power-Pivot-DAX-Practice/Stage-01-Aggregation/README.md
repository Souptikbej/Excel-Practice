# Stage 01 – Aggregation Functions

## Overview

Welcome to **Stage 01** of the **Power Pivot DAX Practice Series**.

This stage focuses on the most fundamental DAX functions used in data analysis—**Aggregation Functions**. These functions are the building blocks for creating business metrics and Key Performance Indicators (KPIs).

---

## Learning Objectives

After completing this stage, you should be able to:

- Create DAX Measures in Power Pivot.
- Identify numeric fields suitable for aggregation.
- Select the correct aggregation function based on a business requirement.
- Understand the difference between `COUNT()`, `COUNTA()`, and `DISTINCTCOUNT()`.
- Build basic business KPIs using DAX.

---

## Functions Covered

| Category | Functions |
|----------|-----------|
| Sum | `SUM()` |
| Average | `AVERAGE()` |
| Minimum | `MIN()` |
| Maximum | `MAX()` |
| Count | `COUNT()` |
| Count Non-Blank | `COUNTA()` |
| Distinct Count | `DISTINCTCOUNT()` |

---

## Dataset

The dataset contains sales transactions with the following fields:

| Field | Description |
|--------|-------------|
| OrderID | Unique order identifier |
| Customer | Customer name |
| Product | Product name |
| Category | Product category |
| Qty | Quantity sold |
| Unit Price | Price per unit |
| Sales | Total sales amount |
| Discount | Discount amount |
| Profit | Profit earned |
| Region | Sales region |

---

## Folder Structure

```
Stage-01-Aggregation/
│
├── README.md
├── Dataset.xlsx
├── Practice_Questions.md
├── My_Solutions.xlsx
├── Expected_Output.md
└── Screenshots/
```

---

## Practice Tasks

Complete all questions in `Practice_Questions.md`.

The questions are divided into the following categories:

- SUM()
- AVERAGE()
- MIN()
- MAX()
- COUNT()
- COUNTA()
- DISTINCTCOUNT()

The final section contains business-oriented questions similar to those asked during Data Analyst interviews and encountered in real-world reporting scenarios.

---

## Expected Deliverables

Before moving to Stage 02, ensure that you have:

- Imported the dataset into the Power Pivot Data Model.
- Created all required DAX Measures.
- Verified each measure using a PivotTable.
- Saved the workbook as `My_Solutions.xlsx`.
- Added screenshots of your completed work.
- Compared your results with `Expected_Output.md`.

---

## Skills Gained

By completing this stage, you will gain experience in:

- Creating DAX Measures
- Understanding aggregation logic
- Selecting the correct function for different business scenarios
- Building foundational business KPIs
- Working with Excel Power Pivot

---

## Completion Checklist

- [ ] Dataset imported into Power Pivot
- [ ] All DAX measures created
- [ ] All 25 questions completed
- [ ] Measures validated using PivotTable
- [ ] Workbook saved as `My_Solutions.xlsx`
- [ ] Screenshots added
- [ ] Solutions reviewed

---

## Next Stage

**Stage 02 – Text Functions**

Topics include:

- LEFT()
- RIGHT()
- MID()
- LEN()
- UPPER()
- LOWER()
- PROPER()
- TRIM()
- CONCATENATE()
- SEARCH()
- FIND()
- REPLACE()
- SUBSTITUTE()

These functions are commonly used for cleaning and transforming text data before analysis.