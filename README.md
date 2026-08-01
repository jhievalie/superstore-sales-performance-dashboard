# 📊 Superstore Sales Performance Dashboard

An interactive **Sales Performance Dashboard** built with **Microsoft Power BI** to analyze retail sales performance using the **Sample Superstore** dataset.

This project demonstrates data modeling, Power Query transformations, DAX calculations, and dashboard design following Power BI best practices.

---

## 📸 Dashboard Preview

> *(Add your dashboard screenshot here)*

![Dashboard Overview](Images/dashboard-overview.png)

---

## 📌 Project Overview

The dashboard provides business users with an interactive overview of sales performance across different regions, customer segments, product categories, and time periods.

It was designed to answer common business questions such as:

- 💰 How much revenue was generated?
- 📦 How many orders were placed?
- 📈 How are sales trending over time?
- 🌎 Which regions perform best?
- 🛍 Which products generate the highest sales?
- 👥 Who are the top customers?

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

## 🏗 Data Model

The report follows a simple star-schema approach.

### Tables

- Orders (Fact Table)
- Calendar (Date Dimension)
- _Measures (DAX Measures)

Data model:

![Data Model](Documentation/data-model.png)

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

Data preparation includes:

- Data type validation
- Date conversion
- Calendar table creation
- Data quality checks
- Model relationship creation

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

- Microsoft Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)

---

## 📂 Dataset

This project uses the **Sample Superstore** dataset.

The dataset is **not included** in this repository to respect the original dataset owner's distribution terms.

Please download the dataset from its original source and place it inside the `Dataset` folder before opening the Power BI report.

---

## 🚀 Future Improvements

Planned enhancements include:

- Drill-through pages
- Bookmarks and navigation
- Tooltip pages
- Mobile-optimized layout
- Custom Power BI visual (.pbiviz)
- Additional business KPIs

---

## 👨‍💻 Author

**Jomar Pajenago**

Aspiring Data Analyst | Power BI | SQL | Excel | Python

GitHub: https://github.com/jhievalie

LinkedIn: https://www.linkedin.com/in/jomarp21/

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub.
