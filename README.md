
# 📌 Project Overview


This project analyzes the widely used Superstore dataset to uncover key business insights about sales performance, profitability, customer behavior, and product performance. The goal is to answer high-value business questions such as:

- Which product categories drive the most revenue and profit?

- Which regions or segments perform best?

- Which products generate losses?

- How do discount rates impact profit?

- What patterns exist in monthly sales?

This project demonstrates strong analytical skills across R, dplyr, ggplot2, EDA, data cleaning, visualization, trend analysis, and business interpretation.

 
# 🧰 Tools & Skills Used

#### Category	Skills / Tools
Languages	R, tidyverse, ggplot2
Data Manipulation	dplyr, lubridate, stringr
Visualization	ggplot2, faceting, histograms, bar charts, line charts
Business Analytics	Profit analysis, segmentation, trend analysis
Statistical Concepts	Margins, correlations, linear trend lines
Reporting	Quarto / R Markdown


# 📂 Project Structure

```
├── README.md
├── data/
│   └── Sample - Superstore.csv
├── analysis/
│   └── superstore_analysis.R
├── plots/
│   ├── monthly_sales_trend.png
│   ├── profit_by_subcategory.png
│   ├── discount_vs_profit.png
│   ├── profit_margin_distribution.png
│   ├── region_profit.png
│   ├── segment_profit.png
│   ├── march_top5_by_year.png
```


# 📊 Key Insights & Visualizations


## 📈 1. Monthly Sales Trend (2014–2017 Combined)


<img width="1344" height="960" alt="unnamed-chunk-10-1" src="https://github.com/user-attachments/assets/4644a11e-d341-49aa-b590-d41b1c54ee6b" />
<img width="1344" height="960" alt="unnamed-chunk-12-1" src="https://github.com/user-attachments/assets/acba1f23-ae9f-47e4-9c49-617c01d1e066" />





Insight:

- Sales consistently peak in November and December, indicating strong seasonal demand. March, June, and September are secondary mini-peaks.

- The trend line shows overall upward movement, suggesting year-over-year growth.

## 🛍️ 2. Top 5 Sub-Categories Driving Sales in Peak Months of Latest Year (2017)

(Overall and also broken down by year)


<img width="1344" height="960" alt="Top_5_Sub-Categories_Driving_Sales_in_March_2017-1" src="https://github.com/user-attachments/assets/883fc650-d8d5-48c6-8576-878a3b451856" />

<img width="1344" height="960" alt="Top_5_Sub-Categories_Driving_Sales_in_November_2017-1" src="https://github.com/user-attachments/assets/555ce73b-3322-4124-95ce-701b54f244a1" />

<img width="1344" height="960" alt="Top_5_Sub-Categories_Driving_Sales_in_December_2017-1" src="https://github.com/user-attachments/assets/f4cbe747-2709-48b5-b49b-980d277dbf87" />


Insight:

Technology products dominate March sales, especially Phones, Machines, Copiers.

Furniture occasionally appears (Chairs, Tables), but Technology remains strongest.

Product focus in March should prioritize high-demand Tech SKUs.



## 💸 4. Profitability by Product Sub-Category

<img width="1344" height="960" alt="unnamed-chunk-17-1" src="https://github.com/user-attachments/assets/d5f8a397-ea6b-40db-a53f-f94a4d6f9388" />


Insight:

Top profit generators:

Copiers (extremely high margins)

Phones

Accessories

Loss-generating sub-categories:

Tables (largest losses)

Bookcases

Supplies

Recommendation:
Reevaluate pricing, shipping cost structure, or discontinue chronically unprofitable products.


## 📊 5. Profit Margin Distribution

<img width="1344" height="960" alt="Distribution_of_Profit_Margin_per_Order-1" src="https://github.com/user-attachments/assets/30021f4b-3bdb-499a-aa96-842f79e0ec49" />

Insight:

Most orders cluster around 0–20% margin range, with heavy right skew.

Several orders have extremely negative margins, indicating operational inefficiencies.

Mean profit margin ≈ 12%.

## 🌎 6. Profit by Region (with Margin %)

<img width="1344" height="960" alt="unnamed-chunk-24-1" src="https://github.com/user-attachments/assets/f1f301bf-0017-4a37-a7ee-849072ce1fc2" />

Insight:
Region	Profit	Margin
West	Highest	14.9%
East	Strong	13.5%
South	Moderate	11.9%
Central	Weakest	7.9%

Recommendation:
Investigate the Central region for high shipping costs, low-margin customers, or unprofitable products.

## 👥 7. Profit by Customer Segment (with Margin %)


<img width="1344" height="960" alt="unnamed-chunk-27-1" src="https://github.com/user-attachments/assets/e66c44fd-98b5-406b-a040-3d3ee1616948" />

Insight:
Segment	Profit	Margin
Consumer	Highest revenue	11.5% margin
Corporate	Strong	13% margin
Home Office	Smallest revenue	14% margin

Interpretation:
The Home Office segment is smaller but more profitable per order.
Opportunity: Explore targeted promotions to grow this high-margin segment.

## 📈 8. Sales vs. Profit Relationship

<img width="1344" height="960" alt="unnamed-chunk-16-1" src="https://github.com/user-attachments/assets/ec2767c1-cdfe-4691-b465-4cd894a834f3" />
<img width="1344" height="960" alt="unnamed-chunk-17-1" src="https://github.com/user-attachments/assets/0aba3df9-6735-484b-9680-97bb86603cc4" />

Insight:
A weak positive correlation:
Higher sales generally lead to higher profit, but with large variance.

Some high-sales orders still produce losses due to heavy discounting or high costs.

# 📌 Summary of Business Recommendations
✅ Focus inventory and marketing on high-profit items:

Copiers, Phones, Accessories

❗ Reduce loss-making categories:

Tables, Bookcases, Supplies

📍 Address regional underperformance:

Investigate Central region cost structure

🎯 Strengthen pricing strategy:

Avoid unnecessary deep discounts

Optimize pricing for low-margin products

💼 Customer Strategy:

Expand the high-margin Home Office segment

Maintain strong Corporate relationships
