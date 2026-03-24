# 📂 Data Dictionary
## 📌 Overview
This document describes the structure of the dataset used in the project, including tables, columns, and their meanings.

## 🧾 Sales Data Tables (2020,2021,2022)

| Column Name | Description |
|------------|------------|
| OrderNumber | Unique identifier for each order |
| OrderDate | Date of the transaction |
| StockDate | Date the product arrived in storage |
| ProductKey | Identifier of the product |
| CustomerKey | Identifier of the customer |
| OrderQuantity | Number of items in one invoice or order |
| TerritoryKey | Code for the region (country or continent) |
| OrderLineItem | Number of lines in the invoice |

## 👥 Customer Lookup Table

| Column Name | Description |
|------------|------------|
| CustomerKey | Unique customer identifier |
| Prefix | Abbreviation of the name for the title |
| FirstName | Customer First Name |
| LastName | Customer Last Name |
| BirthDate | Customer's date of birth |
| MaritalStatus | The client's social status |
| Gender | Male or Female |
| EmailAddress | Customer email |
| AnnualIncome | Customer's monthly income |
| TotalChildren | Number of children  |
| EducationLevel | The client's educational level |
| Occupation | Client function  |
| HomeOwner | Own a house or not  |
| Income Level | Customer income level (10,000, 50,000, etc.) |
| Age | Customer age  |
| Age_Type | Customer age classify  |

## 🚴 Product Lookup Table

| Column Name | Description |
|------------|------------|
| ModelName | Product model category |
| Net_Profit | Total profit after cost |
| ProductColor | Color of the product |
| ProductCost | Unit cost of the product |
| ProductKey | Unique product identifier |
| ProductName | Name of the product |
| ProductPrice | Unit selling price |
| ProductSize | Size or dimensions |
| ProductSKU | Stock Keeping Unit code |
| ProductStyle | The style of the product is women's, men's or both |
| ProductSubcategoryKey | Product subcategory ID

## 🚲 Product Subcategories Lookup Table

| Column Name | Description |
|------------|------------|
| ProductCategoryKey | Foreign key to the Product Categories table |
| ProductSubcategoryKey | Unique identifier for each subcategory |
| SubcategoryName | Name of the product subcategory |

## 📁 Product Categories Lookup Table

| Column Name | Description |
|------------|------------|
| CategoryName | Name of the product category |
| ProductCategoryKey | Unique identifier for each category | 

## 🔄 Returns Data Table

| Column Name | Description |
|------------|------------|
| ProductKey | Foreign key linking to the Product table |
| ReturnDate | The date when the product was returned |
| ReturnQuantity | The number of items returned in a single transaction |
| TerritoryKey | Foreign key linking to the Sales Territory table |
| Year | The year of the return transaction |

## 🌍 Territory Lookup Table

| Column Name | Description |
|------------|------------|
| Continent | The continent where the sales territory is located |
| Country | The country associated with the sales territory |
| Region | The specific region or province within the territory |
| SalesTerritoryKey | Unique identifier for each sales territory (Primary Key) |

## 📅 Calendar Lookup Table

| Column Name | Description |
|------------|------------|
| Date | The unique date used as the primary key for the calendar |
| Day | The day of the month extracted from the date |
| Month Name | The full name of the month (e.g., January, February) |
| Quarter | The quarter of the year (1, 2, 3, or 4) |
| Year | The fiscal or calendar year |
