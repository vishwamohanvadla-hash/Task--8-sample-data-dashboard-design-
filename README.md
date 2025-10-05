# Task--8-sample-data-dashboard-design-
# 🧭 Simple Sales Dashboard Design (Power BI)

## 🎯 Objective
Create a clean and interactive **Sales Dashboard** that visualizes sales performance by **product category**, **region**, and **month**.  
The dashboard helps business users analyze trends, identify top-performing regions, and make data-driven decisions.

---

## 🧰 Tools & Technologies
- **Power BI Desktop**
- (Optional) **Python + Pandas** for data cleaning
- **Dataset:** `Superstore_Sales.csv`

---

## 📂 Dataset Details
The dataset contains the following columns:

| Column Name  | Description |
|---------------|-------------|
| Order Date    | Date when the order was placed |
| Region        | Sales region (e.g., East, West, Central, South) |
| Category      | Product category (e.g., Furniture, Office Supplies, Technology) |
| Sales         | Total sales amount |
| Profit        | Profit earned for each sale |

---

## ⚙️ Steps Followed

### 1. Data Import and Cleaning
- Imported the `Superstore_Sales.csv` file into **Power BI**
- Converted **Order Date** column to proper *Date* format
- Added a **Month-Year** column using Power Query:
  ```m
  = Date.ToText([Order Date], "MMM yyyy")
