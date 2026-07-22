# 📖 Excel Lookup Functions Practice Questions

This document contains practical Lookup Function exercises based on multiple business datasets.

The questions simulate real-world Data Analyst tasks where information must be retrieved from different tables using lookup functions.

---

# 📊 Datasets

## Dataset 1 — Employee Master

Columns:

- Employee_ID
- Employee_Name
- Department
- Designation
- City
- Manager_ID
- Salary

---

## Dataset 2 — Manager Master

Columns:

- Manager_ID
- Manager_Name
- Experience
- Location

---

## Dataset 3 — Quarterly Sales

Columns:

- Product
- Q1
- Q2
- Q3
- Q4

---

# VLOOKUP()

### Problem 1
Retrieve the Employee Name using Employee_ID.

### Problem 2
Retrieve the Department using Employee_ID.

### Problem 3
Retrieve the Salary using Employee_ID.

### Problem 4
Retrieve the Designation for Employee EMP008.

### Problem 5
Retrieve the City for Employee EMP004.

---

# HLOOKUP()

Use the Quarterly Sales dataset.

### Problem 1
Retrieve Q3 sales for Laptop.

### Problem 2
Retrieve Q4 sales for Mobile.

### Problem 3
Retrieve Q2 sales for Printer.

### Problem 4
Retrieve Q1 sales for Monitor.

### Problem 5
Retrieve Q4 sales for Printer.

---

# XLOOKUP()

### Problem 1
Retrieve the Salary using Employee_ID.

### Problem 2
Retrieve the Department for Employee EMP009.

### Problem 3
Return "Employee Not Found" if the Employee_ID does not exist.

### Problem 4
Retrieve the Manager_ID using Employee_ID.

### Problem 5
Retrieve the Employee Name for EMP006.

---

# INDEX() + MATCH()

### Problem 1
Retrieve the Salary using Employee_ID.

### Problem 2
Retrieve the Department using Employee_ID.

### Problem 3
Retrieve the Designation using Employee_ID.

### Problem 4
Retrieve the City using Employee_ID.

### Problem 5
Retrieve the Employee Name using Employee_ID.

---

# ⭐ Challenge Problems

These exercises combine multiple datasets and simulate real business tasks.

---

## Challenge 1 — Manager Lookup

Using Employee Master and Manager Master, retrieve the Manager Name for every employee.

---

## Challenge 2 — Manager Experience

Retrieve the Manager's Experience (Years) for each employee.

---

## Challenge 3 — Manager Location

Retrieve the Manager's Office Location using Manager_ID.

---

## Challenge 4 — Employee Summary

Create the following format:

EMP004 - Sneha Ghosh - Developer - Bangalore

Use lookup functions to retrieve the required information.

---

## Challenge 5 — Salary Verification

Given a list of Employee_IDs, retrieve the corresponding Salary.

If an Employee_ID is not found, display:

Not Available

---

# 🎯 Goal

Complete all practice problems without referring to external solutions.

Focus on understanding:

- Which dataset contains the required information
- Which column should be used as the lookup key
- Which lookup function is best suited for the task
- How lookup functions help combine related datasets

Mastering these concepts will prepare you for real-world Excel reporting tasks and provide a strong foundation for SQL JOIN operations.
