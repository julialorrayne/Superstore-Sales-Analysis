# Superstore Sales Analysis  

## Background and Overview
This project is based on a mock superstore dataset. The company has significant amounts of data on its products orders, and customers. This project analyses and synthesizes this data to uncover insights that will enhance the superstore profitability. 
The goal of this project is to identify profit drivers, evaluate shipping efficiency, and provide data-driven recommendations to optimize business decisions.  
 
**Tools Used:** Python (Pandas, Plotly, Scikit-learn, Matplotlib, NumPy)
**Techniques:** Exploratory Data Analysis (EDA), Machine Learning Modeling, Correlation Analysis, Data Visualization, Business Insights  

## Data Structure Overview
The dataset contains 9,995 records of Superstore sales data. It includes information about orders, shipping details, customers, and products, along with key performance metrics such as sales, quantity, discount, and profit.

The original dataset can be found [here](https://usfedu-my.sharepoint.com/:x:/g/personal/lorrayne_usf_edu/EcGQGlYn56hIoRIFKAQOP-0B_8SEwR0CelpfssVhzTI8ug?e=fKVIJd)

## Executive Sumamary

---

## Key Insights  

### **1. Top 5 Most Profitable Transactions**
![Most Profitable products table](https://github.com/julialorrayne/Projects-images/blob/main/superstore/5%20most%20profitable.png?raw=true)

•	**Technology** → Copiers accounts for 3 out of the Top-5 most profitable transactions, generating $20,159.94 in total profit and $41,999.88 in sales.
These transactions all involve the Canon imageCLASS 2200 Advanced Copier, confirming it as the single most profitable product line.
•	**Regional Performance**:
The Central region contributes $17,976.83 (≈ 60.5%) of total Top-5 profit, followed by the West (22.6%) and East (16.9%) regions.
This concentration indicates strong sales potential and operational efficiency in the Central region.
•	**Customer Segmentation**:
Consumer customers represent 4 of 5 most profitable transactions, accounting for $21,336.82 in profit, while Corporate customers contribute $8,399.98.
The high profitability of Consumer transactions highlights sustained margins even in smaller-scale purchases. 
 
**Business Interpretation**

•	Product Focus: The Canon imageCLASS 2200 Advanced Copier drives most of the profit within this group.
Maintaining strong supplier relationships, optimizing inventory, and offering bundled service plans for this line could further improve margins.

•	Regional Strategy: The Central region’s dominance indicates an opportunity to replicate its success model—review shipping efficiency, regional pricing, and sales incentives.

•	Customer Insights: With Consumer transactions producing the majority of profits, targeted marketing, loyalty programs, and premium upsell campaigns could strengthen retention and revenue per order.

---

### **2. Shipping Mode Analysis**

#### **Ship Mode Frequency**
![ship mode frequency](https://github.com/julialorrayne/Projects-images/blob/main/superstore/ship%20mode.png?raw=true)

Standard Class is the most frequently used shipping mode, accounting for 5,967 orders — representing the majority of all shipments.
Its widespread use indicates it is likely the default or most cost-efficient option for customers.

Second Class and First Class follow with moderate utilization, suggesting these modes are chosen for customers who balance faster delivery with moderate cost.

Same Day shipping is used least frequently, implying that expedited delivery is rarely required or that higher costs discourage its use.


#### **Sales Amount by Ship Mode**
![ship mode sales](https://github.com/julialorrayne/Projects-images/blob/main/superstore/ship%20mode%20sales.png?raw=true)

Despite having fewer transactions, Same Day shipping generates the highest total sales ($1,357,934), indicating that customers who choose this mode tend to place higher-value orders.

First Class follows with a strong sales contribution($459,193), while Standard Class dominates in volume but not in total revenue.

Second Class has both the lowest sales volume and value, suggesting it is the least preferred option across customers.


---

### **3. Regional Analysis**

#### **Sales by Region and Ship Mode**
![sales by ship mode and region](https://github.com/julialorrayne/Projects-images/blob/main/superstore/sales%20by%20ship%20mode%20and%20region.png?raw=true)

• The East and West regions generate the highest total sales — $725,456 in the West and $678,499 in the East — indicating stronger market activity and customer demand.

•	The Central region shows moderate performance ($501,239), while the South region reports the lowest sales volume ($391,724).

•	Across all regions, Standard Class remains the dominant shipping mode, followed by Second Class and First Class.

Recommendation

•	Investigate the South region’s weaker sales performance by analyzing customer demographics, marketing reach, and product availability to identify potential demand gaps.

•	Replicate successful strategies from the East and West regions — such as regional promotions, improved delivery speed, or inventory optimization — to boost overall sales performance.


### **4. Monthly Sales Trend**
![monthly sales trend by ship mode](https://github.com/julialorrayne/Projects-images/blob/main/superstore/monthly%20sales%20trend%20by%20ship%20mode.png?raw=true)
- Sales peaks are observed during March, May, September, and November, suggesting increased purchasing activity likely driven by promotional events, holidays, or seasonal demand cycles.

Standard Class consistently leads in total sales volume throughout the year, showing stable customer preference for economical shipping.

**Recommendation:**  
Align marketing and promotional campaigns with high-sales months (March, May, September, November) to maximize seasonal revenue opportunities and promotional ROI.

Maintain adequate inventory and staffing levels in advance of these peaks to ensure smooth order fulfillment.
---

## Profitability & Correlation Analysis

### **Profitability by Ship Mode and Region**
![profitability correlation with ship mode and region](https://github.com/julialorrayne/Projects-images/blob/main/superstore/profitability%20correlation%20with%20ship%20mode%20and%20region.png?raw=true)
Profit is not always proportional to sales volume. Some transactions with high sales values yield relatively low or even negative profits, indicating potential pricing or cost inefficiencies.

The Central and East regions display stronger positive correlations between sales and profit, suggesting healthier margins and operational efficiency.

In contrast, the South region shows more scattered or negative profit values, especially for Standard Class and Same Day shipping, implying higher discounting or elevated shipping costs that reduce overall profitability.

First Class and Second Class order

### **Correlation Matrix (Overall)**
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

### 📈 Sales vs. Profit Correlation by Region

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


**Summary Insight:**  
Profitability varies by region. While the **West and Central regions** exhibit strong alignment between sales and profit, the **South region** shows almost no correlation, signaling inefficiencies. The **East region** maintains consistent profitability, making it a benchmark for best practices in pricing and operations.


## Recommendations

## Business Recommendations
Prioritize **Technology** category (especially *Copiers* and *Binders*).  
Maintain **Standard Class** for order volume; scale **Same Day** for premium customers.  
Reevaluate **discount policies** to improve profit margins.  
Plan **seasonal marketing** around sales peaks (March, May, September, November).  
Investigate **South region** for pricing or operational inefficiencies.  
