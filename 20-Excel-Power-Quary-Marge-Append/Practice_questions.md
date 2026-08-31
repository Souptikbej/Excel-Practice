# Practice Questions

## 1. Merge Queries

### Sales

|OrderID|CustomerID|Product|Quantity|UnitPrice|
|---|---|---|---:|---:|
|1001|C001|Laptop|2|55000|
|1002|C003|Mouse|5|700|
|1003|C002|Keyboard|3|1200|
|1004|C005|Monitor|1|15000|
|1005|C004|Printer|2|9000|
|1006|C006|Webcam|4|2500|

### Customers

|CustomerID|CustomerName|City|Membership|
|---|---|---|---|
|C001|Rahul Sharma|Delhi|Gold|
|C002|Sneha Das|Kolkata|Silver|
|C003|Amit Roy|Mumbai|Gold|
|C004|Priya Singh|Pune|Bronze|
|C005|Rohan Mehta|Hyderabad|Silver|

### Tasks
1. Merge using **CustomerID**.
2. Use **Left Outer Join**.
3. Expand **CustomerName**, **City**, **Membership**.
4. Create **SalesAmount = Quantity × UnitPrice**.
5. Identify the order without a matching customer.

---

## 2. Append Queries

### Sales_January

|OrderID|Date|Product|Amount|
|---|---|---|---:|
|2001|05-Jan|Laptop|65000|
|2002|09-Jan|Mouse|1800|
|2003|15-Jan|Keyboard|3200|
|2004|22-Jan|Monitor|14000|

### Sales_February

|OrderID|Date|Product|Amount|
|---|---|---|---:|
|2005|03-Feb|Printer|17000|
|2006|10-Feb|Laptop|62000|
|2007|18-Feb|Webcam|8500|
|2008|27-Feb|Mouse|2200|

### Tasks
1. Append both tables.
2. Count total rows.
3. Sort by **Date** (Ascending).
4. Filter **Amount > 10000**.
5. Calculate total sales amount.
