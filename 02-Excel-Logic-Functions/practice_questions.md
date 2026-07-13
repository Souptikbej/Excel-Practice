# Excel Logic Functions Practice (Industry-Based)

> **Module:** Logic Functions (IF, AND, OR, NOT, Nested IF, IFS, SWITCH)
>
> **Difficulty:** Beginner → Intermediate
>
> **Dataset:** Retail Sales Operations Dataset (1000 Rows)
>
> **Goal:** Solve real-world business problems using Excel Logic Functions just like a Data Analyst working in a company.

---

# 📖 Scenario

You have joined a retail company as a **Junior Data Analyst**.

Every day, the Operations Team shares sales data with you. Your responsibility is to analyze the data and create calculated columns that help different departments make business decisions.

**Rules**

- ❌ Do NOT modify existing columns.
- ✅ Create new calculated columns.
- ✅ Use Excel formulas only.
- ✅ Try solving without searching for formulas first.

---

# Dataset Columns

| Column |
|---------|
| Order_ID |
| Order_Date |
| Customer_Name |
| Customer_Type |
| Region |
| Salesperson |
| Product |
| Category |
| Quantity |
| Unit_Price |
| Discount_% |
| Sales |
| Profit |
| Stock_Available |
| Delivery_Days |
| Payment_Mode |
| Returned |
| Customer_Rating |
| Target |
| Actual_Sales |

---

# Part 1 — IF Function

## Problem 1 — Profit Status

Create a column named **Profit_Status**.

Business Requirement:

- If Profit is greater than 0 → "Profitable"
- Otherwise → "Loss"

---

## Problem 2 — Order Value

Create a column named **Order_Value**.

Business Requirement:

- Sales greater than ₹50,000 → "High Value"
- Otherwise → "Normal"

---

## Problem 3 — Stock Status

Create a column named **Stock_Status**.

Business Requirement:

- Stock_Available = 0 → "Out of Stock"
- Otherwise → "Available"

---

## Problem 4 — Delivery Performance

Create a column named **Delivery_Status**.

Business Requirement:

- Delivery_Days > 7 → "Late Delivery"
- Otherwise → "On Time"

---

## Problem 5 — Return Investigation

Create a column named **Investigation_Status**.

Business Requirement:

- Returned = Yes → "Needs Investigation"
- Otherwise → "Closed"

---

## Problem 6 — Customer Experience

Create a column named **Customer_Experience**.

Business Requirement:

- Rating ≤ 2 → "Bad Experience"
- Otherwise → "Satisfied"

---

## Problem 7 — Target Achievement

Create a column named **Target_Status**.

Business Requirement:

- Actual_Sales ≥ Target → "Target Achieved"
- Otherwise → "Target Missed"

---

# Part 2 — AND Function

## Problem 8 — Excellent Order

Create **Excellent_Order**.

Conditions:

- Profit > 10,000
- Sales > 50,000

If both are true → "Yes"

Otherwise → "No"

---

## Problem 9 — Bonus Eligibility

Create **Bonus_Eligible**.

Conditions:

- Target Achieved
- Rating ≥ 4

---

## Problem 10 — Urgent Restocking

Create **Restock_Priority**.

Conditions:

- Stock < 10
- Sales > 50,000

---

## Problem 11 — Premium Reward

Create **Reward_Status**.

Conditions:

- Customer_Type = Premium
- Sales > 40,000

---

## Problem 12 — Successful Delivery

Create **Successful_Delivery**.

Conditions:

- Delivery ≤ 3
- Returned = No

---

# Part 3 — OR Function

## Problem 13 — High Risk Order

Create **Risk_Status**.

Conditions:

- Returned = Yes
- OR Rating ≤ 2

---

## Problem 14 — Expensive Product

Create **Premium_Product**.

Conditions:

- Category = Electronics
- OR Unit Price > ₹50,000

---

## Problem 15 — VIP Attention

Create **Priority_Customer**.

Conditions:

- Customer_Type = VIP
- OR Sales > ₹100,000

---

## Problem 16 — Promotion Candidate

Create **Promotion_Candidate**.

Conditions:

- Profit > ₹15,000
- OR Sales > ₹75,000

---

# Part 4 — NOT Function

## Problem 17 — Non Premium Customers

Create **Non_Premium**.

Requirement:

Identify customers who are NOT Premium.

---

## Problem 18 — Non Returned Orders

Create **Clean_Order**.

Requirement:

Identify orders that were NOT returned.

---

## Problem 19 — Employees Missing Target

Create **Needs_Improvement**.

Requirement:

Find employees who have NOT achieved their sales target.

---

## Problem 20 — Non Electronics Products

