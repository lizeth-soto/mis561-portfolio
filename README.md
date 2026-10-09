# mis561-portfolio
Data Visualization Course Portfolio.
This will include all completed assignments in Excel, Tableau, PowerBI through DataCamp, Adobe Express, and various AI tools.

Initial E-Commerce Profitability Analysis: Develop a basic profitability set of dashboards and explain your design. Link to published Tableau workbook:
https://public.tableau.com/views/FlexAssignment3_lizethsoto/ExplanatoryDashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
This assignment was challenging as the analysis required to consider several factors affecting the profitability of the selected product subcategory.

Account Profitability and Service Tiers Analysis: Develop a chart to visualize effect of discount over gross margin, per account tier, in order to make decisions on account policies. Link to published Tableau workbook:
https://public.tableau.com/views/AccountAnalysis_Soto_Lizeth/AppliedChart?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
If I did this assignment again, I would define the data elements with a quantifiable effect on the account policies from the start (discount over gross margin): I lost time trying to find out if cost to serve had correlation with gross margin.

PowerBI - DataCamp Training Certificate | Introduction to Power BI | Completed on September 27, 2026:
https://public.tableau.com/views/PowerBITrainingCertifications_17905753997990/PowerBI-DataCampTrainingCertificate?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
Before loading the order data into Tableau in Flex Assignments 3 and 4, I cleaned it by hand in Excel: I used Text to Columns to split a field that held two values in the same cell, filled the blank cells in the Product field with "Unknown," and deleted the rows missing a matching Order ID so they would not distort the totals. Power BI's Power Query editor handles the same cleanup (Split Column, Replace Values, Filter Rows), but it automatically records each action as an "Applied Step" that I can review, reorder, or undo at any point. In Excel, those edits overwrote the original data, so if I made a mistake, I had to start over and repeat every step from memory. Next time, I would choose Power Query for this task because the cleaning becomes a documented, repeatable process that can be reapplied on new data with a single refresh, and anyone reviewing my work can see exactly what I changed.

Introduction to DAX in Power BI Certificate | Completed on October 4th, 2026:
https://public.tableau.com/views/PowerBITrainingCertifications_17905753997990/PowerBI-DataCampTrainingCertificates?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
To find gross margin for each account, I summarized Revenue and Profit by Customer ID in a pivot table, then divided each account's total profit by its total revenue on the Account Summary sheet and compared the result to the 15% accounting target. In Power BI, I would build gross margin as a measure, not a calculated column. A calculated column is computed and stored once per order line, so it can only produce order-level margins, and adding or averaging those doesn't give an account's true margin. A measure is calculated when it's displayed, summing profit and revenue for whatever is selected (one account, one year, or the full 2022–2025 period) and then dividing, so the margin is correct at any level and stores nothing extra in the model. For Marcus, this means he can select any account and any year during a meeting and see right away whether it meets the 15% target.

REDO: Account Profitability and Service Tiers Analysis: Develop a chart to visualize effect of discount over gross margin, per account tier, in order to make decisions on account policies. Link to published Tableau workbook:
https://public.tableau.com/views/FlexAssignment4_1AccountProfitabilityandServiceTiers/AppliedChart?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
I did this assignment again to make chart more legible and rewrite its justification.

