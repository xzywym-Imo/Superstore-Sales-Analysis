
# 📌 Project Overview


This project analyzes the widely used Superstore dataset to uncover key business insights about sales performance, profitability, customer behavior, and product performance. The goal is to answer high-value business questions such as:

- Which product categories drive the most revenue and profit?

- Which regions or segments perform best?

- Which products generate losses?

- How do discount rates impact profit?

- What patterns exist in monthly sales?

- Whether an order will be profitable or unprofitable before it is completed?
  - Should we allow this order or discount? (Logistic Regression)


# Tools & Skills Used
This project demonstrates strong analytical skills across R, dplyr, ggplot2, EDA, data cleaning, visualization, trend analysis, and business interpretation.


Languages: 	R, tidyverse, ggplot2 

Data Manipulation: 	dplyr, lubridate, stringr 

Visualization:	ggplot2, faceted plots, histograms, bar/line charts 

Business Analytics:	Profitability, segmentation, time series patterns 

Statistics: Margins, correlations, linear modeling, logistic regression


# 📊 Key Insights & Visualizations


## 1️⃣ Monthly Sales Trend (2014–2017 Combined)


<img width="900" height="640" alt="unnamed-chunk-10-1" src="https://github.com/user-attachments/assets/4644a11e-d341-49aa-b590-d41b1c54ee6b" />
<img width="900" height="640" alt="unnamed-chunk-12-1" src="https://github.com/user-attachments/assets/acba1f23-ae9f-47e4-9c49-617c01d1e066" />





**Insight**:

- Sales consistently peak in Novemberand December, indicating strong seasonal demand. March and September are secondary mini-peaks.

- The trend line shows overall upward movement, suggesting year-over-year growth.

## 2️⃣ Top 5 Sub-Categories Driving Sales in Peak Months of Latest Year (2017)


<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/883fc650-d8d5-48c6-8576-878a3b451856" width="500">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/7790f2d8-e7b7-456d-8c99-02aa2753e691" width="500">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/555ce73b-3322-4124-95ce-701b54f244a1" width="500">
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/f4cbe747-2709-48b5-b49b-980d277dbf87" width="500">
    </td>
  </tr>
</table>


March 2017
- Sales are highly concentrated in Technology, with Copiers alone contributing ~35% of total monthly sales.
- Indicates large one-off or B2B purchases, rather than broad consumer demand.
- Furniture and Office Supplies play a minimal role during this period.


September 2017
- Chairs and Phones emerge as dual sales leaders, showing strong demand across Furniture and Technology.
- Sales distribution becomes more balanced, reducing reliance on a single sub-category.
- Binders stand out as a key Office Supplies contributor.


November 2017
- Phones lead sales, consistent with pre-holiday purchasing behavior.
- Furniture (Chairs and Tables) jointly account for a significant share, reflecting higher-value purchases.
- Sales drivers are well diversified across categories.


December 2017
- Chairs dominate December sales, suggesting strong year-end corporate or home-office spending.
- Storage remains consistently important toward year-end.
- Technology maintains presence but is less dominant than earlier months.


**Overall Business Insights**
- Sales drivers are strongly seasonal, shifting from Technology-heavy (early year & pre-holiday) to Furniture-heavy (year-end).
- Copiers, Phones and Chairs are consistently high-impact products and major revenue levers.
- Year-end sales show greater diversification, indicating broader purchasing behavior rather than dependence on a single sub-category.


**💡 Business Recommendations**
- **Align inventory and promotions with seasonality**: prioritize Technology in Q1/Q4-early, Furniture in Q4.
- **Target B2B clients** with bundled or volume discounts for Copiers and Chairs.
- **Leverage pre-holiday demand** by promoting Phones earlier in Q4 to maximize November performance.
- **Strengthen cross-selling** between Furniture and Office Supplies during peak corporate purchasing periods.


## 3️⃣ Profitability by Product Sub-Category

<img width="1344" height="960" alt="unnamed-chunk-17-1" src="https://github.com/user-attachments/assets/d5f8a397-ea6b-40db-a53f-f94a4d6f9388" />


Key Profit Drivers
- Technology dominates profitability: Copiers, Phones, and Accessories generate the highest profits.
- Office Supplies (Paper, Binders, Storage) provide stable, mid-level profits.
- Chairs are the only Furniture sub-category with strong positive profit.


Low or Negative Profit Areas
- Tables show significant losses, making them the largest profit drain even though being a strong sales driver in some months.
- Bookcases and Supplies are slightly unprofitable, suggesting pricing or cost inefficiencies.
- Machines generate low profit relative to their Technology peers.

