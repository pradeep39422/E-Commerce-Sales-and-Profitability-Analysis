# 📊 E-Commerce Sales & Profitability Analysis

Hey there! Thanks for dropping by my repository. I put this project together to showcase how raw e-commerce data can be translated into actual business strategy. As a computer science engineering student deeply interested in data analytics, I wanted to move beyond just writing code and actually uncover the "why" behind the numbers—figuring out what product lines are making money, where the business is taking losses, and how sales targets are being forecasted. 

## 🛠️ The Goal
The main objective here was to answer some real-world business questions using Python (`pandas` and `numpy`) and a bit of spreadsheet magic. Specifically, I looked at:
1.  **Product Performance**: Which items are actually driving profit versus just driving revenue?
2.  **Target Forecasting**: How well is the company predicting its future sales?
3.  **Regional Disparities**: Are there certain states where doing business is actually costing the company money?

## 📂 What's in this Repo?
*   `solution_assign.ipynb`: The Jupyter Notebook where all the heavy lifting happens. This is where I merge the datasets, clean things up, group the data, and run the calculations.
*   `solution_spreadsheet_2.xlsx`: A polished spreadsheet containing the final data cuts, pivot tables, and charts to visualize the findings. 
*   **The Data**: Three raw datasets (`List_of_Orders.xlsx`, `Order_Details.xlsx`, `Sales_target.xlsx`) containing transaction logs, itemized order details, and projected sales targets.

---

## 💡 What I Found (The Highlights)

### 1. Clothing is the Cash Cow 👕
I merged the order history and order details to see the true profit margins. 
*   **The Winner**: Clothing. It didn't have the highest total sales (Electronics won that), but it had the highest profit margin (**8.03%**) and the most consistent order volume. 
*   **The Loser**: Furniture. Despite doing ₹127K in revenue, it only brought in ₹2,298 in profit. That’s a margin of just **1.81%** (or about ₹12 per order). 
*   *My take:* Furniture is bulky and expensive to ship. The logistics costs are eating the margins alive. 


### 2. The Forecasting Got Weird in April 📉
I tracked the month-over-month (MoM) target sales for the struggling Furniture category. 
*   Generally, the sales targets increased by a very steady 0.8% to 1.8% every single month. 
*   However, in **April**, the target suddenly plummeted by **-11.86%**. 
*   *My take:* Uniformly raising targets by 1% a month isn't realistic. The company needs to use historical data and factor in seasonality rather than just drawing a straight line up.

### 3. Punjab is Operating at a Loss 🚨
I isolated the top 5 states by order volume to see where the business was strongest. 
*   **Maharashtra** is doing great, bringing in the highest average profit per order (₹68).
*   **Punjab** is a massive problem. Despite having a high order count, they are averaging a **loss of -₹24.36 per order**. 
*   *My take:* Punjab needs an immediate audit. High order volume combined with negative profit means the company is literally paying people to buy their products there. They either need to rethink their shipping logistics in the region, stop aggressive discounting, or investigate high return rates. 

## 💻 Tech Stack
*   **Python**: `pandas` (for merging, grouping, and logic), `numpy`.
*   **Excel/Google Sheets**: For pivot tables and final presentation. 

— **Pradeep Kumar**
