# Financial Sales Performance Analysis and Presentation

## Project Overview

This project provides a comprehensive financial performance analysis focusing on sales and profitability for the fiscal year. The analysis culminates in a dynamic Tableau dashboard and a corresponding PowerPoint (PPTX) slide deck used to communicate key findings to business stakeholders.

### Deliverables

1.  **Tableau Dashboard (`Financial Sales Dashboard.twbx`):** Interactive visualization of key financial metrics.
2.  **Slide Deck (`Financial Sales Dashboard.pptx`):** A narrative-driven presentation of the key insights and recommended action items.

---

## 1. Summary of the Presentation (PPTX Narrative)

The final slide deck was generated using the analysis derived from the Tableau dashboard and focused on the following three key insights:

| Focus Area | Key Finding Communicated | Actionable Takeaway |
| :--- | :--- | :--- |
| **Overall Performance** | Achieved strong **Year-over-Year (YoY) Sales Growth** (e.g., ~25-30%), exceeding targets. | Continue investment in successful sales channels and markets. |
| **Product Profitability** | The **Paseo** product line was identified as a critical profit driver, despite representing a smaller volume of total units. | Strategically prioritize the marketing and sales of high-margin items like Paseo. |
| **Seasonal Trends** | The company realized its highest profit margin and total profit during **December**. | Analyze marketing spend and inventory management specific to the Q4 period to optimize future results. |

---

## 2. Tableau Dashboard Creation Steps

The dashboard was built in Tableau Desktop (saved as a `.twbx` file) following these primary steps:

### A. Data Source Preparation

1.  **Source File:** Connected to the primary data source (`Financial Sample.xlsx`, as referenced in the workbook).
2.  **Data Cleaning:** Ensured consistent formatting for Date, Currency, and Quantity fields.
3.  **Data Modeling:** Established necessary relationships between tables (if multiple sheets were used).

### B. Calculated Fields

Several custom calculated fields were created to enable deeper analysis:

* `Profit Margin`: `(Profit / Sales) * 100`
* `YoY Sales Growth`: `(ZN(SUM([Sales])) - LOOKUP(ZN(SUM([Sales])), -1)) / ABS(LOOKUP(ZN(SUM([Sales])), -1))`
* `Unit Selling Price`: `Sales / Units Sold`

### C. Core Visualizations

The following core charts were constructed and used as the basis for the final analysis:

* **KPI Cards:** Displaying total Sales, total Profit, and the overall YoY Growth percentage.
* **Monthly Trend Chart:** A dual-axis line chart tracking Sales and Profit over time to identify peak performance periods (e.g., December).
* **Product Performance Bar Chart:** A visualization showing Profit by Product to highlight key drivers like 'Paseo'.
* **Geographical Map:** A map view detailing performance across different Segments or Countries.

### D. Dashboard Assembly

1.  **Layout:** Arranged all core visualizations and KPI cards into a single, cohesive dashboard layout.
2.  **Interactivity:** Added **Filters** (e.g., by Year, Month, or Product) and **Actions** to allow users to drill down into specific data points.
3.  **Branding:** Applied a consistent color palette and clean fonts for professional presentation.
