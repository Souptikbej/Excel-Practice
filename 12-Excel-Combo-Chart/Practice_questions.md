# Practice Questions — Combo Charts & Secondary Axis

## Dataset

Use `Combo_Charts_Secondary_Axis_Practice.xlsx` for all five problems.

---

# Problem 1 — Sales vs Profit Combo Chart

### Business Requirement
Management wants to compare monthly Sales Amount and Profit.

### Task
Create a Combo Chart with:
- `Month` → X-axis
- `Sales_Amount` → Column
- `Profit` → Line

### Requirements
1. Aggregate Sales Amount by Month.
2. Aggregate Profit by Month.
3. Create a Combo Chart.
4. Use a Column for Sales.
5. Use a Line for Profit.
6. Add an appropriate chart title.
7. Add a legend.

### Expected Skill
**Basic Combo Chart — Column + Line**

### Business Question
> How does monthly profit move relative to monthly sales?

### Deliverable
- Monthly summary table
- Combo Chart
- At least one business observation

---

# Problem 2 — Sales vs Growth % Using Secondary Axis

### Business Requirement
Management wants to understand whether sales performance is associated with sales growth.

### Task
Create a Combo Chart with:
- `Sales_Amount` → Column
- `Growth_%` → Line
- `Growth_%` → Secondary Axis

### Requirements
1. Aggregate Sales Amount by Month.
2. Calculate/aggregate Growth % appropriately for the monthly view.
3. Create a Column + Line Combo Chart.
4. Place Growth % on the Secondary Axis.
5. Format the Secondary Axis as a percentage.
6. Add an appropriate chart title.

### Expected Skill
**Combo Chart + Secondary Axis + Percentage**

### Business Question
> Are periods of high sales also associated with higher growth?

### Deliverable
- Monthly summary table
- Combo Chart
- At least one business observation

---

# Problem 3 — Sales vs Orders Combo Chart

### Business Requirement
The sales team wants to understand the relationship between revenue generated and the number of orders.

### Task
Create a Combo Chart with:
- `Sales_Amount` → Column
- `Orders` → Line
- `Orders` → Secondary Axis

### Requirements
1. Group the dataset by Month.
2. Calculate total Sales Amount.
3. Calculate total Orders.
4. Create a Column + Line Combo Chart.
5. Put Orders on the Secondary Axis.
6. Add the chart title: **Monthly Sales vs Orders**

### Expected Skill
**Combo Chart + Secondary Axis**

### Business Question
> Does higher sales always mean a higher number of orders?

### Deliverable
- Monthly summary table
- Combo Chart
- At least one business observation

---

# Problem 4 — Profit vs Profit Margin Analysis

### Business Requirement
Management wants to compare absolute profit with profitability percentage.

### Task
Create a Combo Chart with:
- `Profit` → Column
- `Profit_Margin_%` → Line
- `Profit_Margin_%` → Secondary Axis

### Requirements
1. Aggregate Profit by Month.
2. Aggregate Sales Amount by Month.
3. Calculate monthly Profit Margin using:

```text
Profit Margin % = Total Profit / Total Sales × 100
```

4. Create a Column + Line Combo Chart.
5. Put Profit Margin % on the Secondary Axis.
6. Format the Secondary Axis as a percentage.
7. Add data labels to the Profit Margin line where appropriate.
8. Use the title: **Monthly Profit vs Profit Margin**

### Important
Do not simply average row-level `Profit_Margin_%` values for this business-level monthly analysis.

### Expected Skill
**Financial KPI Combo Chart + Secondary Axis**

### Business Question
> Is the company generating higher profit because of higher sales, or because of better margins?

### Deliverable
- Monthly summary table
- Profit Margin calculation
- Combo Chart
- At least two business observations
- Final business conclusion

---

# Problem 5 — Regional Performance Combo Chart

### Business Requirement
Management wants to compare sales and profit performance across regions.

### Task
Create a regional summary using:
- `Region`
- `Sales_Amount`
- `Profit`

Create a Combo Chart with:
- `Sales_Amount` → Column
- `Profit` → Line
- `Profit` → Secondary Axis

### Requirements
1. Group the dataset by Region.
2. Calculate total Sales Amount for each region.
3. Calculate total Profit for each region.
4. Sort regions from highest Sales to lowest Sales.
5. Create a Column + Line Combo Chart.
6. Put Profit on the Secondary Axis.
7. Exclude Grand Total from the chart.
8. Add an appropriate chart title.

### Expected Skill
**Regional Aggregation + Combo Chart + Secondary Axis**

### Business Question
> Which region generates the highest sales, and does that region also generate the highest profit?

### Deliverable
- Regional summary table
- Sorted regional data
- Combo Chart
- Business conclusion

---

# Analyst Challenge — Interpretation

For every problem, do not stop at creating the chart.

Use this structure:

```text
Observation:
[What does the chart show?]

Business Insight:
[Why does this matter to management?]
```

Example:

```text
Observation:
North has the highest regional sales.

Business Insight:
North is currently the strongest region by absolute sales and also
generates the highest absolute profit.
```

---

# Final Submission Checklist

## Problem 1
- [ ] Monthly Sales summary
- [ ] Monthly Profit summary
- [ ] Column + Line Combo Chart
- [ ] Business observation

## Problem 2
- [ ] Monthly Sales summary
- [ ] Growth %
- [ ] Column + Line Combo Chart
- [ ] Secondary Axis
- [ ] Percentage formatting
- [ ] Business observation

## Problem 3
- [ ] Monthly Sales summary
- [ ] Monthly Orders summary
- [ ] Column + Line Combo Chart
- [ ] Secondary Axis
- [ ] Business observation

## Problem 4
- [ ] Monthly Sales summary
- [ ] Monthly Profit summary
- [ ] Profit Margin calculation
- [ ] Column + Line Combo Chart
- [ ] Secondary Axis
- [ ] Percentage formatting
- [ ] Business conclusion

## Problem 5
- [ ] Regional Sales summary
- [ ] Regional Profit summary
- [ ] Sorted highest → lowest Sales
- [ ] Column + Line Combo Chart
- [ ] Secondary Axis
- [ ] Grand Total excluded
- [ ] Business conclusion

---

# Skills Covered

| Skill | Problem 1 | Problem 2 | Problem 3 | Problem 4 | Problem 5 |
|---|:---:|:---:|:---:|:---:|:---:|
| PivotTable | ✓ | ✓ | ✓ | ✓ | ✓ |
| Aggregation | ✓ | ✓ | ✓ | ✓ | ✓ |
| Combo Chart | ✓ | ✓ | ✓ | ✓ | ✓ |
| Column + Line | ✓ | ✓ | ✓ | ✓ | ✓ |
| Secondary Axis | — | ✓ | ✓ | ✓ | ✓ |
| Percentage Analysis | — | ✓ | — | ✓ | — |
| Business Interpretation | ✓ | ✓ | ✓ | ✓ | ✓ |
| Regional Analysis | — | — | — | — | ✓ |
