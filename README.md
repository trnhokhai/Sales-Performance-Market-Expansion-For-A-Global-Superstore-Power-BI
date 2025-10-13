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

**📖 What is this project about?**

This project aims to build a **Power BI dashboard** using the *Global Superstore Sales* dataset, which includes data on transactions (**Orders**), sales representatives (**People**), and product returns (**Returns**).
The goal is to provide senior managers with **data-driven insights** to:

- **Understand current business performance**
 
- **Optimize market expansion strategies**

- **Identify strategic products for growth**

- **Support better decision-making to drive revenue and ROI**


**👤 Who is this project for?**

✔️ Data analysts & business analysts seeking actionable insights.

✔️ Marketing and sales teams focusing on product performance and market growth.

✔️ Route to market team aiming to improve distribution strategies and market reach.


**❓Business Questions:**

✔️ What is the current performance of Superstore?

✔️ Which markets should Superstore expand into to increase revenue and ROI?

✔️ Which products should be prioritized for strategic growth?


**🎯Project Outcome:**

- Revenue increased significantly, but profit margin remained flat, indicating rising costs and limited operational efficiency gains.  
- Canada emerged as a high-margin market (28%) despite low revenue, while Africa and EMEA showed the fastest YoY growth, revealing expansion potential.  
- Oceania and Africa attracted the most new customers, whereas most revenue still came from loyal, returning buyers.  
- Technology led revenue growth and profitability, but return rates in some tech SKUs (e.g., Cisco, Motorola) impacted margins.  
- Products like Copiers delivered the highest profit per unit, while low-performing items (e.g., Suppliers, Furnishings) diluted overall profitability.

By aligning regional and product strategies, senior managers can **scale in high-margin markets**, **invest in scalable profitable categories**, and **optimize acquisition and return management**, driving **sustainable long-term growth**.

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
