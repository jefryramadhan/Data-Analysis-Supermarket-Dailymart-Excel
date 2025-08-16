# Data-Analysis-Supermarket-Dailymart (Interactive Dashboard creation using MS Excel-SQL-Tableu)

## Project Objective
This Project providing in depth analysis sales data from January - April 2025 for "Supermarket Dailymart". Main objective is to creating important insights related performance product, sales trends, customers behavior to informs strategic business decision.

## Data Used
- <a href=https://github.com/jefryramadhan/Data-Analysis-Supermarket-Dailymart/blob/main/Supermarket%20Data%20Analysist.xlsx>Supermarket Dailymart Data</a>

## Questions (KPIs)
- What is the total number of sales transactions in Jan - April 2025?
- How many unique customers came in January - April 2025?
- How many total products sold in January - April 2025?
- How many average item/product purchased by customers?
- How many verage weekly product sales?
- Which month did the biggest sales occur?
- What is the most sold product?

## Process
preliminary analysis with Excel:
1. Tidy up the data using power Query for transformation, and cleaning data.
2. made sure data is consistent and clean with respect to data type,data format and value used.
3. creating pivot table according to the questions asked (KPIs).
4. merge all pivot table into one dashboard and aplly slicer to make dynamic.
5. <a href="https://github.com/jefryramadhan/Data-Analysis-Supermarket-Dailymart-Excel-SQL-Tableu/blob/main/Dashboard%20Dailymart%20excel%20version.png">View Dashboard Excel version</a>

<img width="1830" height="1062" alt="Dashboard Dailymart" src="https://github.com/user-attachments/assets/7c8769fd-ecb8-483c-8058-1630629a968e" />


SQL:
1. **Data Preparation:** Imported Dataset CSV with -200.000 rows into MySQL Database use command `LOAD DATA LOCAL INFILE` to handling data raw.
2. **Data Transforming:** Function `STR_TO_DATE()` used in process import to ensuring format date its right and already to analyzed.
3. **Query & Analysis:** Each business questions(KPIs) answered with write the Query SQL Specifically use Clause `WHERE` to filtering, `GROUP BY` to Aggregation and functions like `COUNT(DISTINCT ...)`, `AVG()`, and `MONTHNAME()`.
4. <a href="https://github.com/jefryramadhan/Data-Analysis-Supermarket-Dailymart-Excel-SQL-Tableu/blob/main/supermarket_analysis_query.sql">View Query SQL</a>

Tableu:
1. The cleaned data was then connected to Tableu to build comprehensive interactive dashboard. This dasboard designed for visualize key KPIs, monthly and weekly salews trends, and the performance best selling product.
2. <a href="https://public.tableau.com/app/profile/rahmad.jefry.r/viz/SupermarketDailymartDashboard/Dashboard1?publish=yes">Link Dashboard</a>

## Dashboard 
<img width="969" height="697" alt="Supermarket Dailymart Dashboard Tableu" src="https://github.com/user-attachments/assets/9406f32a-bcda-404b-b5e2-390c43826e2b" />

## Project Insight
- weekly sales norms between 11.500 transactions indicating market stability.
- The highest monthly sales performance was in March which was close to 51000 transactions and the lowest was in February at 46000 transactions.
- The highest sales driving product is Cereal and the second is Ice Cream.

## Final Conclusion
To improve the sales of Supermarket Dailymart, from the basket market analysis, the markting strategic plan focuses on the most sold products. Make a bundling promo of Cereal and Ice cream prodcut or make another bundling of top 10 product sold, do a sales strategy to put products that sell less side by side with the most sold so that buyers are interested in buying them. This demographic represents stable weekly sales performance and less stable monthly performance. conducting a special campaign in feb to counteract the seasonal downward trend will stabilize monthly sales.
