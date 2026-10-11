📊 Power BI Assignment – E-commerce Sales Data Modeling
📖 Project Overview
This project demonstrates data preparation, transformation, and modeling using Power BI and Power Query Editor.
The dataset represents an E-commerce sales system, containing order-level, product-level, and sales target information.
The goal is to ensure consistency, accuracy, and business relevance of the prepared data model for analysis and reporting.

📁 Dataset Description
The project uses three datasets:

Dataset	Attributes
List of Orders	Order ID, Order Date, Customer Name, City, State, Category, Amount, Profit
Order Details	Order ID, Category, Sub-Category, Quantity, Amount, Profit
Sales Target	Category, Month of Order Date, Target


🛠️ Tasks Performed
1. Data Import
Imported List of Orders.csv, Order Details.csv, and Sales Target.csv into Power BI.

Used Power Query Editor for transformations.

2. Row Limiting & Data Types
Restricted List of Orders to the first 500 rows.

Converted Order Date column to Date type.

Changed Amount and Target columns to Fixed Decimal Numbers.

3. Text Formatting
Applied Proper Case to the CustomerName column for consistent capitalization.

4. Column Creation
Merged City + State into a new column Location (City, State).

Created a Profit Margin column:

Profit Margin
=
Profit
Amount
×
100
5. Conditional Column
Added Profit Status:

Profit < 0 → Loss

Profit = 0 → Break-Even

Profit > 0 → Profit

6. Merging Data
Merged List of Orders and Order Details using Order ID.

Named the merged output table Orders Data.

7. Handling Missing & Duplicate Data
Identified missing values across tables.

Applied strategies: replacing, removing, or retaining nulls with justification.

Detected and handled duplicate rows based on business logic.

8. Sorting & Filtering
Sorted Orders Data by Order Date (descending).

Applied filters to analyze orders from specific states (e.g., Tamil Nadu).

9. Grouping & Aggregation
Duplicated Order Details to perform:

Count of Order ID

Average Profit by Category

Total Amount by Sub-Category

Duplicated Sales Target to aggregate Total Target by Month.

10. Data Modeling
Established relationships:

List of Orders ↔ Order Details (Order ID)

Order Details ↔ Sales Target (Category)

Verified relationships using Manage Relationships.

🎯 Key Learning Outcomes
Hands-on experience with Power Query transformations.

Skills in data cleansing, formatting, and enrichment.

Ability to merge, aggregate, and model datasets.

Improved understanding of business-ready data models in Power BI.

🧩 Tools Used
Power BI Desktop

Power Query Editor

Functions: TransformColumnTypes, Text.Proper, Merge Queries, Group By, Conditional Column

Features: Data Modeling, Manage Relationships, Sorting & Filtering

🚀 Future Enhancements
Automate transformations with Power Query Parameters.

Build interactive dashboards for sales performance vs. targets.

Extend analysis with DAX measures (e.g., cumulative profit, YoY growth).
