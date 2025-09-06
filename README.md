Rossmann Retail Sales Analysis on Snowflake
This repository contains the end-to-end SQL-based data analysis of the Rossmann store sales dataset, performed entirely within the Snowflake cloud data platform. The primary goal of this project was to conduct data cleaning, feature engineering, and exploratory data analysis (EDA) to uncover insights that could inform a demand forecasting model.

Key Objectives
Data Processing at Scale: To manage and process a large dataset with over 1 million rows efficiently using Snowflake's cloud architecture.

Feature Engineering: To create new, meaningful features from existing data to improve the quality of the analysis.

Insight Discovery: To perform EDA to identify key drivers of sales and understand the impact of factors like promotions, holidays, and seasonality.

🛠️ Tech Stack
Cloud Data Platform: Snowflake

Language: SQL

Dataset: Rossmann Store Sales (Kaggle)

methodology
The entire project followed a structured analytical process within Snowflake:

1. Data Cleaning & Preparation
Loaded the train and store datasets into Snowflake tables from a stage.

Conducted a thorough analysis to identify and handle NULL values through logical imputation (e.g., filling missing CompetitionDistance with the median).

Normalized categorical columns, such as converting StateHoliday from 0 to 'None' for clarity.

2. Feature Engineering
Joined the train and store tables to create a comprehensive primary analysis table.

Engineered new time-based features by extracting the Year, Month, Week, and Day from the date column.

Created custom boolean flags like IsWeekend and PromoMonthFlag to better capture seasonal and promotional effects.

3. Exploratory Data Analysis (EDA)
Wrote a series of SQL queries to analyze the relationships between various features and sales.

Investigated the distribution of store types, assortment levels, and the impact of competitor proximity.

Analyzed the effect of promotions, holidays, and day-of-the-week on average sales.

📊 Key Insights
One of the most significant findings from the EDA was the quantifiable impact of promotions on sales:

The average daily sales for a store on a non-promotional day were €4,406.

During promotional periods, the average daily sales surged to €7,991.

This represents a quantifiable sales uplift of 81.5%, highlighting the critical success of the promotion strategy.

📈 Visualizations
Below are some screenshots of the key queries and the resulting analysis performed in Snowflake.
