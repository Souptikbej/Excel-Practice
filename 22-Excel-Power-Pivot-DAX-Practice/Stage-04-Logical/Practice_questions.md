# Stage 4 — Practice Questions

## Dataset: Employee_Performance

Use the following dataset for all 25 questions.

| EmpID | Employee | Department | Sales | Target | Profit | Attendance% | ExperienceYears | Rating |
|---:|---|---|---:|---:|---:|---:|---:|---:|
| 101 | Rahul | Sales | 120000 | 100000 | 18000 | 96 | 3 | 4 |
| 102 | Priya | Sales | 85000 | 100000 | 12000 | 91 | 2 | 3 |
| 103 | Amit | Finance | 95000 | 90000 | 15000 | 88 | 5 | 4 |
| 104 | Sneha | IT | 140000 | 120000 | 25000 | 97 | 4 | 5 |
| 105 | Vikas | Marketing | 75000 | 80000 | 9000 | 82 | 1 | 2 |
| 106 | Neha | Sales | 110000 | 100000 | 16000 | 94 | 3 | 4 |
| 107 | Anita | IT | 105000 | 120000 | 14000 | 90 | 6 | 3 |
| 108 | Raj | Finance | 125000 | 110000 | 22000 | 95 | 7 | 5 |
| 109 | Pooja | HR | 68000 | 70000 | 7000 | 86 | 2 | 3 |
| 110 | Rohit | Marketing | 92000 | 80000 | 13000 | 93 | 4 | 4 |
| 111 | Arjun | Sales | 155000 | 130000 | 28000 | 98 | 8 | 5 |
| 112 | Kavya | Finance | 78000 | 90000 | 10000 | 89 | 3 | 3 |
| 113 | Suman | IT | 130000 | 120000 | 21000 | 96 | 5 | 4 |
| 114 | Deepak | HR | 82000 | 70000 | 11000 | 92 | 6 | 4 |
| 115 | Meera | Marketing | 115000 | 100000 | 19000 | 95 | 5 | 5 |

---

# Part A — IF()

### Q1
Create a calculated column:

- If `Sales >= Target` → `Achieved`
- Otherwise → `Not Achieved`

### Q2
Create a calculated column:

- If `Profit >= 15000` → `Profitable`
- Otherwise → `Low Profit`

### Q3
Create a calculated column:

- If `Attendance% >= 90` → `Good Attendance`
- Otherwise → `Low Attendance`

### Q4
Create a calculated column:

- If `Rating >= 4` → `Good`
- Otherwise → `Needs Improvement`

---

# Part B — IF with Business Conditions

### Q5
Create a calculated column:

- If `Sales >= Target` → `Bonus Eligible`
- Otherwise → `Not Eligible`

### Q6
Create a calculated column:

- If `Sales >= Target` AND `Profit >= 15000` → `High Performer`
- Otherwise → `Regular Performer`

---

# Part C — AND()

### Q7
Create a calculated column:

- If `Sales >= Target`
- AND `Attendance% >= 95`
- AND `Rating >= 4`

Return `Excellent`.

Otherwise return `Not Excellent`.

### Q8
Create a calculated column:

- If `ExperienceYears >= 5`
- AND `Rating >= 4`
- AND `Attendance% >= 90`

Return `Promotion Eligible`.

Otherwise return `Not Eligible`.

---

# Part D — OR()

### Q9
Create a calculated column:

- If `Sales >= 130000`
- OR `Rating = 5`

Return `Special Recognition`.

Otherwise return `Normal`.

### Q10
Create a calculated column:

- If `Attendance% < 85`
- OR `Rating <= 2`

Return `Management Attention`.

Otherwise return `No Immediate Concern`.

---

# Part E — NOT()

### Q11
Create a calculated column:

If the employee has **NOT achieved the target**, return:

`Follow Up`

Otherwise:

`On Track`

### Q12
Create a calculated column:

If the employee is **NOT from Sales**, return:

`Non-Sales`

Otherwise:

`Sales`

---

# Part F — SWITCH()

### Q13
Create a calculated column called `Performance Rating Category`.

