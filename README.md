# 📊 Global Superstore Sales Performance Dashboard

**An Interactive Business Intelligence Dashboard built with Tableau**

The **Global Superstore Sales Performance Dashboard** is a comprehensive interactive analytics solution developed using **Tableau**. This project analyzes a large retail sales dataset to provide deep insights into sales performance, regional profitability, product revenue, customer segments, and year-over-year growth trends.

The dashboard enables business managers and stakeholders to make data-driven decisions by visualizing key performance metrics in an intuitive and interactive manner.

## 🎯 Project Objectives

- Analyze sales and profit performance by region/market
- Identify the top 10 revenue-generating products
- Evaluate profit margins across different customer segments
- Visualize yearly sales and profit growth trends
- Provide dynamic filtering for year-wise performance analysis
- Deliver actionable business insights through effective visualizations

## 🛠️ Tools & Technologies Used

- **Tableau Desktop** (Data Visualization & Dashboarding)
- Calculated Fields & Table Calculations
- Parameters & Global Filters
- Advanced Chart Types (Packed Bubbles, Donut Chart, Dual Axis Line)
- KPI Cards & Interactivity

## 📸 Dashboard Preview
![Dashboard](./Sales%20Performance%20Dashboard_Image.png)

![Parameter Dashboard](Sales%20Performance%20Dashboard_Image(Parameter).png)


## 📂 Dataset Information

- **Dataset Name**: Global Superstore (Global_Superstore2)
- **Source**: Kaggle (Public Dataset)
- **Rows**: ~51,000 order line items
- **Time Period**: 2011 to 2014
- **Key Fields**: Order Date, Region/Market, Category, Sub-Category, Product Name, Sales, Profit, Segment, Ship Mode, etc.

## 📊 Dashboard Structure

The dashboard is built with **5 main sections** and full interactivity.

### 1. Executive Overview (KPI Cards)
- Total Sales
- Total Profit
- Profit Margin %
- Total Orders
- Average Shipping Days
- **Sales Comparisons** (Current Year vs Previous Year + Growth %)

### 2. Profit by Region
- Bar Chart showing profit contribution by Region/Market
- Highlights **APAC** as the highest profit generating market

### 3. Top 10 Products by Revenue
- **Packed Bubbles Chart** (Size = Revenue, Color = Category)
- High-ticket items like Canon copiers and Cisco phones dominate

### 4. Profit Margin by Customer Segment
- **Donut Chart** showing margin % across Consumer, Corporate & Home Office
- Corporate/Home Office segments show better margins

### 5. Yearly Sales Growth Trend
- Dual-axis Line Chart (Sales & Profit)
- Year Filter for dynamic year-wise analysis

## 🎨 Key Dashboard Features

- Fully Interactive **Year Filter** (updates entire dashboard)  
- Professional KPI Cards with Sales Comparison  
- Packed Bubbles visualization for Top 10 Products  
- Donut Chart for Segment Analysis  
- Dynamic Tooltips with rich information  
- Clean, Modern & Mobile-friendly Layout  
- Fixed dashboard size optimized for presentations (1200 × 800 px)

## 📈 Key Insights

- **APAC** region generates the highest profit due to strong Technology sales
- Technology category dominates both revenue and profit
- High-revenue products sometimes show low/negative profit due to heavy discounts
- Corporate and Home Office segments have better profit margins than Consumer
- Consistent upward sales growth observed from 2011 to 2014

## 💡 Business Recommendations

- Focus marketing and inventory on **APAC** market
- Promote high-margin Technology products
- Review discount strategy on low-profit products
- Target Corporate & Home Office segments for better profitability
- Optimize shipping modes to reduce average delivery days

## 🔍 Calculated Fields Used

Profit Margin % = SUM([Profit]) / SUM([Sales])

Avg Shipping Days = AVG(DATEDIFF('day', [Order Date], [Ship Date]))

YoY Sales Growth % = (ZN(SUM([Sales])) - LOOKUP(ZN(SUM([Sales])), -1)) / ABS(LOOKUP(ZN(SUM([Sales])), -1))

Highest Profit Region = IF SUM([Profit]) = WINDOW_MAX(SUM([Profit])) THEN "Highest" ELSE "Other" END


## 🚀 Future Enhancements

- Add more parameters (Region, Category, Ship Mode)
- Implement forecasting for future sales
- Add product-level profitability deep dive
- Publish to Tableau Public / Tableau Server
- Mobile responsive optimization

## 👨‍💻 Author
Giridharan S
Data Analytics | Tableau | Business Intelligence Enthusiast

## ⭐ Project Outcome
This project demonstrates the power of Tableau in transforming raw retail data into actionable business intelligence. The interactive dashboard provides clear visibility into sales performance, profitability, and growth trends, enabling better strategic decision-making.
