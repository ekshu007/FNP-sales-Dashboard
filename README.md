📌 Project Overview

This project is an Excel-based Sales Analytics Dashboard developed for FNP (Ferns N Petals). It analyzes sales performance using real-world–style transactional data and presents insights through Pivot Tables, Pivot Charts, and slicers.
The project demonstrates how raw data from multiple sources can be modeled using a Star Schema and transformed into a meaningful business dashboard using Microsoft Excel.

📂 Dataset Description
The dashboard is built using three datasets, stored as separate files and integrated into Excel.

1️⃣ Orders Dataset (Fact Table) – orders.csv
Contains transactional sales data and serves as the central fact table.
Key Columns:
Order_ID
Customer_ID
Product_ID
Quantity
Order_Date, Order_Time
Delivery_Date, Delivery_Time
Location
Occasion
Role:
Stores measurable business events such as order count and quantity sold.

2️⃣ Customers Dataset (Dimension Table) – customers.csv

Contains descriptive information about customers.

Key Columns:

Customer_ID
Name
Gender
City
Contact_Number
Email
Address
Role:
Used for customer segmentation and geographic analysis.

3️⃣ Products Dataset (Dimension Table) – products.csv
Contains product-related details.
Key Columns:
Product_ID
Product_Name
Category
Price (INR)
Occasion
Role:
Used to analyze product performance, category trends, and revenue contribution.

⭐ Data Model – Star Schema Design
This project follows a Star Schema, a standard data modeling approach used in data warehousing and business intelligence.

🧮 Fact Table
Orders
Stores quantitative measures:
Order Count
Quantity Sold
Revenue (calculated as Quantity × Price)
Contains foreign keys linking to dimension tables.

📐 Dimension Tables
Customers – customer attributes (city, gender, etc.)
Products – product attributes (category, price, occasion)
🔗 Relationships
Orders.Customer_ID → Customers.Customer_ID
Orders.Product_ID → Products.Product_ID
This design improves analytical clarity, performance, and scalability when working with Pivot Tables.

📊 Dashboard Features
The Excel dashboard provides interactive analysis through:
📈 Total Orders and Quantity Sold
💰 Estimated Revenue
🎁 Sales by Product Category
🎉 Sales by Occasion (Birthday, Anniversary, Diwali, Valentine’s Day, etc.)
🌍 Location-wise order distribution
🕒 Time-based order trends

Interactive Controls:
Slicers for:
Occasion
Product Category
City
Date range

🧮 Pivot Table Logic
Common calculations used:
Total Orders → Count of Order_ID
Total Quantity Sold → Sum of Quantity
Revenue → Quantity × Price (INR)
Category Performance → Revenue and quantity by category
Occasion Analysis → Orders and revenue by occasion

📈 Key Insights (Sample)
Festival and special occasions drive higher sales volume.
Certain product categories (e.g., Sweets, Plants) consistently perform better.
Urban locations contribute a significant share of total orders.
Occasion-based buying behavior is clearly visible.
(Insights vary based on filters applied in the dashboard.)

🛠 Tools & Technologies Used
Microsoft Excel
Pivot Tables
Pivot Charts
Slicers
Lookup formulas (VLOOKUP / XLOOKUP)
CSV files as structured data sources

🚀 How to Use the Project

Open the Excel dashboard file.

Ensure customers.csv, orders.csv, and products.csv are properly linked or imported.

Refresh all Pivot Tables.

Use slicers to explore different sales insights.

⚠️ Assumptions & Limitations

Revenue is calculated using listed product prices only.
Discounts and returns are not considered.
Dataset is static and meant for analytical demonstration purposes.

📁 Project Structure
├── customers.csv      # Customer dimension table
├── orders.csv         # Fact table (sales transactions)
├── products.csv       # Product dimension table
├── Excel Dashboard    # Pivot tables & charts
└── README.md

Translating raw data into actionable insights

It is suitable for academic projects, internships, and data analytics portfolios.