Use `SWITCH()`:

| Rating | Category |
|---:|---|
| 5 | Excellent |
| 4 | Good |
| 3 | Average |
| 2 | Poor |
| 1 | Very Poor |

### Q14
Create a calculated column called `Sales Performance Band`.

Use `SWITCH(TRUE())`:

- `Sales >= 130000` → `Excellent`
- `Sales >= 100000` → `Good`
- `Sales >= 80000` → `Average`
- Below `80000` → `Low`

### Q15
Create a calculated column called `Attendance Category`.

Use `SWITCH(TRUE())`:

- `Attendance% >= 95` → `Excellent`
- `Attendance% >= 90` → `Good`
- `Attendance% >= 85` → `Average`
- Below `85` → `Poor`

---

# Part G — Combined Business Logic

### Q16
Create a calculated column:

If:

- `Sales >= Target`
- AND `Profit >= 20000`
- AND `Rating >= 4`

Return:

`High Performer`

Otherwise:

`Normal Performer`

### Q17
Create a calculated column called `Bonus Category`.

Use `SWITCH(TRUE())`:

**High Bonus**
- `Sales >= Target`
- AND `Profit >= 20000`
- AND `Attendance% >= 95`

**Standard Bonus**
- `Sales >= Target`
- AND `Profit >= 15000`

**No Bonus**
- Otherwise

### Q18
Create a calculated column called `Employee Risk Status`.

Use `SWITCH(TRUE())`:

**High Risk**
- `Attendance% < 85`
- OR `Rating <= 2`

**Medium Risk**
- `Attendance% < 90`
- OR `Rating = 3`

**Low Risk**
- Otherwise

Remember: **condition order matters**.

---

# Part H — IFERROR()

### Q19
Create a calculated column:

`Target Achievement % = Sales / Target × 100`

Use `IFERROR()` so that a zero Target does not produce an error.

### Q20
Create a calculated column:

`Profit Margin % = Profit / Sales × 100`

Use `IFERROR()`.

---

# Part I — Real Business Problems

### Q21
Create a calculated column:

- If `Sales > Target` → `Exceeded`
- Otherwise → `Did Not Exceed`

**Important:** Use strict `>`.

### Q22
Create a calculated column:

If:

- `Rating <= 2`
- OR `Attendance% < 85`

Return:

`Needs Improvement`

Otherwise:

`Satisfactory`

### Q23
Create a calculated column called `Sales Classification`.

Use `SWITCH(TRUE())`:

- `Sales >= 130000` → `Tier 1`
- `Sales >= 100000` → `Tier 2`
- `Sales >= 80000` → `Tier 3`
- Below `80000` → `Tier 4`

### Q24
Create a calculated column called `Overall Employee Status`.

Use the following business rules **in this order**:

**Top Performer**
- `Sales >= Target`
- AND `Profit >= 20000`
- AND `Rating >= 4`
- AND `Attendance% >= 95`

**Good Performer**
- `Sales >= Target`
- AND `Rating >= 4`

**Needs Attention**
- `Sales < Target`
- OR `Rating <= 2`

**Average**
- Otherwise

### Q25
Create a calculated column called `Employee Classification`.

Use `SWITCH(TRUE())` and the following order:

**Star Performer**
- `Sales >= Target`
- AND `Profit >= 20000`
- AND `Rating >= 4`
- AND `Attendance% >= 95`

**Potential Performer**
- `Sales >= Target`
- AND `Rating >= 4`

**Needs Support**
- `Sales < Target`
- AND `Rating <= 3`

**Attendance Concern**
- `Attendance% < 85`

**Regular Performer**
- Otherwise

---

# Submission Format

For review, submit your **25 DAX formulas** in order:

```text
Q1: [DAX formula]
Q2: [DAX formula]
Q3: [DAX formula]
...
Q25: [DAX formula]
```

The formulas will be checked for:

- Correct syntax
- Correct function
- Correct conditions
- Correct operators
- Correct output labels
- Correct `SWITCH(TRUE())` order
- Correct business logic
