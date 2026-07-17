# 📖 Excel Text Functions Practice Questions

This document contains practice problems based on a single HR Employee dataset.

The problems simulate common business tasks performed by Data Analysts while cleaning and preparing data.

---

# Dataset Columns

| Column |
|---------|
| Employee_ID |
| Full_Name |
| Email |
| Department |
| City |
| Employee_Code |
| Remarks |

---

# LEFT()

### Problem 1
Extract the department prefix from Employee_Code.

### Problem 2
Extract the first 3 letters of each employee's name.

### Problem 3
Create a short employee tag using the first 4 characters of Employee_ID.

### Problem 4
Extract the first 2 letters of the City.

### Problem 5
Extract the first word of the Department.

### Problem 6
Create a department abbreviation using the first 3 letters.

---

# RIGHT()

### Problem 1
Extract the employee number from Employee_Code.

### Problem 2
Extract the last 3 characters of Employee_ID.

### Problem 3
Extract the email extension.

### Problem 4
Extract the last name from Full_Name.

### Problem 5
Extract the joining year from Employee_Code.

### Problem 6
Extract the last 5 characters from Remarks.

---

# MID()

### Problem 1
Extract the joining year from Employee_Code.

### Problem 2
Extract the middle 3 characters from Employee_ID.

### Problem 3
Extract the username from Email.

### Problem 4
Extract the department code from Employee_Code.

### Problem 5
Extract the word "Support" from the Department.

### Problem 6
Extract the word "Improvement" from Remarks.

---

# LEN()

### Problem 1
Count the number of characters in Full_Name.

### Problem 2
Find employees whose name length is greater than 12 characters.

### Problem 3
Count the number of characters in Email.

### Problem 4
Count the number of characters in Remarks.

### Problem 5
Find the department with the longest name.

### Problem 6
Count the number of characters before applying TRIM().

---

# TRIM()

### Problem 1
Remove unnecessary spaces from Full_Name.

### Problem 2
Compare character count before and after TRIM().

### Problem 3
Create a cleaned employee name list.

### Problem 4
Identify employees whose names contained extra spaces.

### Problem 5
Standardize the Full_Name column.

---

# UPPER(), LOWER(), PROPER()

### Problem 1
Convert all employee names to uppercase.

### Problem 2
Convert all employee names to lowercase.

### Problem 3
Convert all employee names to Proper Case.

### Problem 4
Convert Department names to uppercase.

### Problem 5
Convert email usernames to lowercase.

### Problem 6
Standardize employee names using TRIM() and PROPER().

---

# SEARCH() / FIND()

### Problem 1
Find the position of '@' in Email.

### Problem 2
Find the position of '-' in Employee_Code.

### Problem 3
Determine whether "Data" exists in Department.

### Problem 4
Find the position of "Performer" in Remarks.

### Problem 5
Find the position of "Support" in Department.

### Problem 6
Find the first occurrence of the letter 'a' in Full_Name.

---

# SUBSTITUTE()

### Problem 1
Replace ".com" with ".in" in Email.

### Problem 2
Replace spaces with underscores in Full_Name.

### Problem 3
Replace "Performer" with "Employee" in Remarks.

### Problem 4
Replace "-" with "/" in Employee_Code.

### Problem 5
Replace "Data" with "Business" in Department.

### Problem 6
Replace "Work From Home" with "Remote".

---

# CONCAT(), TEXTJOIN(), &

### Problem 1
Create a display name in the format:

Employee_ID - Full_Name

### Problem 2
Create:

Full_Name (Department)

### Problem 3
Create an email signature containing:

- Regards,
- Employee Name
- Department

### Problem 4
Combine:

City - Department

### Problem 5
Create:

Employee_ID | Full_Name | City

### Problem 6
Create a complete employee profile using TEXTJOIN().

---

# 🎯 Goal

Complete all practice problems without referring to external solutions. Focus on understanding when and why each text function is used in real-world data cleaning and preparation tasks.
