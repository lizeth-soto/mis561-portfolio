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

Introduction to DAX in Power BI Certificate | Completed on October 3rd, 2026:
https://public.tableau.com/views/PowerBITrainingCertifications_17905753997990/PowerBI-DataCampTrainingCertificates?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
To find gross margin for each account, I summarized Revenue and Profit by Customer ID from the order-level data in a pivot table, then copied the distinct account list to the sheet "Account Summary" and divided each account's total profit by its total revenue and compared the result to the 15% accounting target. For example, Alex Avila's margin for the complete data period is −6.52% (−$362.87 ÷ $5,563.56), well below the target.
In Power BI, I would build gross margin as a measure, not a calculated column. An account's margin isn't stored on any single order line. It comes from the account's total profit and total revenue, and those totals change with whatever date range is selected. A measure shows the full 2022–2025 margin by default and recalculates when the view is narrowed to a single year. A static Excel summary can't do that without rebuilding the pivot by hand. For Marcus, this means he can select any account and any year during a meeting and see right away whether it meets the 15% target, without waiting for a rebuilt spreadsheet.
