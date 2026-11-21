# E-Commerce Sales Data Preparation and Modeling using Power BI
📌 Project Overview

This project focuses on data preparation, transformation, cleansing, aggregation, and relationship modeling using Microsoft Power BI and Power Query Editor.

The objective is to transform raw E-commerce sales datasets into a structured, consistent, and business-ready data model that can be used for meaningful analysis and reporting.

The project involves importing multiple CSV files, handling missing and duplicate values, creating calculated columns, merging datasets, performing aggregations, and establishing relationships between tables.

📂 Dataset Description

The project uses three datasets:

1. List of Orders

Contains order-level and customer-related information.

Column Name	Description
Order ID	Unique order identifier
Order Date	Date on which the order was placed
Customer Name	Name of the customer
City	Customer's city
State	Customer's state
Category	Product category
Amount	Total order amount
Profit	Profit earned from the order
2. Order Details

Contains product-level information associated with each order.

Column Name	Description
Order ID	Order identifier
Category	Product category
Sub-Category	Product sub-category
Quantity	Number of products ordered
Amount	Sales amount
Profit	Profit earned
3. Sales Target

Contains monthly sales targets for different product categories.

Column Name	Description
Category	Product category
Month of Order Date	Month associated with the sales target
Target	Target sales amount
🛠️ Tools and Technologies
Microsoft Power BI
Power Query Editor
Power BI Data Modeling
CSV Files
Data Transformation and Cleansing
🔄 Project Tasks and Implementation

1. Data Import
Imported List of Orders.csv into Power BI.
Opened Power Query Editor using the Transform Data option.
Imported Order Details.csv and Sales Target.csv into Power Query Editor.
Verified that all three datasets were loaded successfully.

3. Row Limiting and Data Types
Restricted the List of Orders table to the first 500 rows.
Changed the Order Date column to the Date data type.
Converted Amount and Target columns to Fixed Decimal Number.
Verified the data types of the relevant columns.

4. Text Formatting
Applied Proper Case formatting to the Customer Name column.
Standardized customer names to maintain consistency and readability.
5. Column Creation

Location Column

Merged the City and State columns to create a new column named Location in the form ofCity, State

Profit Margin Column

Created a custom column named Profit Margin.

Formula: in custom column tab--> Profit/ amount in % datatype


5. Conditional Column

Created a conditional column named Profit Status based on the Profit value.

Condition	Profit Status
Profit < 0	Loss
Profit = 0	Break-Even
Profit > 0	Profit
<img width="1204" height="584" alt="Screenshot 2026-11-19 143233" src="https://github.com/user-attachments/assets/43b0da8f-96da-4548-9925-3f850bd072fc" />

6. Merging Data (Joins)
Merged the List of Orders and Order Details tables using Order ID.
Used a LEFT OUTER join operation to combine related records.
Named the merged output table Orders Data and Expanded the required columns from the merged table.
<img width="992" height="756" alt="Screenshot 2026-11-19 143923" src="https://github.com/user-attachments/assets/7e284276-df2a-4b29-a718-7a595dbb114c" />


8. Handling Missing and Duplicate Data

Missing Values:

Identified null and missing values across all three datasets.
There are no Duplicate value in these datasets.

8. Sorting and Filtering Data
Sorted the Orders Data table by Order Date in descending order.
Applied a state-level filter to analyze orders from Tamil Nadu.
Verified the filtered records to ensure accurate results.

10. Grouping and Aggregating Data

Order Details Aggregation

Created a duplicate of the Order Details table and performed the following aggregations:

Grouping	Aggregation
Order ID	Count of Order ID
Category	Average Profit
Sub-Category	Total Amount


Sales Target Aggregation

Duplicated the Sales Target table.
Grouped records by Month of Order Date.
Calculated the total Target for each month.
<img width="1095" height="622" alt="Screenshot 2026-11-19 152947" src="https://github.com/user-attachments/assets/aa78d190-ddfc-4595-8299-022e30b9731b" />

10. Data Modeling

Established relationships between the orders data and Sales target datasets in many to many relationship using Power BI's Manage Relationships feature.
<img width="1293" height="563" alt="Screenshot 2026-11-21 153011" src="https://github.com/user-attachments/assets/ec882fab-2fb2-4d0e-a993-3a2c9253f238" />



🎯 Conclusion

This project demonstrates practical data preparation and data modeling skills using Microsoft Power BI and Power Query Editor.

By performing data cleaning, transformation, merging, aggregation, and relationship modeling, raw E-commerce datasets are converted into a structured and reliable data model.

The prepared data can serve as a foundation for further business intelligence analysis, sales performance monitoring, profit analysis, and target comparison.

Technologies: Power BI | Power Query | Data Cleaning | Data Transformation | Data Modeling | CSV
