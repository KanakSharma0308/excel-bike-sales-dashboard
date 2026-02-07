# excel-bike-sales-dashboard
📌 Project Overview
This project provides a comprehensive analysis of customer demographics and purchasing behavior for a retail bike store. By processing over 1,000 records of raw data, the project identifies key drivers—such as income, age, and commute distance—that influence a customer's decision to purchase a bike.

The goal was to transform unstructured data into a dynamic, interactive dashboard to assist in data-driven marketing decisions.

🖼️ Dashboard Preview
https://github.com/KanakSharma0308/excel-bike-sales-dashboard/blob/main/dashboard.png

🖼️ Pivot Tables Review
https://github.com/KanakSharma0308/excel-bike-sales-dashboard/blob/main/pivot_table1.png
https://github.com/KanakSharma0308/excel-bike-sales-dashboard/blob/main/pivot_table2.png
https://github.com/KanakSharma0308/excel-bike-sales-dashboard/blob/main/pivot_table3.png

🚀 Key Objectives
Demographic Analysis: Identify which age brackets and genders are most likely to buy bikes.
Financial Correlation: Evaluate how average income affects purchasing power.
Logistics Tracking: Measure the impact of commute distance on customer conversion.
Market Segmentation: Enable stakeholders to filter data by region, education, and occupation.

🛠️ Technical Workflow
1. Data Cleaning (ETL Process)
Raw data often contains inconsistencies that can skew analysis. I performed the following cleaning steps:
Duplicate Removal: Cleaned the dataset to ensure 1,000 unique customer IDs.
Value Standardization: Used "Find and Replace" to transform shorthand codes into descriptive text:
M / S → Married / Single
F / M → Female / Male
Category Correction: Standardized "Commute Distance" values (e.g., "10+ Miles" to "More than 10 Miles") for logical sorting in visualizations.

2. Feature Engineering (Age Brackets)
To analyze purchasing patterns across life cycles, I used a nested IF statement to create an Age Range column:
Excel
=IF(L2>54, "Old", IF(L2>=31, "Middle Age", IF(L2<31, "Adolescent", "Invalid")))
Adolescent: Under 31
Middle-Age: 31–54
Old: 55 and above

3. Data Modeling & Pivot Tables
I utilized Pivot Tables to aggregate data into actionable insights:
Income Analysis: Buyers had an average income of $57,962, while non-buyers averaged $54,874.
Commute Analysis: Sales peak significantly for customers with a commute of 0–1 miles.
Trend Analysis: Identified the Middle-Age bracket as the highest-performing segment with 383 purchases.

💡 Business Insights Uncovered
The "Middle-Age" Opportunity: The 31–54 age group is the primary market, showing both the highest interest and financial capability.
The Distance Threshold: There is a clear inverse correlation between commute distance and bike purchases; conversion rates drop sharply after the 5-mile mark.
Income Influence: Higher-income males represent the demographic with the highest individual purchasing frequency.

📁 How to Use
Clone the repository or download the .xlsx file.
Open the file in Microsoft Excel.
Navigate to the "Bike Sale Dashboard" sheet.
Use the Slicers on the left to filter the data by Region, Education, or Occupation.

Tools: Microsoft Excel (Advanced Formulas, Pivot Tables, Slicers, Data Visualization)
Project Category: Retail / Sales Analytics

