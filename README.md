# Superstore Sales & Profit Analytics

<p align="center">
  <strong>Interactive Business Intelligence Dashboard using Power BI and R</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI"/>
  <img src="https://img.shields.io/badge/R-Programming-276DC3?style=for-the-badge&logo=r&logoColor=white" alt="R"/>
  <img src="https://img.shields.io/badge/Machine%20Learning-Random%20Forest-2E8B57?style=for-the-badge" alt="Machine Learning"/>
  <img src="https://img.shields.io/badge/Analytics-Sales%20%26%20Profit-6C63FF?style=for-the-badge" alt="Analytics"/>
</p>

## Overview

**Superstore Sales & Profit Analytics** is a business intelligence project developed using Microsoft Power BI and R. It explores sales performance, profitability, customer segments, product categories and regional trends through an interactive dashboard.

The project combines Power BI's visualization and reporting capabilities with R-based statistical graphics and a Random Forest regression model for profit prediction.

## Objectives

- Analyse overall sales and profitability.
- Compare sales performance across product categories and geographical regions.
- Examine the contribution of different customer segments.
- Visualize the relationship between sales and profit.
- Implement Random Forest regression to predict profit.
- Build an interactive dashboard with KPI cards, slicers, filters and drill-down functionality.
- Present business insights through clear and meaningful visualizations.

## Tech Stack

| Technology | Purpose |
|---|---|
| Microsoft Power BI Desktop | Dashboard development and interactive reporting |
| R | Statistical analysis and predictive modelling |
| DAX | KPI calculations and business metrics |
| ggplot2 | R-based visualizations |
| dplyr | Data manipulation and aggregation |
| randomForest | Random Forest regression |
| Sample Superstore | Transactional business dataset |

## Dataset

The project uses the **Sample Superstore** dataset, which contains transactional information about orders, customers, products, sales and profit.

Important fields include:

- `Order ID`
- `Order Date`
- `Region`
- `Category`
- `Sub-Category`
- `Segment`
- `Sales`
- `Profit`
- `Quantity`
- `Discount`

Dataset resources: [Tableau Sample Data](https://www.tableau.com/learn/sample-data)

## Dashboard Features

### 1. KPI Cards

The dashboard includes five key performance indicators:

- **Total Sales** — overall sales value.
- **Total Profit** — overall profit generated.
- **Total Orders** — distinct number of orders.
- **Average Order Value** — sales divided by distinct orders.
- **Profit Margin** — total profit as a proportion of total sales.

### 2. Power BI Visualizations

Four native Power BI charts provide complementary views of business performance:

| Visualization | Purpose |
|---|---|
| Sales by Region | Compare regional sales |
| Profit by Sub-Category | Examine product-level profitability |
| Sales by Customer Segment | Compare customer segment contributions |
| Sales Trend Over Time | Explore changes in sales across dates |

### 3. R Visualizations

Four R-based visualizations extend the dashboard's analytical capabilities:

| Visualization | Purpose |
|---|---|
| Total Sales by Category | Compare sales across product categories |
| Total Profit by Category | Compare category-level profitability |
| Sales vs. Profit | Explore the relationship between sales and profit |
| Actual vs. Predicted Profit | Visualize Random Forest predictions against actual values |

### 4. Interactive Dashboard

- Region, Category and Segment slicers.
- Interactive filtering of supported visuals.
- Date and product hierarchy drill-down where configured.
- Two dashboard pages separating business overview from advanced analytics.
- Synchronized slicers across pages where enabled.

## Random Forest Regression

Random Forest regression is used to predict profit based on selected business features.

The final simplified model uses:

- **Input features:** Sales and Category.
- **Target variable:** Profit.
- **Train-test split:** 80:20.
- **Number of trees:** 50.

The actual-versus-predicted scatter plot compares the model's predictions with observed profit values. Points closer to the diagonal reference line represent predictions closer to the actual values.

Model performance should be evaluated using quantitative metrics such as Root Mean Squared Error (RMSE) and \(R^2\). No numerical model-performance results are reported here because they have not yet been recorded.

## Key Findings

The current dashboard shows the following observations:

- Technology has the highest sales among the three product categories.
- Technology contributes the highest category-level profit in the displayed dashboard.
- The West region records the highest sales, followed by the East region.
- The Consumer segment contributes approximately 50.56% of total sales.
- Profitability varies across product sub-categories, with some categories showing losses.
- The sales-versus-profit scatter plot contains both high-value transactions and loss-making observations.

These observations are based on the current dashboard output and can be explored further using the interactive filters.


## Getting Started

### Prerequisites

- Microsoft Power BI Desktop.
- R for Windows.
- The `ggplot2`, `dplyr` and `randomForest` packages.

### Install R Packages

Run the following command in the R console:

```r
install.packages(c("ggplot2", "dplyr", "randomForest"))
```

### Configure Power BI

1. Install R and the required packages.
2. Open Power BI Desktop.
3. Navigate to **File → Options and settings → Options → R scripting**.
4. Verify that Power BI detects the R installation.
5. Import the Sample Superstore dataset.
6. Create the required KPI measures and visualizations.
7. Add R visuals and execute the corresponding scripts.
8. Configure slicers, filters and drill-down functionality.

## Business Applications

The dashboard can help business users:

- Identify leading product categories and regions.
- Compare revenue and profitability.
- Investigate loss-making sub-categories.
- Understand the sales contribution of different customer segments.
- Evaluate the potential usefulness of predictive profit modelling.

## Limitations

- The analysis is based on historical transactional data.
- The Random Forest model uses a limited set of input features.
- Model performance depends on the quality and representativeness of the data.
- Predictions should be evaluated quantitatively before being used to support business decisions.

## Future Enhancements

- Evaluate the model using RMSE, MAE and \(R^2\).
- Compare Random Forest with other regression techniques.
- Incorporate additional business features where available.
- Improve model validation and hyperparameter tuning.
- Add further time-based and regional analyses.

## Academic Context

This project was developed as part of **Data Visualization Lab — Practical No. 7**, Course Code **TE7663**, Academic Year **2026–2027**, Semester V.

## References

- [Tableau Sample Data](https://www.tableau.com/learn/sample-data)
- [R Project](https://www.r-project.org/)
- [Microsoft Power BI Documentation](https://learn.microsoft.com/en-us/power-bi/)
- [ggplot2 Documentation](https://ggplot2.tidyverse.org/)
- [dplyr Documentation](https://dplyr.tidyverse.org/)
- [randomForest Package Documentation](https://cran.r-project.org/package=randomForest)

---

<p align="center">
  <strong>Built with Power BI, R and Data Analytics</strong>
</p>
