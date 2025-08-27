<h1>📦 DataCo Supply Chain Analysis</h1>
<h2>Overview </h2>
<h4>This project presents a comprehensive data analysis of the DataCo company's supply chain operations. Using transactional data, the analysis aims to identify key performance metrics, uncover operational bottlenecks, and provide actionable insights to enhance logistics efficiency, optimize profitability, and inform strategic decision-making.</h4>

<h3>🚀 Project Highlights</h3>
<ul><li>Data-Driven Insights:<br>Delivered a series of high-impact visualizations and findings on profitability, delivery performance, and market trends.</li>

<li>Operational Bottleneck Identification:<br> Pinpointed significant geographical disparities in delivery times and identified an operational bottleneck in the "Standard Class" shipping mode.</li>

<li>Potential Revenue Loss:<br> Quantified over $10,989,166 in potential revenue loss from cancelled and On-hold orders, providing a clear business case for strategic intervention.</li>

<li>End-to-End Analysis: <br>Demonstrated a complete data analysis workflow from raw, messy data to final, strategic recommendations.</li></ul>

<h3>⚙️ Methodology</h3>
    <h4>The analysis was conducted in Python and followed a structured, multi-phase approach:</h4>

<ul><li>Data Acquisition & Cleaning:<br>The raw DataCoSupplyChainDataset was loaded and meticulously     cleaned. This involved handling missing values, standardizing column names, and converting    data types to ensure data integrity.</li>
  <ul><li>Initial Inspection:<br> We first used df.info() and df.head() to understand the data's  structure, identify data types, and spot missing values and inconsistencies.</li>

  <li>Column Standardization: <br>We cleaned the column names by removing spaces and special characters, and converting them to a consistent format (e.g. order_date).</li>

  <li>Data Type Conversion: We converted Order Date and Shipping_Date from string objects to datetime format to enable time-based calculations. We also ensured that all numerical columns were correctly formatted as float or integer types.</li></ul></ul>

<ul><li>Feature Engineering: <br>New, insightful columns were created to enrich the analysis. Key metrics such as Delivery_Time_Days, Total_Order_Value, Order_Profit_Margin and Order_Status_Category were calculated to enable a deeper understanding of the business.</li>

  <ul><li>Delivery_Time_Days:<br> Calculated the time taken for a product to be delivered by subtracting  the order date from the shipping date.</li>
  
  <li>Total_Order_Value: <br>Created a new column to represent the total value of each order item.</li>
 
 <li>Order_Profit_Margin: <br>Calculated the profit margin as a percentage for each order to better understand profitability.</li>
  
  <li>Order_Status_Category: <br>Grouped the detailed order statuses into broader, more manageable categories (e.g., 'Completed', 'Canceled', 'On Hold') for easier analysis.</li></ul></ul>

<ul><li>Exploratory Data Analysis (EDA):<br> A series of visualizations were created using Matplotlib and Seaborn to explore key performance indicators (KPIs) and uncover hidden patterns. This phase focused on financial analysis, product performance, logistics efficiency, and customer behavior.</li>

  <ul><li>Financial Analysis:<br> We plotted monthly trends for revenue and profit, identified top-performing product categories, and visualized the relationship between profit and order value using a scatter plot.</li>

  <li>Logistics Analysis:<br> We created bar charts to analyze the average delivery time and late delivery risk across different shipping modes and regions.</li>

  <li>Customer & Market Analysis:<br> We identified the top countries by number of orders and used a pie chart to visualize the distribution of order statuses.</li></ul></ul>

<ul><li>⭐Strategic Recommendations:<br> Insights from the EDA were synthesized into a final report, providing clear, data-backed recommendations for executive-level decision-making.</li></ul>

<h3>📈 Key Findings & Recommendations</h3>
<h4>The analysis revealed several critical insights for DataCo's leadership:</h4>

<ul><li>Financial Performance:<br>
      The top-performing product categories and high-value orders were identified as the primary drivers of profitability, but significant variability in profit margins suggests a need for standardized pricing.</li>

<li>Logistics & Delivery:<br>
      A clear performance hierarchy was observed across different shipping modes, with notable geographical disparities in on-time delivery.</li>

<li>Order Fulfillment:<br>
  A significant portion of revenue is tied up in pending and on-hold orders, highlighting an opportunity to streamline the order-to-cash cycle.</li></ul>

<h3>💡Recommendations:</h3>

<ul><li>Enhance Logistics: <br>
  Investigate and resolve root causes of delays in high-risk regions to improve customer satisfaction and reduce late-delivery penalties.</li>

<li>Focus on Profitability:<br> 
  Implement a dynamic pricing model and a cost-control framework to standardize profit margins across all orders.</li>

<li>Optimize Order Flow:<br> Develop a robust process for managing pending orders to accelerate their conversion into completed sales and revenue.</li></ul>
