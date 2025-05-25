# Supply Chain Data Analysis Project

This project analyzes supply chain data for a skincare company to enhance **efficiency**, **reliability**, and **profitability**. It explores five key areas:

- Demand Forecasting & Sales Insights
- Inventory Optimization
- Supplier & Manufacturing Efficiency
- Quality Control
- Logistics & Cost Efficiency

<!-- Optional: Add a header image here, e.g., ![Supply Chain Analysis](supply-chain.jpg) -->
<!-- Suggestion: Use a free stock image from Unsplash (e.g., search "supply chain" or "data analysis") -->

## Table of Contents

- [Data Source](#data-source)
- [Data Preparation](#data-preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Analysis and Modeling](#analysis-and-modeling)
- [Insights and Recommendations](#insights-and-recommendations)
- [SKU Analysis](#sku-analysis)
- [Customer Analysis](#customer-analysis)
- [Production Analysis](#production-analysis)
- [Shipping Analysis](#shipping-analysis)
- [Supplier Analysis](#supplier-analysis)
- [Transportation Analysis](#transportation-analysis)

## Data Source

The dataset is a CSV file with 100 records and 27 columns, covering product information, sales and customer data, inventory and orders, shipping and logistics, supplier and manufacturing, and quality control. See [`dataset.csv`](dataset.csv) for the data.

## Data Preparation

- **Cleaning:** Reduced columns from 27 to 24; no duplicates or imputation required.
- **Transformations:** Added custom columns for analysis:
  - Stock efficiency
  - Total lead time per SKU
  - Manufacturing costs per unit
  - Transportation costs per unit
  - Profitability and profit/loss for SKUs

## Exploratory Data Analysis (EDA)

Used summary statistics and visualizations to uncover trends and patterns. See the [project documentation](documentation.md) for detailed charts and findings.

<!-- Optional: Add a sample chart image here, e.g., ![EDA Chart](eda-chart.jpg) -->

## Analysis and Modeling

This section is in progress. It will detail analytical techniques, tools, assumptions, and model outputs once completed.

## Insights and Recommendations

### SKU Analysis

**Insights:**

- Top SKUs (`SKU10`, `SKU4`) lead sales, but profitability is low (3.44K profit vs. 87.85K loss).
- Stock gaps and long lead times (e.g., `SKU30`: 90 days) are issues.

**Recommendations:**

- Adjust pricing/costs for low-profit SKUs (e.g., `SKU0`, `SKU22`).
- Optimize stock for high-demand SKUs (e.g., `SKU0`, `SKU4`).
- Reduce lead times with supplier collaboration.
- Enhance forecasting using sales trends.

### Customer Analysis

**Insights:**

- Unknown (46K) and Female (15K) demographics drive sales; Male customers (8K) show high churn risk.
- Only 15% of deliveries are on-time (avg. lead time: 31.92 days).

**Recommendations:**

- Target Unknown and Female demographics with marketing.
- Improve delivery performance to boost satisfaction and retention.

### Production Analysis

**Insights:**

- Skincare has high manufacturing costs ($1.5K) vs. low prices ($0.5K); Haircare is cost-efficient ($0.5K cost, $1.5K price).
- Many SKUs are pending inspection.

**Recommendations:**

- Adjust skincare pricing or cut costs.
- Scale haircare production for demand.
- Speed up inspections to clear backlogs.

### Shipping Analysis

**Insights:**

- Carrier A excels in revenue (67K) and availability, while Carrier C struggles with long lead times (228 days for skincare).
- Losses total 87.85K.

**Recommendations:**

- Optimize Carrier C’s operations.
- Increase stock with Carrier A.
- Investigate and mitigate financial losses.

### Supplier Analysis

**Insights:**

- Supplier 1 offers high stock (1233) and short lead times (14.8 days); Supplier 3 underperforms (674 stock, 20.1 days).
- Losses of 87.85K noted.

**Recommendations:**

- Leverage Supplier 1’s strengths.
- Improve Supplier 3’s stock and lead times.
- Address loss causes with cost-saving measures.

### Transportation Analysis

**Insights:**

- Rail leads revenue (97.58K) but has high costs and long lead times (56.57 days).
- Sea is cost-effective with shorter lead times (47.53 days).

**Recommendations:**

- Reduce rail costs and delays.
- Expand sea transport usage.
- Optimize high-cost routes (e.g., Route A).

---

For a deeper dive into the analysis and visualizations, check out the [project documentation](documentation.md).

This repository includes:

- [`dataset.csv`](dataset.csv): The supply chain dataset used in the analysis.
- [`documentation.md`](documentation.md): Detailed documentation of the analysis, including visualizations and findings.