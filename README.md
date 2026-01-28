# 🌍 Sales Performance & Market Expansion For A Global Superstore | Power BI

![background](https://github.com/user-attachments/assets/c712d9dd-90e5-4347-92d6-5d5a1971d253)



## Table of Contents
1. [📌 Background & Overview](#background--overview)
2. [📂 Dataset Description & Data Structure](#dataset-description--data-structure)
3. [📊 Key Insights & Visualizations](#key-insights--visualizations)
4. [🔎 Final Conclusion & Recommendation](#final-conclusion--recommendation)

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



## 📊 Visualizations

### 🔍 Dashboard Preview

### I. Overview
<img width="1517" height="846" alt="Overview" src="https://github.com/user-attachments/assets/25aa8877-d3ac-445b-9c19-9781abe54eab" />

### II. Market
<img width="1522" height="856" alt="Market Analyst" src="https://github.com/user-attachments/assets/bf065326-d7fa-4b51-82b7-40cfb81d6446" />

### III. Product Analysis
<img width="1518" height="852" alt="Product Analysis" src="https://github.com/user-attachments/assets/d3e40db6-bf65-49d4-a997-ab6280d5749a" />

### IV. Sales Agent
<img width="1513" height="855" alt="Sales Agents" src="https://github.com/user-attachments/assets/6886f950-6ca0-4f4c-b81f-84dcfc8214d0" />


## Insight & Recommendation
## 📊 Market Optimization Summary

### 🌍 **Market Overview**
The company has established a presence in all major global markets.  
Rather than entering new ones, it is recommended to **expand within existing markets**.

**🇨🇦 Canada** is recommended for growth:  
Despite strong **YoY growth** and **healthy profit margin**, its **customer base remains limited**, resulting in relatively low revenue.  
👉 **Develop a strategy to broaden customer reach in Canada.**

---

### 👩‍💼 **Sales Agent**
**Nicole Hansen** manages the **Canadian market**.  
Revenue, profit margin, and YoY growth are all performing well.  
👉 **Continue her oversight of this market.**

---

### 🛒 **Product Strategy**
**Phones**, **Copiers**, **Chairs**, and **Bookcases** are the company’s best-selling products overall.  
👉 **Position Copiers and Phones as strategic products moving forward.**

---

### 📌 **Current Market Optimization by Region**

#### 🌏 **APAC Market**
- Best performer overall.  
- Continue **heavy investment**, focusing on **Technology** and **Furniture** (each > $1.3M revenue).  
- **Improve return rate (6–7%)** to enhance margins.

#### 🇪🇺 **EU Market**
- ~$3M revenue, **10–13% margin**, and ~55% YoY growth.  
- Expand **Technology** and **Office Supplies** while maintaining **product quality** (return rate ~6%).

#### 🇺🇸 **US Market**
- Profitability is strong, but **revenue scale lags**.  
- Expand product offerings or increase marketing to drive **top-line growth**.

#### 🌎 **LATAM Market**
- Strong **growth** but **low margins**.  
- Invest cautiously with focus on **cost control** and **raising AOV** (Average Order Value).

#### 🌍 **Africa & EMEA**
- Underperforming with **high customer counts** but **negative profit**.  
- **Investigate root causes** and consider **corrective measures or market exit.**

---

✅ **Overall Recommendation:**  
Focus on **expanding within high-performing regions (APAC, EU, Canada)** while **optimizing costs and returns** in underperforming ones.
