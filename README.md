## FURNITURE SALES ANALYSIS IN THE US

![Furniture Sales Dashboard](https://drive.google.com/uc?export=view&id=1qkgcKvpn3i774gZntlSss3aa8cNSftnj)


This project is a Furniture Sales Performance Dashboard designed to provide a comprehensive overview of sales metrics, shipping behavior, and regional distribution insights. Built using Microsoft Excel, the dashboard empowers business stakeholders to make data-driven decisions by visualizing trends.

## Objective

**This project aimed to analyse trends across:**
- Time
- Shipping Distribution by State
- Shipping Durations
- Highest revenue products
- Top Selling Cities
- Shipping Mode

**The results of the analysis can enable stakeholders to gain insights into key factors that are boosting and limiting sales revenue. It will also indicate locations or regions that are high performers, providing a good opportunity for marketing campaigns and loyalty programs.**

## Key Features
- KPI cards for Sales revenue, Profit, Quantity, and Year on Year Metrics.
- Geographical distribution by state.
- Slicers to enable interactivity
- Pivot Table

## Excel formulas for interactivity

- Top Selling Cities : `="Top Selling City: " & INDEX(G18:G22,MATCH(MAX(H18:H22),H18:H22,0),1) & " (" &TEXT(MAX(H18:H22), "$#,##0") & ") "`
- Order by duration: `="Most orders (" & TEXT(MAX(H30:H37), "0%") & ") were delivered in " & INDEX(G30:G37, MATCH(MAX(H30:H37), H30:H37, 0)) & "."`
- Sales by category: `="Highest Sales from Category: "&INDEX(G53:G56,MATCH(MAX(H53:H56),H53:H56,0))&" ("&TEXT(MAX(H53:H56),"$#,##0")&")"`
- YOY metrics = `=IF(L5>0,"▲","▼")&TEXT(ABS(L5),"0%")&" YoY"`

## KEY INSIGHTS

- Sales volume and revenue are growing YoY, but profitability is declining, indicating margin pressure.
- The majority of customers prefer Standard Class shipping, with most deliveries arriving in 3–5 days.
- New York City and Chairs lead in revenue contribution.
- Peak sales occur in December, suggesting strong seasonal buying trends.

## Tools and Technologies used

- Power Query for Data Transformation and Cleaning
- Pivot Table for analysis and summarization
- Excel Formulas for dynamic interactivity 
