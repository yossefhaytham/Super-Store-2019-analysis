# SuperStore 2019 Analysis

## Project Overview
This project transforms raw sales data from "SuperStore 2019" into a professional Business Intelligence dashboard. The goal is to track performance, forecast financial targets, and identify the best products. This dashboard helps stakeholders make smart decisions based on real data.

## Data Resources
You can access the datasets used and generated in this project via the links below:

* **Original Data Source:** [Download Original Data](https://github.com/yossefhaytham/Super_Store_2019_analysis/tree/main/orginal_data)
* **Processed Analysis File:** [Download Final Data Model & Dashboard](https://github.com/yossefhaytham/Super_Store_2019_analysis/tree/main/SuperStore-2019-analysis)

## Problem Statement & Analytical Logic
This analysis addresses specific business challenges regarding efficiency and strategy. I focused on three core areas:

### 1. Branch Performance & Targets
**The Business Question:**
The company has four branches. We need to know not just how much they sold, but if they met their financial goals.

**The Solution:**
* I analyzed each branch individually to separate top performers from those needing help.
* **Actual vs. Expected Profit:** I calculated the difference between the profit we made and the profit we *expected* to make. This highlights exactly which branches are underperforming.

### 2. Product Category Optimization
**The Business Question:**
With so many products, it is hard to know which ones actually drive growth and which ones are just "busy work."

**The Solution:**
* I analyzed product categories to find the "Best Performing Category."
* I looked at **Revenue** (Cash flow) and **Profitability** (Real earnings). This helps decide where to spend the marketing budget.

### 3. The Impact of Discount on Profitability
**The Business Question:**
Discounts drive sales, but they also eat into profits. We need to understand the "Safe Zone" for discounting.

**The Logic Visualization:**
The diagram below illustrates the business rule used in this analysis:

![Profit vs Discount Logic](https://github.com/yossefhaytham/Super-Store-2019-analysis/blob/main/resource/roles.png)

* **The Concept:** There is a baseline "Actual Cost" for every product.
* **Positive Profit (+):** If we apply a small discount, the selling price stays *above* the cost. We make a profit.
* **Negative Profit (-):** If the discount is too big, the selling price falls *below* the cost. This results in a loss.
* **Goal:** The dashboard helps monitor these levels to ensure discounts do not result in selling at a loss.

## Technical Workflow
The project was built using a professional Excel BI pipeline:

1.  **Data Cleaning (Power Query):**
    * Connected to raw files and fixed missing values.
    * Removed duplicates and standardized text formats.
    * Created custom columns to classify data for analysis.

2.  **Data Modeling (Power Pivot):**
    * Built a "Star Schema" model (separating Transactions from Lookup tables).
    * Created relationships to ensure the dashboard filters work correctly and quickly.

3.  **Calculations (DAX):**
    * Wrote formulas to calculate Total Sales, Profit Margins, and Variance automatically.

4.  **Dashboard Design:**
    * Created a clean layout with interactive Slicers and Timelines.
    * Users can filter by Branch, Year, or Category instantly.

## Dashboard Preview
Below is the static view of the final dashboard design:

![Dashboard Static](https://raw.githubusercontent.com/yossefhaytham/Super_Store_2019_analysis/refs/heads/main/resource/IMG-For-dashboard.jpg)

## Interactive Demonstration
The following GIF demonstrates the interactivity of the dashboard, showing how the logic updates dynamically when filtering:

![Dashboard Interactive](https://raw.githubusercontent.com/yossefhaytham/Super_Store_2019_analysis/refs/heads/main/resource/Super_Store_2019_GIF.gif)
