# 📘 Excel IFERROR & IFNA Practice

A beginner-friendly repository to practice **IFERROR** and **IFNA** in Microsoft Excel.

This repository is designed for learners who have completed basic Excel formulas but **have not yet learned Lookup functions (VLOOKUP, XLOOKUP, INDEX-MATCH)**.

---

## 📖 About

When working with real-world datasets, formulas often return errors.

Instead of displaying confusing Excel errors like:

- #DIV/0!
- #VALUE!
- #N/A

you can handle them professionally using:

- ✅ IFERROR
- ✅ IFNA

Learning these functions makes your dashboards and reports much cleaner and more user-friendly.

---

# 📚 Topics Covered

- Understanding Excel Errors
- IFERROR Function
- IFNA Function
- Handling Division Errors
- Handling Text Extraction Errors
- Working with Invalid Data
- Real Business Examples
- Practice Exercises

---

# 🎯 Learning Objectives

After completing this repository, you will be able to:

- Identify common Excel errors
- Use IFERROR to replace error messages
- Understand when IFNA should be used
- Build cleaner Excel reports
- Prepare for Lookup functions

---

# 📌 Functions Used

- IFERROR
- IFNA

---

# 💡 Common Excel Errors

| Error | Meaning |
|--------|----------|
| #DIV/0! | Division by zero |
| #VALUE! | Invalid data type |
| #N/A | Value not available |
| #NAME? | Formula name not recognized |
| #REF! | Invalid cell reference |
| #NUM! | Invalid numeric value |

---

# 🧠 IFERROR Syntax

```excel
=IFERROR(value, value_if_error)
```

Example:

```excel
=IFERROR(A2/B2,"No Sales")
```

---

# 🧠 IFNA Syntax

```excel
=IFNA(value, value_if_na)
```

Example:

```excel
=IFNA(A2,"Not Found")
```

---

# 📈 Real-World Use Cases

- Sales Reports
- HR Dashboards
- Inventory Reports
- Finance Dashboards
- Customer Data Cleaning
- Email Validation
- KPI Calculations

---

# ⚠️ Difference Between IFERROR and IFNA

| IFERROR | IFNA |
|----------|------|
| Handles all Excel errors | Handles only #N/A |
| Most commonly used | Mostly used with Lookup functions |

---

Those functions commonly generate **#N/A**, making **IFNA** much more useful.

---

## ⭐ If you found this repository helpful, consider giving it a star!
