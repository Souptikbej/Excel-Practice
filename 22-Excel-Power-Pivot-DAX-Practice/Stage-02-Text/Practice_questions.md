# DAX Stage 2 — Practice Questions

## Dataset

Use the `Employee_Master` table from `README.md`.

Columns:

`EmpID`, `Employee Name`, `Email`, `Department`, `City`, `Employee Code`, `Mobile`

---

# Part A — Basic Text Extraction

### Q1. Employee Code Prefix
Create a calculated column that extracts the first **3 characters** from `Employee Code`.

**Example:** `EMP-1001` → `EMP`

---

### Q2. Mobile Last 4 Digits
Create a calculated column that extracts the last **4 digits** from `Mobile`.

**Example:** `9876543210` → `3210`

---

### Q3. First Name
Create a calculated column that extracts the employee's **first name** from `Employee Name`.

**Example:** `Rahul Sharma` → `Rahul`

---

### Q4. Last Name
Create a calculated column that extracts the employee's **last name** from `Employee Name`.

**Example:** `Rahul Sharma` → `Sharma`

---

### Q5. Employee Name Length
Create a calculated column that counts the number of characters in `Employee Name`.

**Example:** `Rahul Sharma` → `12`

> Count spaces as characters.

---

# Part B — Text Standardization

### Q6. Uppercase Name
Convert `Employee Name` into **UPPERCASE**.

**Example:** `Rahul Sharma` → `RAHUL SHARMA`

---

### Q7. Lowercase Name
Convert `Employee Name` into **lowercase**.

**Example:** `Rahul Sharma` → `rahul sharma`

---

### Q8. Space Validation
Check whether `Employee Name` contains a space.

Return:

- `Yes` if a space exists
- `No` if a space does not exist

---

### Q9. Remove Extra Spaces
Use a DAX text function to clean unnecessary leading, trailing, or repeated spaces from `Employee Name`.

---

# Part C — Replace and Modify Text

### Q10. Department Replacement
Replace `Sales` with `Business Development` in the `Department` column.

**Example:** `Sales` → `Business Development`

Other departments should remain unchanged.

---

### Q11. Employee Name + Department
Create:

`Employee Name - Department`

**Example:**

`Rahul Sharma - Sales`

---

### Q12. Employee Name + Department + City
Create:

`Employee Name - Department - City`

**Example:**

`Rahul Sharma - Sales - Kolkata`

---

### Q13. Remove Hyphen from Employee Code
Remove `-` from `Employee Code`.

**Example:**

`EMP-1001` → `EMP1001`

---

# Part D — Email Analysis

### Q14. Position of @
Find the **position of `@`** in the `Email` column.

**Example:**

`rahul.sharma@abc.com`

Return the character position of `@`.

> Do not return the position after `@`.

---

### Q15. Email Username
Extract the username from `Email`.

**Example:**

`rahul.sharma@abc.com` → `rahul.sharma`

---

### Q16. Email Domain
Extract the domain from `Email`.

**Example:**

`rahul.sharma@abc.com` → `abc.com`

---

### Q17. Mask Mobile Number
Create a masked mobile number where the first **6 digits** are replaced by `XXXXXX`.

**Example:**

`9876543210` → `XXXXXX3210`

---

# Part E — Business-Oriented Text Columns

### Q18. Login ID
Create a Login ID using:

`first name.last name`

Convert the result to lowercase.

**Example:**

`Rahul Sharma` → `rahul.sharma`

> Do not use the Email column for this question.

---

### Q19. Email Signature
Create:

`Employee Name | Department | ABC Pvt Ltd`

**Example:**

`Rahul Sharma | Sales | ABC Pvt Ltd`

---

### Q20. Company Email Validation
Check whether the employee's email belongs to the domain:

`abc.com`

Return:

- `Yes`
- `No`

---

### Q21. Employee Code Validation
Check whether `Employee Code` starts with `EMP`.

Return:

- `Valid`
- `Invalid`

---

### Q22. Mobile Validation
Check whether `Mobile` contains exactly **10 digits**.

Return:

- `Valid`
- `Invalid`

> Treat `Mobile` as a Text field.

---

### Q23. Numeric Part of Employee Code
Extract the numeric portion from `Employee Code`.

**Example:**

`EMP-1001` → `1001`

> For this Text Functions exercise, returning `1001` as text is acceptable.

---

### Q24. Employee Initials
Create employee initials using the first letter of the first name and the first letter of the last name.

**Example:**

`Rahul Sharma` → `RS`

The result should be uppercase.

---

### Q25. Employee Label
Create:

`Employee Code | Employee Name`

**Example:**

`EMP-1001 | Rahul Sharma`

---

# Part F — Additional DAX Text Functions

### Q26. REPT — Employee Rating Indicator
Create a text indicator using `REPT()`.

Requirement:

- If Department is `Sales`, return `***`
- If Department is `HR`, return `**`
- For other departments, return `*`

The purpose is to practice dynamically repeating text with `REPT()`.

---

### Q27. EXACT — Case-Sensitive Department Check
Use `EXACT()` to check whether `Department` is exactly:

`Sales`

Return:

- `TRUE`
- `FALSE`

> `EXACT()` is case-sensitive.

---

### Q28. FORMAT — Employee ID Display
Create a display version of `EmpID` using `FORMAT()` so that every ID contains **5 digits**.

Examples:

- `101` → `00101`
- `102` → `00102`
- `110` → `00110`

> Remember: `FORMAT()` returns text.

---

# Submission Format

For every question, submit:

```text
Q1
Formula:
Result:

Q2
Formula:
Result:

...

Q28
Formula:
Result:
```

You can submit your answers as:

- PDF
- DOCX
- Excel
- Screenshot
- Plain text

---

# Important Restrictions

Do **not** use:

- `PROPER()` — it is not a DAX function.
- Columns that do not exist in the supplied dataset unless you explicitly create them first.

For Q18 and Q24, derive the required information from the original `Employee Name` column.

---

# Target

**28 questions total**

Recommended completion target:

**90%+ correct**

After submission, each formula should be checked individually for:

1. Correct DAX syntax
2. Correct function selection
3. Correct source column
4. Correct output
5. Business appropriateness
6. Data type
