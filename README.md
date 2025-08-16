# elabs_probation

# 🛍️ Fashion Boutique EDA Project

Welcome to the **Fashion Boutique Exploratory Data Analysis (EDA)** project—an end-to-end analytical journey that converts raw boutique sales data into actionable retail insights using Python, Pandas and visualization libraries.

***

## 🚦 Project Pipeline  
Data Source → Data Loading (Pandas) → Data Preprocessing → Exploratory Data Analysis → Insight Generation

***

## 📂 Dataset Overview  

- **Rows:** ≈ 2,000  
- **Columns:** 14  
- **File:** Excel workbook (`Fashion_Boutique_Dataset.xlsx`, sheet `Fashion_Data`)  

Key fields:  
`Product_ID`, `Category`, `Brand`, `Season`, `Original_Price`, `Current_Price`, `Markdown_Percentage`, `Purchase_Date`, `Stock_Quantity`, `Customer_Rating`, `is_returned`, `Return_Reason`.

***

## 🔍 Data Preparation  

- **Date Handling** – Converted `Purchase_Date` to `datetime` for monthly analysis.  
- **Missing Values**  
  - Filled `Customer_Rating` nulls with 0 (placeholder strategy).  
  - Retained empty `Return_Reason` for non-returns; trimmed others.  
- **Feature Engineering** – Added `Month` (YYYY-MM) to support seasonality and revenue trend plots.

***

## 🕵️ Exploratory Data Analysis (EDA)

### Categorical Insights  
- Revenue and unit sales by **Category**, **Brand**, and **Season**.  
- Return distributions across **Return_Reason** buckets.

### Numerical Insights  
- Pricing structure: `Original_Price`, `Current_Price`, `Markdown_Percentage`.  
- Operational metrics: `Stock_Quantity`, `Customer_Rating`.

### Relationships & Trends  
- **Revenue Concentration** – *Outerwear* and *Shoes* drive the largest share of sales value.  
- **Seasonality** – Peak revenue in August aligns with monsoon-season promotions in Bhubaneswar.  
- **Price-Markdown Dynamics** – Steeper markdowns strongly depress current prices, especially in clearance categories like *Shoes*.  
- **Returns** – Size issues dominate, signalling a need for better fit guidance.

***

## 📊 Visualization Suite  

| # | Visualization | Purpose / Key Insight |
|---|---------------|-----------------------|
| **1** | **Bar Chart – Total Revenue by Category** | Highlights top-earning categories; *Outerwear* leads. |
| **2** | **Boxplot – Price Distribution by Season** | Reveals higher winter median prices and summer discounts. |
| **3** | **Line Plot – Monthly Revenue Trend** | Shows August revenue spike; useful for promotion timing. |
| **4** | **Scatter – Original vs Current Price (color: Markdown%)** | Exposes markdown strategy impact on final pricing. |
| **5** | **Pie Chart – Return Reasons** | Quantifies why customers return items; size issues ≈ 30-40%. |
| **6** | **Heatmap – Feature Correlations** | Confirms negative correlation between markdown and price; weak links elsewhere. |

*Visuals produced with Matplotlib, Seaborn, and Plotly.*

***

## 🧰 Toolstack  

- **Data Manipulation:** Pandas  
- **Visualization:** Matplotlib, Seaborn, Plotly  
- **Environment:** Jupyter Notebook (Python 3.x)

***

## 🎯 Key Takeaways  

- **Inventory Focus:** Stock lighter apparel year-round for Bhubaneswar’s tropical climate; maintain premium Outerwear for revenue.  
- **Pricing Strategy:** Optimize markdown timing to protect margins while clearing inventory.  
- **Return Mitigation:** Invest in enhanced sizing guides and quality checks to reduce size- and quality-related returns.  
- **Future Work:** Integrate customer feedback loops and predictive models (e.g., demand forecasting) to extend insights.

***

## 📬 Contact  

Questions or feedback? Reach out to **Shantanu Roy – shantanur003@gmail.com**

***


