# Superstore Sales Analysis  

## Background and Overview
This project is based on a mock superstore dataset. The company has significant amounts of data on its products orders, and customers. This project analyses and synthesizes this data to uncover insights that will enhance the superstore profitability. 
The goal of this project is to identify profit drivers, evaluate shipping efficiency, and provide data-driven recommendations to optimize business decisions.  
 
**Tools Used:** Python (Pandas, Plotly, Scikit-learn, Matplotlib, NumPy)

**Techniques:** Exploratory Data Analysis (EDA), Machine Learning Modeling, Correlation Analysis, Data Visualization, Business Insights  

---

## Data Structure Overview
The dataset contains 9,995 records of Superstore sales data. It includes information about orders, shipping details, customers, and products, along with key performance metrics such as sales, quantity, discount, and profit.

Data cleaning techniques included handling missing values and outliers, validating data types, removing duplicates, and eliminating irrelevant variables to ensure data quality and consistency.

The original dataset can be found [here](https://usfedu-my.sharepoint.com/:x:/g/personal/lorrayne_usf_edu/EcGQGlYn56hIoRIFKAQOP-0B_8SEwR0CelpfssVhzTI8ug?e=fKVIJd)

---

## Executive Sumamary

Key findings show that high-margin Technology products, particularly the Canon imageCLASS 2200, generate the majority of profits; Standard Class remains the most cost-effective and widely used shipping mode. Regional analysis highlights strong sales performance in the East and West, while the South region underperforms due to likely pricing and cost inefficiencies. Seasonal patterns further indicate demand peaks in March, May, September, and November, offering actionable windows for marketing and operational planning.


Strategic recommendations include:

•	Product Strategy: Prioritize and promote high-margin products such as the Canon imageCLASS 2200 and bundle complementary items.

•	Shipping Optimization: Preserve affordability and efficiency in Standard Class deliveries.

•	Regional Performance: Replicate the successful sales and pricing models of the East and West regions. Conduct a deeper review of discounting and delivery operations in the South to address low profitability.

•	Seasonality and Demand Planning: Align marketing campaigns, promotions, and staffing with high-sales months to capitalize on peak demand and ensure smooth fulfillment.

•	Pricing and Discount Strategy: Implement a data-driven discount policy.	Apply smarter, data-based discounts as current discounts reduce profit without significantly increasing sales.

---

## Key Insights  

### Top 5 Most Profitable Transactions
![Most Profitable products table](https://github.com/julialorrayne/Projects-images/blob/main/superstore/5%20most%20profitable.png?raw=true)

•	**Technology** → Copiers accounts for 3 out of the Top-5 most profitable transactions, generating $20,159.94 in total profit and $41,999.88 in sales.
These transactions all involve the Canon imageCLASS 2200 Advanced Copier, confirming it as the single most profitable product line.

---

### Shipping Mode Analysis

#### Ship Mode Frequency
![ship mode frequency](https://github.com/julialorrayne/Projects-images/blob/main/superstore/ship%20mode.png?raw=true)

Standard Class is the most frequently used shipping mode, accounting for 5,967 orders — representing the majority of all shipments.
Its widespread use indicates it is likely the default or most cost-efficient option for customers.

Second Class and First Class follow with moderate utilization, suggesting these modes are chosen for customers who balance faster delivery with moderate cost.

Same Day shipping is used least frequently, implying that expedited delivery is rarely required or that higher costs discourage its use.


#### Sales Amount by Ship Mode
![ship mode sales](https://github.com/julialorrayne/Projects-images/blob/main/superstore/ship%20mode%20by%20sales.png?raw=true)

Standard Class generates the highest total sales ($1,357,934).

Second Class follows with a sales contribution of $459,193, closely followed by First Class($351,428).

Same Day has both the lowest sales volume and value, suggesting it is the least preferred option across customers.


---

### Regional Analysis

#### **Sales by Region and Ship Mode**
![sales by ship mode and region](https://github.com/julialorrayne/Projects-images/blob/main/superstore/sales%20by%20ship%20mode%20and%20region.png?raw=true)

• The East and West regions generate the highest total sales — $725,456 in the West and $678,499 in the East — indicating stronger market activity and customer demand.

•	The Central region shows moderate performance ($501,239), while the South region reports the lowest sales volume ($391,724).

•	Across all regions, Standard Class remains the dominant shipping mode, followed by Second Class and First Class.


---

### Monthly Sales Trend
![monthly sales trend by ship mode](https://github.com/julialorrayne/Projects-images/blob/main/superstore/monthly%20sales%20trend%20by%20ship%20mode.png?raw=true)
- Sales peaks are observed during March, May, September, and November, suggesting increased purchasing activity likely driven by promotional events, holidays, or seasonal demand cycles.

Standard Class consistently leads in total sales volume throughout the year, showing stable customer preference for economical shipping.

---

## Profitability & Correlation Analysis

### **Profitability by Ship Mode and Region**
![profitability correlation with ship mode and region](https://github.com/julialorrayne/Projects-images/blob/main/superstore/profitability%20correlation%20with%20ship%20mode%20and%20region.png?raw=true)
Profit is not always proportional to sales volume. Some transactions with high sales values yield relatively low or even negative profits, indicating potential pricing or cost inefficiencies.

The Central and East regions display stronger positive correlations between sales and profit, suggesting healthier margins and operational efficiency.

In contrast, the South region shows more scattered or negative profit values, especially for Standard Class and Same Day shipping, implying higher discounting or elevated shipping costs that reduce overall profitability.


### Correlation Matrix
![correlation matrix](https://github.com/julialorrayne/Projects-images/blob/main/superstore/correlation%20matrix.png?raw=true)
| Variable Relationship | Observation |
|-----------------------|--------------|
| **Sales & Profit** | Weak positive correlation |
| **Discount & Profit** | Strong negative correlation |
| **Discount & Sales** | Slight negative correlation |
| **Quantity & Profit** | Minimal correlation |

Sales and Profit show a weak positive correlation (r = 0.47), suggesting that while higher sales often lead to higher profits, the relationship is not strongly linear — likely due to varying costs, discounts, and product margins.

Discount and Profit display a strong negative correlation (r = -0.22), confirming that larger discounts tend to reduce profit margins without a proportionate increase in sales.

Discount and Sales have a slight negative correlation (r = -0.03), indicating that discounts do not consistently drive higher sales volumes.

Quantity and Profit exhibit minimal correlation (r ≈ 0.07), meaning that selling more units doesn’t necessarily translate into higher profits — possibly due to product mix or variable pricing.


---

### Sales vs. Profit Correlation by Region

| **Region** | **Correlation (r)** | **Interpretation** |
|-------------|--------------------|--------------------|
| **South**   | 0.01               | Very weak correlation |
| **Central** | 0.64               | Strong positive correlation |
| **West**    | 0.65               | Strong positive correlation |
| **East**    | 0.52               | Moderate positive correlation |


South Region: Shows the lowest correlation between Sales and Profit (r ≈ 0.01), indicating potential inefficiencies in pricing or discount management. Despite steady sales, profit remains inconsistent, suggesting that higher discounts or operational costs are eroding margins.

Central Region: Exhibits a moderate correlation (r ≈ 0.64), reflecting relatively stable pricing and profit behavior but still with room for optimization in discount policies.

West Region: Also presents a strong positive correlation (r ≈ 0.65), showing effective alignment between revenue growth and profit generation — though minor discount-related inefficiencies may persist.

East Region: Demonstrates the highest correlation between Sales and Profit (r ≈ 0.52), suggesting strong operational efficiency and disciplined pricing strategies. This region appears to manage discounting and cost structures effectively, maintaining profitability consistency.


---

## Business Recommendations
**1. Product Strategy**

•	Focus on high-margin products — particularly the Canon imageCLASS 2200, which generated the majority of profits among top transactions.
Promote them more aggressively and bundle complementary items to increase the order value. 



**2. Shipping Optimization**

•	As the most frequently used and cost-effective shipping mode, continue to preserve affordability of Standard Class to sustain order volume and customer satisfaction.



**3. Regional Performance**

•	Both East and West regions show strong sales(generating $678K and $725K respectively) and positive profit correlation (r ≈ 0.52–0.65), indicating efficient operations and effective pricing. Analyze their sales practices, promotional campaigns, and cost structures to replicate these models across other regions.

•	South region underperforms in both sales and profitability. Conduct a deeper diagnostic into pricing, discounting, and delivery costs to identify inefficiencies.



**4. Seasonality and Demand Planning**

•	Sales peaks occur in March, May, September, and November. Align marketing campaigns and promotional discounts with these high-sales periods to maximize ROI.

•	Increase inventory and staffing capacity ahead of peak months to avoid stockouts and maintain customer satisfaction.



**5. Pricing and Discount Strategy**

•	Correlation analysis shows that discounts have a strong negative impact on profit (r = -0.22), while their effect on sales is minimal. Implement discount optimization — offer discounts selectively where they demonstrably improve volume or customer acquisition.
