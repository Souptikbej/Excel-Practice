# Power Pivot Learning Roadmap

## Goal

Learn Power Pivot from beginner to job-ready level for Data Analyst roles.

---

# Learning Progress

## Module 1 — Power Pivot Basics ✅

### Topics Covered

- What is Power Pivot?
- Power Pivot Window
- Data Model
- Fact Table
- Dimension Table
- Relationships
- One-to-Many Relationship
- Primary Key
- Foreign Key
- Diagram View
- Calculated Column
- Measure
- PivotTable using Data Model

---

## Dataset Used

Retail Sales Dataset

Tables:

- Customers
- Products
- Sales
- Date

---

# Relationships

Customers(CustomerID)
        │
        │ 1 → *
        ▼
Sales(CustomerID)

Products(ProductID)
        │
        │ 1 → *
        ▼
Sales(ProductID)

Date(Date)
        │
        │ 1 → *
        ▼
Sales(Date)

---

# Star Schema

            Customers
                 │
Products ─── Sales ─── Date

Sales = Fact Table

Customers, Products, Date = Dimension Tables

---

# Calculated Columns Learned

## Sales Amount

```DAX
Sales Amount =
fct_Sales[Quantity] * RELATED(dim_Products[UnitPrice])
```

Purpose

- Fetch UnitPrice from Product table
- Calculate row-wise sales

---

## Product Category

```DAX
Product Category =
RELATED(dim_Products[Category])
```

Purpose

Learn how RELATED() works.

---

## Customer State

```DAX
Customer State =
RELATED(dim_Customers[State])
```

Purpose

Bring values from related table.

---

# Measures Learned

## Total Sales Amount

```DAX
Total Sales Amount =
SUM(fct_Sales[Sales Amount])
```

---

## Total Quantity Sold

```DAX
Total Quantity Sold =
SUM(fct_Sales[Quantity])
```

---

## Average Sales per Transaction

```DAX
Average Sales per Transaction =
AVERAGE(fct_Sales[Sales Amount])
```

---

## Number of Orders

```DAX
Number of Orders =
COUNTROWS(fct_Sales)
```

---

## Distinct Customers

```DAX
Distinct Customers =
DISTINCTCOUNT(fct_Sales[CustomerID])
```

---

## Highest Transaction

```DAX
Highest Transaction =
MAX(fct_Sales[Sales Amount])
```

---

# DAX Functions Learned

- RELATED()
- SUM()
- AVERAGE()
- COUNTROWS()
- DISTINCTCOUNT()
- MAX()

---

# Business Analysis Completed

✔ Category-wise Sales

✔ State-wise Sales

✔ Customer-wise Sales

✔ Product-wise Sales

✔ Highest Revenue Product

✔ Highest Revenue Customer

---

# Important Concepts

## Calculated Column

- Calculated once
- Stored in memory
- Row Context

Example

Quantity × Unit Price

---

## Measure

- Calculated when needed
- Not stored
- Filter Context

Example

SUM(Sales Amount)

---

# Current Skill Level

✅ Data Model

✅ Relationships

✅ RELATED()

✅ Calculated Columns

✅ Basic Measures

✅ PivotTables

---

# Next Topics

- SUMX()
- DIVIDE()
- IF()
- RELATEDTABLE()

After that:

- CALCULATE()
- FILTER()
- ALL()
- VALUES()
- Time Intelligence
- Variables (VAR)

---

# Current Status

Module 1 Completed Successfully
