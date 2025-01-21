**Project Report: Financial Analysis of Top 2000 Global Companies in 2024**

---

### Executive Summary

This project focuses on analyzing financial data for the top 2000 global companies in 2024. The dataset includes key financial metrics, offering insights into company performance and market presence across various industries. The objective is to clean, preprocess, and derive valuable information, paving the way for in-depth analysis and visualization.

### Objectives

1. Understand the dataset structure and identify key attributes for analysis.
2. Clean and transform data to ensure consistency and accuracy.
3. Create derived features to enhance analysis.
4. Explore the data to uncover trends, relationships, and anomalies.

### Methodology

#### **Data Loading and Initial Exploration**
- Imported the dataset using `pandas` and inspected it using `.head()`, `.tail()`, `.info()`, and `.describe()`.
- Identified relevant columns such as `Country`, `Sales`, `Profit`, `Assets`, and `Market Value`.
- Reviewed the distribution of companies across countries.

#### **Data Cleaning and Preprocessing**
- Addressed inconsistencies in financial data representation:
  - Converted values such as "B" (billion) and "M" (million) into numeric format using a custom cleaning function.
  - Removed unnecessary columns like `Unnamed: 0` for a cleaner dataset.
  - Converted `Country` to a categorical data type for improved performance.

#### **Feature Engineering**
Developed new features to facilitate better analysis:
- **Profit Margin (%):** Indicates profitability relative to sales.
- **Asset Turnover Ratio:** Highlights efficiency in utilizing assets.
- **Return on Assets (ROA) (%):** Measures profitability relative to assets.
- **Company Size:** Categorized companies based on `Assets` as Small, Medium, or Large.
- **Costs:** Derived as `Sales - Profit`.

#### **Outlier Detection and Handling**
- Identified anomalies where `Costs` were zero or negative, suggesting data inconsistencies.
- Removed such records to enhance the reliability of the dataset.

#### **Exploratory Data Analysis (EDA)**
- Conducted visualizations using `matplotlib` and `seaborn` to understand:
  - Distributions of key metrics such as `Sales` and `Profit`.
  - Relationships between profitability indicators like `ROA` and `Profit Margin`.
  - Differences in performance across company sizes and geographic locations.

### Findings

1. The dataset required significant preprocessing to handle inconsistencies in financial data representation.
2. Feature engineering added valuable metrics such as profitability ratios and company size categorizations.
3. EDA revealed clear patterns and relationships, such as higher asset efficiency in smaller companies and geographic trends in profitability.

### Conclusion and Next Steps

This project successfully prepared a robust, clean, and enriched dataset ready for further financial analysis and advanced modeling. Future steps could involve:

1. Building predictive models to forecast key metrics like `Profit` and `Market Value`.
2. Conducting sector-specific analyses to uncover industry trends.
3. Integrating external data sources for a broader context, such as economic indicators or stock performance.

---

This report highlights the methods, findings, and impact of this project, demonstrating significant progress toward uncovering insights from the financial dataset.


