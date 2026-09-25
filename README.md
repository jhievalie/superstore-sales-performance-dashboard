# 📊 Superstore Sales Performance Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power%20Query-217346?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

An interactive **Sales Performance Dashboard** built with **Microsoft Power BI**, using **PostgreSQL** as the database layer and **Power Query** for data transformation and integration.

The project analyzes retail sales performance using the **Sample Superstore** dataset and demonstrates data modeling, SQL/database management, Power Query transformations, DAX calculations, and dashboard design following Power BI best practices.

---

## 📸 Dashboard Preview

Interactive dashboard built using Microsoft Power BI.

![Superstore Sales Performance Dashboard](Images/dashboard-overview.png)

### Sales Trend

![Sales Trend](Images/sales-trend.png)

### Top Products

![Top Products](Images/top-products.png)

---

## 📌 Project Overview

This interactive Power BI dashboard provides business users with a comprehensive view of retail sales performance across different regions, customer segments, product categories, and time periods.

The project uses **PostgreSQL as the data storage layer**, with Power Query connecting Power BI to the PostgreSQL database. The data is transformed and prepared in Power Query before being loaded into the Power BI data model.

It was designed to help decision-makers monitor sales performance, identify trends, evaluate regional performance, and discover high-performing products and customers through interactive visualizations.

### Business Questions Answered

- 💰 How much revenue was generated?
- 📦 How many orders were placed?
- 📈 How are sales trending over time?
- 🌎 Which regions perform best?
- 🛍 Which products generate the highest sales?
- 👥 Who are the top customers?

---

## 🎯 Business Objectives

This dashboard was developed to help decision-makers:

- Monitor overall sales performance
- Identify top-performing products and customers
- Compare sales across regions and categories
- Analyze sales trends over time
- Support data-driven business decisions

---

## ✨ Features

### Executive KPIs

- Total Sales
- Total Orders
- Average Order Value
- Average Sales per Day

### Interactive Visualizations

- Monthly Sales Trend
- Sales by Category
- Sales by Region
- Top 10 Products
- Top 10 Customers

### Interactive Filters

- Year
- Region
- Category
- Segment

---

## 🏗 Data Architecture & Model

The project uses a simple **star-schema approach**, with PostgreSQL serving as the database layer and Power BI serving as the reporting and visualization layer.

### Data Flow

```text
Sample Superstore Dataset
          ↓
      PostgreSQL
          ↓
     Power Query
          ↓
   Power BI Data Model
          ↓
     Power BI Report
```

### Database

The source data is stored in a PostgreSQL database in an `orders` table.

PostgreSQL was used to:

- Store the sales dataset in a relational database
- Define structured data types for each column
- Manage the `orders` table using SQL
- Provide a centralized data source for Power BI

### Power Query

Power Query connects Power BI to PostgreSQL and performs the required transformations, including:

- Data type validation
- Column renaming
- Data preparation
- Data quality checks
- Integration with the Power BI data model

The PostgreSQL database uses `snake_case` column names, while Power Query maps them to the existing Power BI model's user-friendly column names.

### Power BI Data Model

The report follows a simple star-schema approach.

#### Tables

- **Orders** — Fact Table
- **Calendar** — Date Dimension
- **_Measures** — DAX Measures

Data model:

![Data Model](Documentation/data-model.png)

---

## 🗄 PostgreSQL Database

The `orders` table was created using PostgreSQL:

```sql
CREATE TABLE orders (
    Order_ID varchar(15),
    Order_Date date,
    Ship_Date date,
    Ship_Mode varchar(15),
    Customer_ID varchar(10),
    Customer_Name varchar(40),
    Segment varchar(15),
    Country varchar(40),
    City varchar(20),
    States varchar(25),
    Postal_Code int,
    Region varchar(15),
    Product_ID varchar(20),
    Category varchar(20),
    Sub_Category varchar(20),
    Product_Name varchar(255),
    Sales decimal(18,3)
);
```

The database was managed using **pgAdmin 4**, while SQL was used to create and populate the table.

---

## 🧮 DAX Measures

The dashboard uses custom DAX measures including:

- Total Sales
- Total Orders
- Average Order Value
- Average Sales per Day

See the complete formulas here:

📄 [Documentation/dax-measures.md](Documentation/dax-measures.md)

---

## ⚙ Power Query Transformations

Power Query connects directly to the PostgreSQL database instead of loading the original CSV directly into Power BI.

The transformation process includes:

- Connecting to PostgreSQL
- Selecting the `public.orders` table
- Renaming database columns to match the Power BI model
- Data type validation
- Date handling
- Calendar table creation
- Data quality checks
- Maintaining model relationships

This approach allows the PostgreSQL database structure to remain optimized for database use while preserving the existing Power BI model and dashboard structure.

---

## 🎨 Dashboard Design

Design principles used:

- Clean executive layout
- Microsoft Fluent-inspired color palette
- Responsive spacing
- Consistent KPI cards
- Interactive slicers

Documentation:

📄 [Documentation/dashboard-design.md](Documentation/dashboard-design.md)

---

## 🛠 Built With

| Tool / Technology | Purpose |
|------|---------|
| **Microsoft Power BI Desktop** | Dashboard Development & Data Visualization |
| **PostgreSQL** | Relational Database & Data Storage |
| **pgAdmin 4** | PostgreSQL Database Management |
| **Power Query** | Data Transformation & Data Integration |
| **DAX** | Business Calculations & Measures |
| **SQL** | Database Table Creation & Data Management |
| **GitHub** | Version Control & Portfolio |

---

## 📂 Dataset

This project uses the publicly available **Sample Superstore** dataset.

The original dataset is not included in this repository.

To reproduce the project, download the dataset from its original source and load the data into PostgreSQL before connecting Power BI to the database.

Dataset Source:

- [Sales Forecasting Dataset by Rohit Sahoo (Kaggle)](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting)

---

## 🚀 Future Improvements

Planned enhancements include:

- Drill-through pages
- Bookmarks and navigation
- Tooltip pages
- Mobile-optimized layout
- Custom Power BI visual (.pbiviz)
- Additional business KPIs
- Additional PostgreSQL analytical views
- Advanced SQL-based reporting queries

---

## 👨‍💻 Author

**Jomar Pajenago**

Aspiring Data Analyst passionate about Business Intelligence, Data Visualization, SQL, and Process Automation.

- GitHub: [jhievalie](https://github.com/jhievalie)
- LinkedIn: [Jomar Pajenago](https://www.linkedin.com/in/jomarp21/)

---

⭐ If you found this project useful or interesting, consider giving it a star on GitHub.

Made with ❤️ using **Microsoft Power BI, PostgreSQL, Power Query, DAX, SQL, and GitHub.**
