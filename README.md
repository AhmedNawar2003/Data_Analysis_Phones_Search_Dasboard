# Data_Analysis_Phones_Search_Dasboard

# 📊 Phones Search Dashboard – Power BI Final Project

## 📁 Project Overview
This Power BI project analyzes a dataset of phone products listed online to uncover insights related to pricing, sales performance, customer ratings, and sustainability.  
It demonstrates the full data analysis workflow — from data cleaning and modeling to visualization and storytelling.

---

## 🧹 Data Preparation (Power Query)
Data cleaning and transformation steps:
- Checked and corrected **data types**
- Handled **null and missing values**
- Removed duplicates and standardized text fields
- Ensured numerical columns (price, sales, offers) were properly formatted
- Created a clean data model ready for DAX calculations

---

## ⚙️ DAX Calculations & Measures
Key calculated columns and measures:
- `Avg Product Price = AVERAGE(Product[product_price])`
- `Avg Star Rating = AVERAGE(Product[product_star_rating])`
- `Total Sales = SUM(Product[total_sales])`
- `Sales per Product = [Total Sales] / COUNT(Product[product_title])`
- `Best Seller Count = COUNTROWS(FILTER(Product, Product[is_best_seller] = TRUE()))`
- `Amazon Choice Count = COUNTROWS(FILTER(Product, Product[is_amazon_choice] = TRUE()))`
- `Climate Friendly % = DIVIDE(COUNTROWS(FILTER(Product, Product[climate_friendly] = TRUE())), COUNTROWS(Product))`

---

## 📊 Dashboard Highlights
Visuals designed to deliver clear insights:
- **KPI Cards:** Average Price, Star Rating, Total Sales, Climate-Friendly %, Amazon Choice Count  
- **Bar Charts:** Total Sales & Total Offers by Product Title  
- **Pie/Donut Charts:** Sales by Prime Eligibility, Best Seller, Amazon Choice  
- **Line Chart:** Sales trend by Date  

---

## 💡 Insights
- Average product price: **$180.36**  
- Average star rating: **4.07⭐**  
- Total sales: **111K units**  
- Only **19%** of products are climate-friendly  
- A small portion of products are **Amazon Choice** or **Best Sellers**

---

## ✅ Conclusion
The dashboard reveals that non-Prime products contribute most to total sales, while climate-friendly and Amazon Choice products remain underrepresented.

---

## 🔧 Recommendations
1. Promote **climate-friendly** and **Prime-eligible** products.  
2. Focus on improving **product ratings** through better quality and customer engagement.  
3. Increase offers for **top-selling brands**.  
4. Utilize **Amazon Choice** and **Best Seller** tags for marketing visibility.  
5. Monitor **sales trends** to identify seasonal peaks.

---

## 🛠️ Tools Used
- **Power BI**
- **Power Query**
- **DAX**
- **Data Visualization & Storytelling**

---

## 👨‍💻 Author
**Ahmed Nawar**  
Data Analyst | Power BI Developer  
🔗 [GitHub](https://github.com/AhmedNawar2003) | 💼 [LinkedIn](https://www.linkedin.com/in/ahmednawar2003)
