# Excel Data Analysis Practice — Combo Charts & Secondary Axis

## Overview
This practice set is designed for entry-level Data Analysts to practice Excel charting techniques used in real-world business reporting.

**Topic:** Combo Charts & Secondary Axis  
**Problems:** 5  
**Dataset:** One common dataset for all problems

**Business scenario:** You are a Data Analyst at a consumer electronics company. Management wants to analyze sales, profit, growth, order volume, profitability, and regional performance.

## Files

| File | Description |
|---|---|
| `Combo_Charts_Secondary_Axis_Practice.xlsx` | Excel workbook containing the practice dataset |
| `Combo_Charts_Secondary_Axis_Dataset.csv` | CSV version of the dataset |
| `README.md` | Overview, objectives, and instructions |
| `Practice_questions.md` | Five practice problems |

## Dataset

The dataset contains monthly performance data for three products across four regions during 2025.

| Column | Description |
|---|---|
| `Month` | Reporting month |
| `Region` | Sales region |
| `Product` | Product category |
| `Sales_Amount` | Total sales amount |
| `Profit` | Total profit |
| `Units_Sold` | Number of units sold |
| `Growth_%` | Sales growth percentage |
| `Orders` | Number of orders |
| `Profit_Margin_%` | Profit as a percentage of sales |

**Data size:** 48 records × 9 columns  
**Period:** January 2025 – December 2025  
**Regions:** North, South, East, West  
**Products:** Laptop, Mobile, Tablet

## Learning Objectives

By completing this practice set, you should be able to:

- Create PivotTables for business summaries.
- Aggregate sales and profit by month and region.
- Create Combo Charts.
- Combine Column and Line charts.
- Use a Secondary Axis when two measures have different scales.
- Format percentage measures correctly.
- Sort summarized data.
- Exclude Grand Total from charts when appropriate.
- Interpret charts from a business perspective.
- Write concise, data-driven business insights.

## Key Concepts

### Combo Chart
A Combo Chart combines two chart types, commonly Column + Line.

Example:
- Sales → Column
- Profit → Line

### Secondary Axis
Use a Secondary Axis when two measures have substantially different scales or units.

Example:
- Profit → ₹ values
- Profit Margin → % values

## Recommended Workflow

```text
Raw Dataset
    ↓
PivotTable / Summary
    ↓
Aggregate Required Measures
    ↓
Create Chart
    ↓
Select Column + Line
    ↓
Apply Secondary Axis Where Required
    ↓
Format Chart
    ↓
Interpret Business Insight
```

## Important Analytical Rule

For monthly Profit Margin analysis:

```text
Profit Margin % = Total Profit / Total Sales × 100
```

Do not simply average row-level profit margins when the question asks for an overall monthly margin.

## Practice Rules

1. Try solving each problem independently.
2. Use the same dataset for all five problems.
3. Do not include Grand Total in charts unless specifically requested.
4. Check whether a Secondary Axis is appropriate.
5. After every chart, write at least one business observation.
6. Focus on data-analysis operations rather than decorative Excel features.

## Completion Checklist

- [ ] Problem 1 — Sales vs Profit Combo Chart
- [ ] Problem 2 — Sales vs Growth % with Secondary Axis
- [ ] Problem 3 — Sales vs Orders with Secondary Axis
- [ ] Problem 4 — Profit vs Profit Margin % with Secondary Axis
- [ ] Problem 5 — Regional Sales vs Profit with Secondary Axis

## Expected Analyst Mindset

Do not stop after creating a chart. Ask:

- What changed?
- Which period or region performed best?
- Which performed worst?
- Is higher profit caused by higher sales or better margins?
- Does the relationship between the measures make business sense?
- What action could management take based on the result?

The goal is:

**Excel Chart → Analysis → Business Insight**

## Skills Practiced

**Excel:** PivotTables, aggregation, Combo Charts, Secondary Axis, percentage formatting, sorting, chart interpretation, business insights.

**Data Analysis:** trend comparison, KPI comparison, regional performance analysis, profitability analysis, scale comparison.

## Status

**Topic:** Combo Charts & Secondary Axis  
**Problems:** 5  
**Status:** Completed
