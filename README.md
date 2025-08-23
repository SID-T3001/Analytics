# Analytics
Projects related to DATA ANALYTICS
Executive Summary

This deep-dive analysis of the supply chain transactional data reveals critical insights into the company's operational performance, financial health, and key market dynamics. While the business demonstrates strong revenue growth, a strategic focus is needed to address operational inefficiencies, particularly in logistics and order fulfillment.

Our analysis identifies three core areas for strategic intervention:

1. Optimize Logistics: Streamline delivery operations by targeting high-risk regions and leveraging efficient shipping modes to mitigate delivery risk and enhance customer experience.

2. Monetize Top-Tier Markets: Fortify presence in high-volume markets by deploying tailored

marketing and sales strategies to capture a larger share of the most profitable customer base.

3. Streamline Order Fulfillment: Implement a robust process for managing order statuses to

reduce the volume of pending and on-hold orders, thereby accelerating the conversion of sales into revenue.
By strategically addressing these imperatives, the firm can move beyond reactive management and build a data-driven, resilient, and highly profitable supply chain ecosystem.

Key Findings & Strategic Recommendations

1. Financial Performance

Insight: The scatter plot of Profit vs. Order Value demonstrates a strong positive correlation, indicating that high-value orders are the primary drivers of profitability. However, the dispersion of data points shows significant variance in profit margins across orders of similar value, suggesting a lack of standardized pricing or cost control.

Recommendation:
Standardize Pricing & Costing: Implement a dynamic pricing model and review product-level costs to reduce profit variability and ensure consistent margins, even on lower-value orders.

2. Logistics & Operational Efficiency

Insight: Our analysis of Delivery Time vs. Shipping Mode indicates a clear performance hierarchy, with Express Air and Standard Class being the most widely used. The Late Delivery Risk chart, however, reveals significant geographical disparities, with certain regions exhibiting a disproportionately high risk of late shipments. This is a critical operational bottleneck.

Recommendation:

Optimize Regional Logistics: Conduct a localized deep-dive into the high-risk regions to identify and resolve root causes of delays, such as poor last-mile delivery infrastructure or inefficient routing. This is a strategic imperative for improving customer satisfaction.
Right-Size Shipping Modes: While Standard Class is popular, evaluate whether it is

the most optimal mode for all orders. Consider a tiered shipping strategy that matches order value and product category with the most appropriate shipping mode to balance cost and speed.

3. Customer & Market Insights

Insight: The Orders by Country chart confirms a strong concentration of demand in a few key markets. The Order Status Distribution pie chart, however, highlights an area of concern: a substantial percentage of orders are in Pending, On Hold, or Canceled status. These are effectively lost revenue opportunities.

Recommendation:

Fortify Core Markets: Develop a strategic plan to deepen market penetration in the

top-performing countries. This could involve targeted marketing campaigns or establishing localized partnerships.

Leverage High-Value Opportunities: Conduct a granular review of high-profit, high-

value orders to identify the underlying drivers of their success. Develop a best-practice framework to replicate these conditions across the organization.


Streamline Fulfillment & Conversion: Implement a robust order management system to proactively manage Pending and On Hold orders. This will accelerate the order-to-cash cycle and reclaim potentially lost revenue. Evaluate the drivers of order cancellation to reduce churn.
Based on the dataset, DataCo is a global e-commerce and retail company. Its primary business involves selling a wide variety of products directly to consumers online.

The company's operations are defined by two core functions:

E-commerce and Sales

DataCo sells goods across multiple categories, including electronics, apparel, and sporting goods. Its business model relies on a direct-to-consumer sales channel, where it processes individual orders from customers located around the world. The company uses different marketing and sales strategies to serve various customer segments.

Supply Chain and Logistics

A major part of DataCo's business is the management of a complex global supply chain. The company handles all aspects of order fulfillment, including inventory management, order processing, and shipping. It uses various shipping modes and works with different logistics partners to get products to customers efficiently and reliably, while managing costs and delivery times.
About the "DataCo" Company

The "DataCo" company is a fictional entity created for this dataset. It's a case study designed to simulate a real-world business with a complex supply chain. It's not a real organization, but the data and the problems it presents are highly realistic, making it an excellent tool for practicing data analysis skills.

Purpose of the Data Analysis

We performed this data analysis to transform raw transactional data into actionable business intelligence. The core purpose was to help DataCo move away from making decisions based on intuition and instead use a data-driven approach to improve its operations. We aimed to answer critical business questions, such as:

Which products and markets are the most profitable?

Are there any bottlenecks in the shipping and delivery process?

How can the company better manage its order fulfillment to increase revenue?
Impact on Executive-Level Decision-Making

This data analysis provides a clear, evidence-based roadmap for executive decision-making. The insights we've uncovered will directly influence strategy and resource allocation.

Financial Decisions: Our analysis of profit and revenue trends helps executives decide

where to invest (e.g., allocating more marketing budget to high-profit product categories). By identifying the top revenue drivers and understanding profit margins, executives can prioritize products and markets that will yield the greatest return.

Operational Decisions: The logistics insights on delivery times and late shipments are

critical for improving efficiency. Executives can use this information to make strategic choices, such as optimizing shipping routes, evaluating new logistics partners, or even establishing new distribution centers in regions with a high number of late deliveries.

Strategic Decisions: By understanding customer demand and order status, executives can formulate business strategy. For example, they can prioritize sales efforts in top-performing countries and implement new processes to reduce the number of pending or canceled orders, directly improving the company's bottom line.

Here is a step-by-step summary of everything we did in this project, from start to finish. This is formatted so you can easily add it to your report to explain your methodology.

1. Data Acquisition and Environment Setup

We began by acquiring the DataCo Supply Chain Dataset from Kaggle. We set up a local data analysis environment using Jupyter Notebook in VS Code. We imported the necessary Python libraries: pandas for data manipulation, matplotlib and seaborn for visualization, and numpy for numerical operations.

2. Data Cleaning and Preprocessing

This was a critical phase where we transformed the raw, messy data into a clean, usable format.

Initial Inspection: We first used df.info() and df.head() to understand the data's structure, identify data types, and spot missing values and inconsistencies.

Column Standardization: We cleaned the column names by removing spaces and special characters, and converting them to a consistent format (e.g., order_date).
Data Type Conversion: We converted Order Date and Shipping_Date from string objects to datetime format to enable time-based calculations. We also ensured that all numerical columns were correctly formatted as float or integer types.

Handling Missing Data: We handled missing values by either dropping columns that were irrelevant to the analysis (e.g., customer_email) or by filling them with appropriate values where needed.

3. Feature Engineering

We created new, insightful columns from the existing data to enrich our analysis.

Delivery_Time_Days: Calculated the time taken for a product to be delivered by subtracting the order date from the shipping date.

Total_Order_Value: Created a new column to represent the total value of each order item.

Order_Profit_Margin: Calculated the profit margin as a percentage for each order to better understand profitability.
Order_Status_Category: Grouped the detailed order statuses into broader, more manageable categories (e.g., 'Completed', 'Canceled', 'On Hold') for easier analysis.

4. Exploratory Data Analysis (EDA) and Visualization

In this phase, we used a variety of charts to uncover key insights into the company's performance. We used pandas for data aggregation and matplotlib/seaborn for visualization.

Financial Analysis: We plotted monthly trends for revenue and profit, identified top-

performing product categories, and visualized the relationship between profit and order value using a scatter plot.

Logistics Analysis: We created bar charts to analyze the average delivery time and late delivery risk across different shipping modes and regions.

Customer & Market Analysis: We identified the top countries by number of orders and used a pie chart to visualize the distribution of order statuses.