**💡 Overall Insights & Recommandation**
- High sales not equal to high profit: some high-revenue sub-categories (like tables) negatively impact overall profitability.
- Technology offers high sales and high profit margins, they’re the safest and most reliable products for the company.
- Furniture profitability is uneven, requiring sub-category-level strategy rather than category-wide decisions.

## 4️⃣ Profit Margin Distribution

<img width="1344" height="960" alt="Distribution_of_Profit_Margin_per_Order-1" src="https://github.com/user-attachments/assets/30021f4b-3bdb-499a-aa96-842f79e0ec49" />


- Most orders make a small to moderate profit.
- There are some extreme losses, but they’re rare.
- Overall, the average profit is positive, meaning losses come from a few bad orders, not the whole business.

## 5️⃣ Profit by Region (with Margin %)

<img width="1344" height="960" alt="unnamed-chunk-24-1" src="https://github.com/user-attachments/assets/f1f301bf-0017-4a37-a7ee-849072ce1fc2" />

- West is the strongest region: it makes the most profit and has the highest profit margin (14.9%).
- East also performs well, with solid profit and a healthy margin (13.5%).
- South is average: makes money, but margins are lower (11.9%).
- Central is the weakest region, with the lowest profit and margin (7.9%).


**💡 Recommendation**:
- West: Keep current strategy and continue focusing on high-profit products.
- East: Make small pricing and cost improvements to close the gap with West.
- South: Reduce heavy discounting and prioritize higher-margin products.
- Central: Review costs and pricing before trying to increase sales.


## 6️⃣ Profit by Customer Segment (with Margin %)


<img width="1344" height="960" alt="unnamed-chunk-27-1" src="https://github.com/user-attachments/assets/e66c44fd-98b5-406b-a040-3d3ee1616948" />

- Consumer generates the highest total profit, but has the lowest margin (11.5%).
- Corporate shows a good balance of strong profit and solid margin (13%).
- Home Office has the highest margin (14%) but the lowest total profit, likely due to lower sales volume.

**💡 Recommendations**:
- Consumer: Improve margins by reducing discounts and pushing higher-margin products.
- Corporate: Continue targeting this segment as it provides stable and efficient profitability.
- Home Office: Grow sales volume while maintaining high margins through targeted promotions.


## 7️⃣ Sales vs. Profit Relationship

<img width="1344" height="960" alt="unnamed-chunk-16-1" src="https://github.com/user-attachments/assets/ec2767c1-cdfe-4691-b465-4cd894a834f3" />

- Higher sales generally lead to higher profit, but the relationship is not strong.
- Some high-sales orders still lose money, showing that selling more doesn’t always mean earning more.
- Profit varies widely at similar sales levels, suggesting pricing and discounts matter a lot.
- Some high-sales orders still produce losses due to heavy discounting or high costs.


## 8️⃣ Discount vs. Profit Relationship
<img width="1344" height="960" alt="unnamed-chunk-17-1" src="https://github.com/user-attachments/assets/0aba3df9-6735-484b-9680-97bb86603cc4" />

- Higher discounts clearly reduce profit.
- Large discounts are often linked to negative profit (losses).
- Most high-profit orders happen at low or zero discounts.


## 9️⃣ Machine Learning: Profitability Prediction (Logistic Regression)

#### Goal
- Predict whether an order will be profitable or unprofitable before it is completed.
- Should we allow this order or discount? 

#### Impactful Features

Numeric: Discount, Quantity
Categorical: Category, Region

#### Model

- Logistic Regression (GLM with binomial family)
- Trained using an 80/20 train–test split
- Random seed set for reproducibility

#### Key Model Insights

- Discount is the strongest negative predictor of profitability
  - Higher discounts greatly reduce the chance of making a profit.

- Higher quantity slightly increases the probability of profitability.

- Technology and Office Supplies categories are more likely to be profitable than Furniture.

- West, South, and East regions have higher profitability likelihood than the baseline region.

- Sales amount itself is not a strong predictor once discount and category are considered.

#### Model Performance
- Test accuracy: ~94%


# 📌 Summary of Business Recommendations
- **Control discounting aggressively**: High discounts are the main driver of unprofitable orders and should require approval or review.
- **Prioritize high-margin products**: Focus growth on Technology and Office Supplies rather than pushing low-margin Furniture items.
- **Shift focus from sales volume to profit quality**: High sales do not guarantee profit; pricing decisions matter more than order size.
- **Invest in strong regions**: Expand strategies used in West and East regions while improving cost control in weaker regions.
- **Use predictive analytics for decision support**: Apply the profitability prediction model to flag risky orders before they are accepted.
