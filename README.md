# 🌍 Sales Performance & Market Expansion For A Global Superstore | Power BI

![background](https://github.com/user-attachments/assets/c712d9dd-90e5-4347-92d6-5d5a1971d253)



## Table of Contents
- [📌 Background & Overview](#-background--overview)
- [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)
- [🧠 Design Thinking Process](#-design-thinking-process)
- [📊 Key Insights & Visualizations](#-visualizations)
- [🚀 Insight & Recommendation](#insight--recommendation)

---

## 📌 Background & Overview

**Objective:**

#### **What is this project about?**
This project analyzes the **Global Superstore Sales** dataset to build a **Power BI dashboard** that evaluates business performance across regions, product categories, and customer segments.

The analysis integrates:
- **Orders**: transactional sales data  
- **People**: sales representatives by region  
- **Returns**: product return data impacting profitability  

The goal is to provide **data-driven insights** that support strategic decision-making related to revenue growth, profitability, and market expansion.

---

#### **Who is this project for?**
- Data analysts and business analysts seeking actionable insights  
- Sales and marketing teams evaluating product performance and regional growth  
- Route-to-market teams optimizing distribution strategies and market reach  
- Senior managers and decision-makers supporting strategic planning  

---

#### **Business Questions**
- What is the current business performance across regions and product categories?  
- Which markets present the strongest opportunities for revenue and ROI expansion?  
- Which products and categories should be prioritized for profitable growth?  
- Where are profitability risks driven by costs, returns, or low margins?  

## 📂 Dataset Description & Data Structure

### **📌 Data Source** 

- **Source**: Kaggle  
- **Size**: The **Orders** table contains **51,290** records.  
- **Format**: CSV  

### 📊 **Data Structure & Relationships**  

#### 1️⃣ **Tables Used:**  
The dataset consists of **three tables**:  

- 🛒 **Orders** – Contains detailed transaction and customer information (**51,290 records**).

<details>
<summary> <strong>Table 1: Orders</strong></summary>

| Column Name       | Data Type   | Description                              |
|------------------|------------|------------------------------------------|
| `Order ID`      | `VARCHAR`   | Unique identifier for each order.       |
| `Order Date`    | `DATE`      | Date when the order was placed.         |
| `Ship Date`     | `DATE`      | Date when the order was shipped.        |
| `Ship Mode`     | `VARCHAR`   | Shipping method used for delivery.      |
| `Customer ID`   | `VARCHAR`   | Unique identifier for each customer.    |
| `Customer Name` | `VARCHAR`   | Full name of the customer.              |
| `Segment`       | `VARCHAR`   | Customer segment (e.g., Consumer, Corporate). |
| `City`         | `VARCHAR`   | City where the order was placed.        |
| `State`        | `VARCHAR`   | State where the order was placed.       |
| `Country`      | `VARCHAR`   | Country where the order was placed.     |
| `Postal Code`  | `VARCHAR`   | Postal code of the shipping address.    |
| `Market`       | `VARCHAR`   | Market region (e.g., APAC, EMEA).       |
| `Region`       | `VARCHAR`   | Geographical region of the order.       |
| `Product ID`   | `VARCHAR`   | Unique identifier for each product.     |
| `Category`     | `VARCHAR`   | Product category (e.g., Furniture, Office Supplies). |
| `Sub-Category` | `VARCHAR`   | Sub-category of the product.            |
| `Product Name` | `VARCHAR`   | Name of the product ordered.            |
| `Sales`        | `DECIMAL`   | Revenue generated from the order.       |
| `Quantity`     | `INT`       | Number of items ordered.                |
| `Profit`       | `DECIMAL`   | Profit earned from the order.           |

</details>

- 🔄 **Returns** – Stores data on returned orders.

<details>
<summary> <strong>Table 2: Returns</strong></summary>

| Column Name  | Data Type | Description |
|--------------|-----------|-------------|
| `Returned`   | `VARCHAR` | Indicates whether the order was returned (e.g., 'Yes' or 'No'). |
| `Order ID`   | `VARCHAR` | Unique identifier for each order. |

</details>
  
- 👥 **People** – Holds information about sales representatives.

<details>
<summary> <strong>Table 3: People</strong></summary>

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| `Person`    | `VARCHAR` | Name of the salesperson. |
| `Region`    | `VARCHAR` | Geographic region where the salesperson operates. |

</details>

#### 2️⃣ Data Relationships:
<img width="996" height="802" alt="Data Modeling" src="https://github.com/user-attachments/assets/d9ac8578-a199-4739-8a23-a3ea3c1a5ae1" />

## 🧠 Design Thinking Process 
### 1️⃣ Empathize  
#### 5W1H
| Question | Details |
|---------|---------|
| **Who will use this dashboard?** | Senior Management <br> Sales Manager <br> Marketing Manager |
| **What problem does this dashboard solve?** | Help stakeholders understand business performance quickly <br> Identify where to grow and what to focus on for market expansion <br> Detect inefficient markets, products, and sales execution |
| **When & where will stakeholders use this dashboard?** | Weekly and monthly business review meetings <br> Executive decision-making discussions <br> Individual analysis before proposing business strategies |
| **Why is this analysis needed?** | Business operates across multiple markets with uneven performance <br> Growth opportunities exist, but not all growth is profitable <br> Stakeholders need data-backed insights, not raw reports |
| **How will stakeholders make decisions using this dashboard?** | Set growth and expansion priorities <br> Allocate resources across markets and products <br> Optimize sales and product strategies <br> Review outcomes and iterate decisions |

| Key Item | Description |
|----------|-------------|
| **Primary Stakeholder** | Sales Manager |
| **Problem Statement** | Use data to identify profitable growth opportunities and support market expansion decisions. |

#### Empathy Map

| Category | Details |
|----------|---------|
| **Thinking & Feeling** | There is a lot of data, but not enough clear insight. <br> Where are we missing growth opportunities? <br> Are we scaling the right markets and products? <br> Revenue is growing, but is this growth sustainable? |
| **Seeing** | Revenue is increasing across markets <br> Performance varies significantly by market and product <br> Global markets show different growth and margin patterns <br> No clear prioritization of strategic products or markets |
| **Saying** | Show me the full picture. <br> Which markets and products actually drive profit? <br> Don’t give me numbers, give me insights. <br> If a product is underperforming, be clear about it. |
| **Doing** | Request concise executive summaries <br> Compare performance across markets and products <br> Ask follow-up questions on low-margin or high-return areas <br> Focus on expansion and optimization decisions |
| **Pains** | Too much data, not enough clarity <br> Difficulty identifying profitable growth <br> Risk of expanding low-margin segments <br> Lack of a clear expansion strategy |
| **Gains** | Clear visibility into business performance <br> Data-driven market and product prioritization <br> Ability to track growth and risk continuously <br> Stronger confidence in strategic decisions |

#### Stakeholder Needs

| Area | Key Questions |
|------|---------------|
| **Market** | Which markets are growing the fastest? <br> Which markets generate the most profit? <br> Which markets have growth potential but operational risk? |
| **Customer** | Which customer segments drive revenue and profit? <br> Where does demand come from across markets? <br> Are return rates increasing as volume scales? |
| **Product** | Which products are best-sellers by market? <br> Which products generate the highest profit margins? <br> Which products should be prioritized or deprioritized during expansion? |
| **Sales** | Who are the top-performing sales agents by profitability? <br> Which sales agents drive sustainable growth? <br> How does sales performance vary across markets? |


## 📊 Visualizations

### 🔍 Dashboard Preview

### I. Overview
<img width="1517" height="846" alt="Overview" src="https://github.com/user-attachments/assets/25aa8877-d3ac-445b-9c19-9781abe54eab" />

#### 💡 Key Business Insights

- **Profitable growth confirmed:** Revenue and profit are growing in lockstep (+51.5% and +52.3% YoY), indicating that growth is value-driven rather than achieved at the expense of margins.

- **Margin stability signals maturity:** Profit margin remains stable at approximately **11.6%**, suggesting a healthy but maturing growth phase where margin expansion is beginning to level off.

- **Strong demand with improving execution:** Order volume increased significantly (+51.7% YoY) while the return rate declined to **4.68%**, reflecting strong customer demand supported by better operational execution.

- **Revenue concentration in core markets:** APAC, EU, and the US account for the majority of revenue contribution, functioning as the company’s primary revenue engines.

- **Efficiency not always driven by scale:** Several smaller markets achieve higher relative margins, highlighting that scale does not necessarily equate to operational efficiency.

- **Product mix impacts profitability:** Technology and Office Supplies generate most of the revenue, while Furniture consistently underperforms on margin, indicating that product mix is a key driver of overall profitability.

- **Different market growth dynamics:** Emerging markets (EMEA, Africa) show strong growth momentum from a smaller base, whereas core markets exhibit steadier, more mature growth patterns.

- **Return risk varies by product category:** Office Supplies combine high demand with lower return risk, while Technology and Furniture carry higher return exposure, increasing operational risk as volume scales.


### II. Market
<img width="1522" height="856" alt="Market Analyst" src="https://github.com/user-attachments/assets/bf065326-d7fa-4b51-82b7-40cfb81d6446" />

#### 💡 Insights

- **Overall performance remains strong:** Total revenue reached **$12.64M** with **$1.47M profit** and a stable **11.61% profit margin**, indicating healthy overall business performance.

- **Growth is volume-driven, not value-driven:** Revenue growth is primarily driven by increasing order volume, while **AOV remains flat (-0.1% YoY)**, suggesting limited pricing or value uplift.

- **Execution quality remains stable:** Return rate continues to trend downward, indicating consistent execution quality across markets despite rapid growth.

- **Revenue concentration in core markets:** APAC, EU, and the US account for the majority of both revenue and profit, functioning as the company’s core scale markets.

- **Efficiency varies by market:** Profitability differs significantly across regions, confirming that higher revenue scale does not necessarily translate into higher efficiency.

- **Canada as a structural outlier:** Canada operates as a **high-margin, low-scale market (~26.6% margin)**, making it structurally different from other regions.

- **Emerging market growth potential:** EMEA and Africa exhibit the highest revenue growth rates (**~59.8% and ~56.5%**), signaling strong expansion potential from a smaller base.

- **Higher return risk in select markets:** LATAM and the US show elevated return rates (**~5.8–5.9%**), introducing higher operational and customer-fit risk as volume scales.

- **Long-term growth structure:** Over time, overall growth is structurally driven by core markets, while emerging markets contribute gradually without introducing significant volatility.

- **Profit per customer dynamics:** Markets with higher AOV (APAC, EU) generate higher profit per customer, while Africa and Canada underperform on this metric, indicating that pricing alone does not determine customer profitability.


### III. Product Analysis
<img width="1518" height="852" alt="Product Analysis" src="https://github.com/user-attachments/assets/d3e40db6-bf65-49d4-a997-ab6280d5749a" />

####  💡 Insights

- **Growth driven by volume, not value:** Revenue growth is primarily volume-driven, as **AOV declined slightly (–0.1% YoY)** while transaction volume continued to increase.

- **Revenue concentration by sub-category:** Revenue is highly concentrated in a small number of sub-categories, led by **Phones, Copiers, Chairs, and Bookcases**.

- **Revenue does not equal efficiency:** Profitability varies significantly across sub-categories, confirming that high revenue does not necessarily translate into high efficiency.

- **Margin drag identified:** **Tables** act as a clear margin drag, generating **negative profit (~–$64K)** with a **–8.46% margin**.

- **Strong Pareto effect:** Pareto analysis confirms a clear **80/20 pattern**, where a limited set of sub-categories contributes approximately **80% of total revenue**, while the remaining products add marginal value.

- **Volume–profit mismatch:** Order volume does not consistently translate into profit; several moderate-volume sub-categories deliver strong profitability, while some high-volume categories scale inefficiently.

- **Product–market fit differences:** Product performance varies meaningfully by market, indicating differences in product–market fit and limiting the effectiveness of a uniform global product strategy.


### IV. Sales Agent
<img width="1513" height="855" alt="Sales Agents" src="https://github.com/user-attachments/assets/6886f950-6ca0-4f4c-b81f-84dcfc8214d0" />

#### 💡 Insights

- **Strong contribution to overall growth:** Sales performance supports continued business growth, with **$12.64M revenue (+51.5% YoY)** and **$1.47M profit (+52.3% YoY)**, while profit margin remains stable at **11.61%**.

- **Uneven revenue contribution across agents:** Revenue generation is highly concentrated, with a small group of sales agents driving a disproportionate share of total sales.

- **Revenue does not equal profitability:** High revenue performance at the agent level does not consistently translate into high profitability.

- **Execution risk among high-volume agents:** Several agents generate strong sales volume but operate with lower margins or higher return rates, increasing execution and customer-fit risk.

- **Efficiency-driven agent performance:** Other agents deliver moderate revenue with stronger margins and lower return exposure, indicating more efficient and sustainable selling behavior.

- **Product mix drives outcomes:** Sales performance is strongly influenced by product mix, not solely by selling activity or order volume, highlighting the importance of aligning incentives with profitable products.


## Insight & Recommendation

## 🚀 Strategic Framework Summary

| Strategy Area | Key Actions |
|---------------|-------------|
| **Market Strategy** | Focus on expanding within existing markets instead of entering completely new ones. <br> Continue investing in core markets (APAC, EU, US) where revenue is large and stable. <br> Expand carefully in high-growth markets (EMEA, Africa) to capture growth while controlling risk. <br> Treat Canada as a high-margin niche market, prioritizing profitability over volume growth. |
| **Product Strategy** | Prioritize high-performing products (e.g., Phones, Copiers) that consistently generate revenue and profit. <br> Avoid scaling products that drive revenue but hurt margins (e.g., Tables with negative profit). <br> Simplify the product portfolio by focusing on the small group of products that drive most revenue. |
| **Risk & Quality Control** | Monitor return rate alongside revenue growth to avoid scaling low-quality or high-risk segments. <br> Investigate markets or products with high growth but elevated return rates before expanding further. |
| **Sales Execution** | Evaluate sales performance using profitability metrics rather than revenue alone. <br> Encourage sales teams to focus on selling the right products, not just increasing order volume. <br> Replicate selling patterns from high-margin, low-return performers across teams. |
| **Business Impact** | Enables profitable and controlled growth. <br> Reduces risk from over-expansion. <br> Aligns market, product, and sales decisions with long-term value creation. |


