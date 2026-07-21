# 📖 Excel Date & Time Functions Practice Questions

This document contains practical Excel Date & Time Function exercises based on a single Customer Orders dataset.

The questions are inspired by real business scenarios that Data Analysts commonly solve.

---

# Dataset Columns

| Column |
|---------|
| Order_ID |
| Order_Date |
| Delivery_Date |
| Customer_Name |
| Region |
| Order_Status |
| Sales |

---

# DATE()

### Problem 1
Create an Expected Invoice Date by adding 2 days to the Order Date using the DATE() function.

### Problem 2
Create a date representing the first day of the Order Month.

### Problem 3
Create a date representing the last day of the Order Month using DATE() logic (without using EOMONTH()).

### Problem 4
Create the Financial Year Start Date (1-Apr) for the year of each Order Date.

### Problem 5
Create a new column showing 1-Jan of the same year as the Order Date.

---

# TODAY() / NOW()

### Problem 1
Calculate the number of days since each order was placed.

### Problem 2
Identify orders that are older than 30 days.

### Problem 3
Identify orders placed within the last 7 days.

### Problem 4
Calculate the age of each order using today's date.

### Problem 5
Display today's date as the report generation date.

---

# YEAR() / MONTH() / DAY()

### Problem 1
Extract the Order Year.

### Problem 2
Extract the Order Month Number.

### Problem 3
Extract the Day of the Month.

### Problem 4
Identify all orders placed during March.

### Problem 5
Create a Month-Year helper column (Example: Jan-2025).

---

# WEEKDAY() / WEEKNUM()

### Problem 1
Find the weekday number for each Order Date.

### Problem 2
Identify whether each order was placed on a Weekend or Weekday.

### Problem 3
Calculate the week number for each Order Date.

### Problem 4
Identify all orders placed during Week 12.

### Problem 5
Create a new column categorizing each order as Weekend or Weekday.

---

# DATEDIF()

### Problem 1
Calculate the delivery time in days.

### Problem 2
Identify orders delivered in more than 5 days.

### Problem 3
Identify orders delivered within 3 days.

### Problem 4
Categorize deliveries as Fast, Normal, or Delayed based on delivery duration.

### Problem 5
Calculate the number of complete months between the Order Date and Today().

---

# EDATE() / EOMONTH()

### Problem 1
Calculate the contract renewal date after 3 months.

### Problem 2
Calculate the last day of the Order Month.

### Problem 3
Calculate the last day of the month after 6 months.

### Problem 4
Calculate the first day of the next month.

### Problem 5
Calculate the last day of the previous month.

---

# NETWORKDAYS() / NETWORKDAYS.INTL()

Assume Saturday and Sunday are weekends.

### Problem 1
Calculate the number of working days between the Order Date and Delivery Date.

### Problem 2
Identify orders that required more than 5 working days for delivery.

### Problem 3
Calculate working days excluding a predefined list of holidays.

### Problem 4
Assume only Sunday is considered a weekend using NETWORKDAYS.INTL() and compare the result.

### Problem 5
Identify orders completed within 3 working days.

---

# TEXT()

### Problem 1
Display the Order Date in the format:

dd-mmm-yyyy

### Problem 2
Display the Order Date as:

Month Year

Example:

January 2025

### Problem 3
Display only the weekday name.

### Problem 4
Display the Order Date as:

05 January, 2025

### Problem 5
Create the following format:

Week 12 - March

---

# ⭐ Challenge Problems

### Challenge 1 — Delivery SLA

Categorize deliveries as:

- On Time (≤3 days)
- Slight Delay (4–6 days)
- Late (>6 days)

---

### Challenge 2 — Monthly Sales Report

Create a Month-Year helper column to prepare monthly sales reports.

---

### Challenge 3 — Weekend Analysis

Identify all orders placed on weekends and calculate their total sales.

---

### Challenge 4 — Business Days vs Calendar Days

Calculate both Calendar Days and Working Days for each order and compare the results.

---

### Challenge 5 — Monthly Closing Report

Create a column that shows the last day of the Order Month and determine whether the order was placed in the First Half or Second Half of the month.

---

# 🎯 Goal

Complete all practice problems without referring to external solutions.

Focus on understanding how Date & Time functions are applied in real-world business reporting, operational analysis, and data preparation tasks performed by Data Analysts.
