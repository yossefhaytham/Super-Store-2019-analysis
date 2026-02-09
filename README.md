# SuperStore 2019 Analysis

## Project Overview
This project represents an end-to-end data analysis solution for the SuperStore 2019 dataset. The primary goal was to transition from raw transactional records to a professional Business Intelligence dashboard. The project focuses on performance tracking, financial forecasting, and product segmentation to aid stakeholders in making data-driven decisions.

## Data Resources
You can access the datasets used and generated in this project via the links below:

* **Original Data Source:** [Download Orginal Data](https://github.com/yossefhaytham/Super_Store_2019_analysis/tree/main/orginal_data)
* **Processed Analysis File:** [Download Final Data Model & Dashboard](https://github.com/yossefhaytham/Super_Store_2019_analysis/tree/main/SuperStore-2019-analysis)

## Problem Statement & Analytical Logic
This analysis was driven by specific business questions regarding operational efficiency and product strategy. The following core problems were addressed:

### 1. Branch Performance & Target Variance Analysis
**The Business Question:**
The company operates across four distinct branches. The critical challenge was not just to see how much they sold, but to determine if they met their financial potential compared to expectations.

**The Analytical Approach:**
* I analyzed the performance of the four branches individually to isolate high-performing locations from those requiring operational support.
* **Actual vs. Expected Profit:** I calculated the gap between the *Realized Profit* (what was actually earned) and the *Expected Profit* (the financial target).
* This variance analysis allows management to see exactly which branch missed the target and by what margin, moving beyond simple sales totals to actual financial health.

### 2. Product Category Optimization
**The Business Question:**
With a wide range of products, it is difficult to determine which segments are the true drivers of company growth versus those that are simply moving volume without generating significant return.

**The Analytical Approach:**
* I performed a deep-dive analysis into the main product categories to identify the "Best Performing Category."
* The analysis looked at two dimensions:
    1.  **Revenue Generation:** Which category brings in the most cash flow?
    2.  **Profitability:** Which category retains the most money after costs?
* This logic helps in deciding where to allocate marketing budget and inventory space to maximize the Return on Investment (ROI).

## Technical Workflow
The project was executed using a professional Excel BI pipeline:

1.  **Data Extraction & Cleaning (Power Query):**
    * Connected to the raw data source and consolidated files.
    * Performed rigorous data cleaning: handling missing values, standardizing text formats, and removing duplicates.
    * Applied conditional logic to create new classification columns necessary for the analysis.

2.  **Data Modeling (Power Pivot):**
    * Designed a Star Schema data model by normalizing flat tables into Fact Tables (Transactions) and Dimension Tables (Lookups).
    * Established "One-to-Many" relationships to ensure accurate filtering and high-performance calculations.

3.  **DAX Calculations:**
    * Created Measure calculations to dynamically compute KPIs such as Total Sales, Total Profit, Profit Margin %, and Variance to Target.

4.  **Visualization & Interaction:**
    * Designed a user-friendly dashboard layout.
    * Integrated Slicers and Timelines to allow users to filter the entire report by Branch, Year, or Category instantly.

## Dashboard Preview
Below is the static view of the final dashboard design:

![Dashboard Static](https://raw.githubusercontent.com/yossefhaytham/Super_Store_2019_analysis/refs/heads/main/resource/IMG-For-dashboard.jpg)

## Interactive Demonstration
The following GIF demonstrates the interactivity of the dashboard, showing how the "Actual vs. Expected" logic updates dynamically when filtering by different criteria:

![Dashboard Interactive](https://raw.githubusercontent.com/yossefhaytham/Super_Store_2019_analysis/refs/heads/main/resource/Super_Store_2019_GIF.gif)
