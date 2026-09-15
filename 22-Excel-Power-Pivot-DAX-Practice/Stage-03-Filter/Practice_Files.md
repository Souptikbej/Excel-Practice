# Power Pivot DAX Practice --- Stage 3: Filter Functions

## Dataset: Sales_Filter_Practice

Use this exact dataset for all questions.

  ---------------------------------------------------------------------------------------------------
    OrderID Date          Customer   Product    Category      Region       Sales    Profit   Quantity
  --------- ------------- ---------- ---------- ------------- -------- --------- --------- ----------
       1001 01-Jan-2026   Rahul      Laptop     Electronics   East         50000      8000          2

       1002 03-Jan-2026   Priya      Mouse      Electronics   West          4000      1000          5

       1003 05-Jan-2026   Amit       Chair      Furniture     South        10500      2000          3

       1004 08-Jan-2026   Sneha      Table      Furniture     North        14000      2500          2

       1005 12-Jan-2026   Raj        Monitor    Electronics   East         48000      7000          4

       1006 15-Jan-2026   Anita      Keyboard   Electronics   West          8000      1500          8

       1007 18-Jan-2026   Vikas      Sofa       Furniture     South        25000      4500          1

       1008 22-Jan-2026   Neha       Printer    Electronics   North        30000      5000          2

       1009 25-Jan-2026   Rohit      Laptop     Electronics   East         50000      9000          1

       1010 28-Jan-2026   Pooja      Cupboard   Furniture     West         36000      6500          2

       1011 02-Feb-2026   Arjun      Laptop     Electronics   East         55000      9500          2

       1012 05-Feb-2026   Kavya      Chair      Furniture     South        12000      2200          4

       1013 10-Feb-2026   Suman      Monitor    Electronics   North        52000      8000          3

       1014 15-Feb-2026   Deepak     Table      Furniture     West         16000      3000          2

       1015 20-Feb-2026   Meera      Keyboard   Electronics   East          9000      1800          6
  ---------------------------------------------------------------------------------------------------

------------------------------------------------------------------------

# Instructions

-   Create **Measures**, unless a question explicitly says otherwise.
-   Write the DAX formula, not only the numerical result.
-   Use the exact table and column names.
-   Do not change the dataset.
-   Do not add rows or columns.
-   Do not hard-code a result where a dynamic DAX measure is required.
-   Solve the questions independently before checking any solution.

------------------------------------------------------------------------

# Stage 3A --- CALCULATE()

## Q1

Calculate **Total Sales**.

## Q2

Calculate **Total Profit**.

## Q3

Calculate **Electronics Sales only**.

## Q4

Calculate **Furniture Sales only**.

## Q5

Calculate **Electronics Profit only**.

## Q6

Calculate **Sales from East region only**.

## Q7

Calculate **Sales from West region only**.

## Q8

Calculate **Profit from South region only**.

------------------------------------------------------------------------

# Stage 3B --- Multiple Filters

## Q9

Calculate sales for:

**Electronics + East**

## Q10

Calculate profit for:

**Furniture + South**

## Q11

Calculate sales for:

**Electronics + North**

## Q12

Calculate total quantity sold for:

**Electronics + East**

------------------------------------------------------------------------

# Stage 3C --- FILTER()

## Q13

Calculate total sales for orders where:

**Sales \> ₹40,000**

## Q14

Calculate total profit for orders where:

**Profit \> ₹5,000**

## Q15

Calculate total sales for orders where:

**Quantity \>= 3**

## Q16

Calculate total sales for orders where:

**Sales \> ₹30,000 AND Profit \> ₹5,000**

------------------------------------------------------------------------

# Stage 3D --- ALL() / REMOVEFILTERS()

## Q17

Create a measure that returns **Total Sales ignoring the Region
filter**.

## Q18

Create a measure that returns **Total Sales ignoring the Category
filter**.

## Q19

Create a measure that returns **Total Sales ignoring all filters from
the Sales_Filter_Practice table**.

## Q20

Create a measure that calculates:

**Current Region Sales ÷ Total Company Sales**

The denominator must **ignore the Region filter**.

The measure must remain dynamic when the selected Region changes.

------------------------------------------------------------------------

# Stage 3E --- ALLEXCEPT()

## Q21

Calculate total sales while:

**Ignoring all filters except Region.**

Use `ALLEXCEPT()` for this exercise.

------------------------------------------------------------------------

# Stage 3F --- VALUES()

## Q22

Create a measure that returns the **number of distinct regions in the
current filter context**.

Important:

-   Use `VALUES()`.
-   Do not use `DISTINCTCOUNT()` for this question.

------------------------------------------------------------------------

# Stage 3G --- SELECTEDVALUE()

## Q23

Create a measure that displays the **currently selected Region**.

When exactly one Region is selected, return the Region name.

Example:

`East`

When multiple Regions or no single Region is selected, return:

`Multiple/No Selection`

------------------------------------------------------------------------

# Stage 3H --- Business Problems

## Q24

Create a measure for:

**Electronics Sales as a percentage of Total Company Sales**

The denominator must ignore the **Category filter**.

The measure should be designed dynamically rather than being permanently
tied to one category.

## Q25

Create a measure for:

**East Region Sales as a percentage of Total Company Sales**

The denominator must ignore the **Region filter**.

For practice, make sure you understand the dynamic version of the
measure rather than simply hard-coding `East` into the numerator.

------------------------------------------------------------------------

# Self-Check Before Submission

Before submitting your answers, ask yourself:

### CALCULATE

-   Did I use `CALCULATE()` where filter context needs to change?

### FILTER

-   Is the condition row-based, such as `Sales > 40000`?

### ALL / REMOVEFILTERS

-   Am I removing the correct filter?
-   Am I removing a column filter or the whole table?

### ALLEXCEPT

-   Which filter must remain?

### VALUES

-   Am I getting distinct values from the current context?

### SELECTEDVALUE

-   What should happen when there is one selection?
-   What should happen when there are multiple/no selections?

### Percentage of Total

-   Is the numerator the current selection?
-   Does the denominator remove the intended filter?
-   Is the measure dynamic?

------------------------------------------------------------------------

# Submission Format

Submit your answers like this:

``` dax
Q1 Total Sales =
SUM(Sales_Filter_Practice[Sales])

Q2 Total Profit =
SUM(Sales_Filter_Practice[Profit])

Q3 Electronics Sales =
CALCULATE(
    [Total Sales],
    Sales_Filter_Practice[Category] = "Electronics"
)
```

Do not submit only numerical outputs. The objective of this stage is to
test your ability to write and select the correct DAX logic.