Create **Other_Category**.

Requirement:

Identify products that are NOT Electronics.

---

# Part 5 — Nested IF

## Problem 21 — Sales Grade

Create **Sales_Grade**.

Rules:

| Sales | Grade |
|--------|-------|
| ≥100000 | Platinum |
| ≥70000 | Gold |
| ≥40000 | Silver |
| Otherwise | Bronze |

---

## Problem 22 — Rating Category

Create **Rating_Category**.

Rules:

| Rating | Category |
|---------|----------|
| 5 | Excellent |
| 4 | Good |
| 3 | Average |
| 2 | Poor |
| 1 | Bad |

---

## Problem 23 — Delivery Speed

Create **Delivery_Speed**.

Rules:

| Days | Status |
|------|--------|
| ≤2 | Express |
| ≤5 | Fast |
| ≤7 | Normal |
| >7 | Delayed |

---

## Problem 24 — Profit Performance

Create **Profit_Category**.

Rules:

| Profit | Category |
|---------|----------|
| >30000 | Excellent |
| >15000 | Good |
| >5000 | Average |
| Otherwise | Poor |

---

## Problem 25 — Discount Recommendation

Create **Suggested_Discount**.

Rules:

| Sales | Discount |
|--------|----------|
| >100000 | 5% |
| >50000 | 10% |
| Otherwise | 15% |

---

# Part 6 — IFS Function

Rewrite the following problems using **IFS** instead of Nested IF.

- Problem 21
- Problem 22
- Problem 23
- Problem 24
- Problem 25

---

# Part 7 — SWITCH Function

## Problem 26 — Payment Code

Create **Payment_Code**.

| Payment Mode | Code |
|--------------|------|
| Cash | C |
| Card | CR |
| UPI | U |
| Net Banking | NB |

---

## Problem 27 — Regional Manager

Create **Region_Manager**.

| Region | Manager |
|---------|----------|
| East | Rahul |
| West | Amit |
| North | Priya |
| South | Karan |

---

## Problem 28 — Department

Create **Department**.

| Category | Department |
|----------|------------|
| Electronics | Tech |
| Furniture | Home |
| Office Supplies | Office |

---

## Problem 29 — Customer Level

Create **Customer_Level**.

| Customer Type | Level |
|---------------|-------|
| Regular | Level 1 |
| Premium | Level 2 |
| VIP | Level 3 |

---

## Problem 30 — Delivery Code

Create **Delivery_Code**.

| Delivery Type | Code |
|---------------|------|
| Standard | STD |
| Express | EXP |
| Same Day | SD |

---

# ⭐ Challenge Problems

## Challenge 1 — Fraud Detection

Create **Fraud_Flag**.

Conditions:

- Sales > ₹100,000
- Payment = Cash
- Returned = Yes

If all conditions are true:

> Possible Fraud

Otherwise:

> Normal

---

## Challenge 2 — Customer Loyalty

Create **Loyalty_Level**.

Rules:

VIP + Rating ≥ 4

→ VIP Loyalty

Premium + Rating ≥ 4

→ Premium Loyalty

Regular + Rating ≥ 4

→ Regular Loyalty

Otherwise

→ Needs Improvement

---

## Challenge 3 — Warehouse Alert

Create **Warehouse_Alert**.

Alert when:

- Stock < 5

OR

- Delivery > 8

OR

- Returned = Yes

---

## Challenge 4 — Sales Performance

Create **Performance_Grade**.

Rules:

| Achievement | Grade |
|------------|-------|
| ≥120% | A |
| 100–119% | B |
| 80–99% | C |
| Below 80% | D |

*(Hint: Achievement % = Actual Sales ÷ Target × 100)*

---

## Challenge 5 — Executive Dashboard Status

Create **Dashboard_Status**.

Rules:

Green

- Profit > 20,000
- Rating ≥ 4

Yellow

- Profit > 10,000

Red

- Everything Else

---

# 🎯 Final Dashboard Task

After completing all logic function problems, create the following Pivot Tables:

- Orders by Region
- Profit by Category
- Sales by Salesperson
- Returned Orders by Region
- Customer Loyalty Count
- Target Achieved vs Target Missed

Add the following Slicers:

- Region
- Customer Type
- Category

---

# 🏆 Bonus Challenge

Without looking at any tutorial or documentation, try to solve every problem using only your understanding of Excel Logic Functions.

If you get stuck:

1. Understand the business requirement.
2. Break the condition into smaller parts.
3. Write the formula.
4. Test it on one row.
5. Fill it down.

This is exactly how Data Analysts solve business problems in real-world organizations.



---
**Author:** Souptik Bej  
**Repository:** Excel Practice Series
