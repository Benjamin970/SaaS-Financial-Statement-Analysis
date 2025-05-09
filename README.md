# SaaS-Financial-Statement-Analysis

## Project Overview
This project focuses on the financial analysis of a Software as a Service (SaaS) company by comparing actual versus budgeted performance across key financial metrics. Using Excel for data cleaning and preprocessing, and Power BI for data modeling, DAX calculations, and interactive dashboard creation, the analysis delivers a comprehensive view of the company’s revenue trends, expense management, and profitability. The project highlights variances in operating expenses, gross profit, net profit, and total revenue, enabling deeper insight into financial performance. Visual storytelling through dashboards provides stakeholders with clear, actionable insights to support strategic planning and decision-making.

## Report Preview
![Screenshot 2025-05-05 233741](https://github.com/user-attachments/assets/81127638-d8bf-4059-b45d-505e628b53b1)
![Screenshot 2025-05-05 233956](https://github.com/user-attachments/assets/22610c41-2d81-4a8c-b118-922bbd085474)
![Screenshot 2025-05-05 234143](https://github.com/user-attachments/assets/2b4563a7-8a36-4613-9b80-60e25cde853f)

## Data Sources
The dataset used in this project consists of structured financial records from a simulated SaaS company. The data includes:
- ACCOUNTS Table – Chart of bank accounts detailing revenue and expense categories.
- TRANSACTIONS Table – Actual financial transactions recorded over a multi-year period.
- BUDGETS Table – Budgeted forecasts for income and expenditure across the same period.

These datasets were synthesized for analytical purposes and imported into Power BI after initial exploration and cleaning in Excel. The data reflects realistic financial structures and performance scenarios typical of SaaS businesses, including recurring subscription revenue, enterprise licensing, and vendor-based expenditures.

## Data Cleaning and Preparation
The raw financial datasets were first processed in Excel and Power Query to ensure accuracy, consistency, and readiness for analysis in Power BI. Key cleaning and preparation steps included:

1. Handling Missing Values: Reviewed and addressed missing or null entries in transaction and budget records to prevent analytical errors.
2. Data Type Correction: Ensured consistency in formats, especially for dates, monetary values, and categorical fields (e.g., account codes, departments).
3. Standardization: Harmonized account names, descriptions, and formats across the ACCOUNTS, TRANSACTIONS, and BUDGETS tables to support proper relational modeling.
4. Data Normalization: Used Power Query to restructure the data into a clean star schema format suitable for Power BI modeling.
5. Date Table Generation: Created a dynamic Date Table using DAX to enable time-based calculations like YTD, MTD, and QoQ.
6. Model Relationships: Established one-to-many relationships between fact (TRANSACTIONS) and dimension (ACCOUNTS, BUDGETS, DATE) tables to ensure analytical integrity.

These steps laid the groundwork for building a reliable, scalable Power BI data model and producing accurate, actionable insights.

## Data Analysis
The data analysis focused on evaluating financial performance by comparing actual results with budgeted expectations across multiple dimensions. Key areas of analysis included:

- Revenue Analysis: Tracked trends and variances in revenue over time, identifying strong performance in recurring SaaS subscriptions (68% of total revenue) and seasonal spikes, particularly in Q4.
- Expense Analysis: Assessed overall expenditure patterns, revealing significant increases in 2024 and volatility in Q3–Q4 across years. Identified major cost centers such as payroll (ADP) and infrastructure (AWS).
- Variance Analysis: Quantified over- and under-performance in both revenue and expenses using DAX measures, enabling precise detection of strategic misalignments.
- Profitability Trends: Monitored monthly profit margins, highlighting June as the only month with positive actual profit, and Q3 as the weakest quarter due to cost overruns.
- Client and Account Contribution: Ranked clients and revenue sources to assess concentration risk. The top two clients contributed over $8.3M, indicating reliance on a small number of major accounts.
- Visualization: Created interactive dashboards in Power BI with drill-down capabilities, KPI cards, and dynamic visuals to allow stakeholders to explore trends and insights across time and accounts.

This analytical approach provided a clear financial narrative and helped surface actionable opportunities to optimize budgeting, cost control, and revenue strategies.

## Results and Findings
The analysis uncovered several key insights into the SaaS company’s financial health and operational performance:

- Revenue Growth: Strong and accelerating revenue growth from 2022 to 2024, with actual revenue surpassing budget targets in 2024. October 2024 marked the highest revenue point in company history.
- Recurring Revenue Dominance: SaaS subscriptions accounted for approximately 68% of total revenue, confirming the effectiveness of the company’s recurring revenue model.
- Profitability Volatility: Despite revenue growth, monthly profit margins were inconsistent. Only June showed a positive actual profit, while Q3 (July–September) consistently underperformed due to rising expenses.
- Expense Surge: Operational expenses increased by over 60% in 2024. Key vendors like ADP ($9.5M) and AWS ($1.3M) represented major spending categories.
- Budget Deviations: Actual spending frequently exceeded budgeted figures in Q3–Q4, reflecting poor cost forecasting and control, especially during peak periods.
- Client Concentration Risk: Revenue was concentrated among a few major clients, with the top two contributing over $8.3M, signaling a need for diversification.
- Vendor Optimization Opportunity: Some vendors (e.g., Web Domain & Hosting) came under budget, suggesting success in cost containment and opportunities for broader optimization.

These findings point to the need for stronger cost governance, more accurate forecasting, and targeted strategies to smoothen profit margins and reduce risk exposure while leveraging growth momentum.

## Recommendations
Based on the findings from the analysis, the following strategic recommendations are proposed to improve the company’s financial performance and operational resilience:

- Strengthen Q3 Operational Planning:
Address consistent underperformance in Q3 by investigating seasonal factors or operational inefficiencies. Introduce targeted campaigns or cost control measures during this critical period.

- Enhance Cost Forecasting and Controls:
Implement rolling forecasts and variance monitoring to anticipate budget deviations. Apply stricter approval workflows for high-cost categories and evaluate discretionary spending.

- Optimize Vendor Relationships:
Reassess contracts with top vendors like ADP and AWS. Negotiate better terms or explore alternative providers to reduce the financial concentration risk and improve cost-efficiency.

- Diversify Client Portfolio:
Reduce dependency on top clients by expanding outreach to mid-tier and small business clients. Develop risk mitigation plans in case of churn or revenue drops from key accounts.

- Focus on High-Performing Revenue Streams:
Double down on SaaS subscriptions, which have shown reliable growth and profitability. Reevaluate the strategy for underperforming segments like product licenses.

- Capitalize on Seasonal Revenue Peaks:
Leverage Q4 momentum—especially in October–December—by launching year-end promotions, renewals, and bundled offerings to maximize recurring revenue capture.

- Improve Budgeting Accuracy:
Use historical data and advanced forecasting tools (e.g., machine learning models) to create more realistic budgets that reflect cyclical patterns and operational volatility.


## Limitations

- Scope Exclusions: The analysis focuses strictly on internal financial data (revenue, expenses, budgets) and excludes non-financial metrics such as customer satisfaction, churn rate, market conditions, or operational KPIs, which are also critical for holistic performance evaluation.

- Static Reporting Period: The insights are drawn from a fixed historical reporting period. The findings may not fully account for recent changes in business strategy, product offerings, or economic conditions.

- No External Benchmarking: The financial performance is assessed in isolation, without comparing results to industry peers or market averages, which limits the ability to contextualize the company’s competitiveness.

- Assumption-Based Interpretations: Some insights, such as causes of revenue dips or cost spikes, are inferred based on patterns rather than verified business events. Actual causes may differ and require validation with qualitative or operational data.
