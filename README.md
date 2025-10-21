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
## Insights Deep Dive
## Recommendations

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


**Recommendation:**  
Focus on the **Technology category** and **Consumer segment** in profitable regions to sustain high margins.

---

### **2. Shipping Mode Analysis**

#### **Ship Mode Frequency**
![ship mode frequency](https://github.com/julialorrayne/Projects-images/blob/main/superstore/ship%20mode.png?raw=true)
- **Standard Class** is the most used shipping mode, accounting for most orders.  
- **Second Class** and **First Class** follow, while **Same Day** is used the least.

#### **Sales Amount by Ship Mode**
![ship mode sales](https://github.com/julialorrayne/Projects-images/blob/main/superstore/ship%20mode%20sales.png?raw=true)
- Despite fewer transactions, **Same Day** shipping generates the **highest total sales**, indicating higher-value orders.

**Recommendation:**  
- Continue prioritizing *Standard Class* for volume and customer satisfaction.  
- Expand *Same Day* delivery for high-value customers to increase profitability.

---

### **3. Regional Analysis**

#### **Order Frequency by Ship Mode and Region**
![order frequency by ship mode and region](https://github.com/julialorrayne/Projects-images/blob/main/superstore/order%20frequency%20by%20ship%20mode%20and%20region.png?raw=true)
- Across all regions, **Standard Class** dominates, followed by **Second Class** and **First Class**.

#### **Sales by Region and Ship Mode**
![sales by ship mode and region](https://github.com/julialorrayne/Projects-images/blob/main/superstore/sales%20by%20ship%20mode%20and%20region.png?raw=true)
- **East** and **West** regions generate the highest total sales.  
- **South** underperforms in both sales and profit.

**Recommendation:**  
Investigate operational costs, discounting, and product mix in the South region to identify reasons for low profitability.

---

### **4. Monthly Sales Trend**
![monthly sales trend by ship mode](https://github.com/julialorrayne/Projects-images/blob/main/superstore/monthly%20sales%20trend%20by%20ship%20mode.png?raw=true)
- Sales peaks occur during **March**, **May**, **September**, and **November**, likely tied to **promotional events** or **seasonal demand**.  

**Recommendation:**  
Align marketing campaigns with these seasonal peaks to maximize promotional ROI.

---

## Profitability & Correlation Analysis

### **Profitability by Ship Mode and Region**
![profitability correlation with ship mode and region](https://github.com/julialorrayne/Projects-images/blob/main/superstore/profitability%20correlation%20with%20ship%20mode%20and%20region.png?raw=true)
- Profit is **not always correlated with sales volume**.  
- Some regions show high sales but **negative profits**, suggesting inefficiencies (e.g., excessive discounts or high shipping costs).

### **Correlation Matrix (Overall)**
![correlation matrix](https://github.com/julialorrayne/Projects-images/blob/main/superstore/correlation%20matrix.png?raw=true)
| Variable Relationship | Observation |
|-----------------------|--------------|
| **Sales & Profit** | Weak positive correlation |
| **Discount & Profit** | Strong negative correlation |
| **Discount & Sales** | Slight negative correlation |
| **Quantity & Profit** | Minimal correlation |

**Recommendation:**  
Reassess **discount strategies**. High discounts significantly reduce profit margins without consistently increasing sales.

---

### **Regional Correlation Insights**
![correlation south](https://github.com/julialorrayne/Projects-images/blob/main/superstore/correlation%20south.png?raw=true)
![correlation west](https://github.com/julialorrayne/Projects-images/blob/main/superstore/correlation%20west.png?raw=true)
![correlation central](https://github.com/julialorrayne/Projects-images/blob/main/superstore/correlation%20central.png?raw=true)
![correlation east](https://github.com/julialorrayne/Projects-images/blob/main/superstore/correlation%20east.png?raw=true)
- **South Region:** Lowest correlation between Sales and Profit → inefficient pricing or discounting.  
- **East Region:** Highest correlation → strong operational efficiency and pricing strategy.  

**Recommendation:**  
Benchmark the East region’s practices across other regions to improve consistency in profitability.

---
## Business Recommendations
Prioritize **Technology** category (especially *Copiers* and *Binders*).  
Maintain **Standard Class** for order volume; scale **Same Day** for premium customers.  
Reevaluate **discount policies** to improve profit margins.  
Plan **seasonal marketing** around sales peaks (March, May, September, November).  
Investigate **South region** for pricing or operational inefficiencies.  
