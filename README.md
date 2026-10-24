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

Advancing in Power BI for Data Visualization: Build a written case for a hiring manager from evidence in your own work, including which tool fits which 
job and where your skills still have gaps. 
https://public.tableau.com/views/PowerBITrainingCertifications_17905753997990/PowerBI-DataCampTrainingCertificates?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
Sarah,
After completing the Power BI courses, I am ready to join Southwest’s business intelligence team and use Power BI to make both of my analyses self-serve.
In Flex 3, I showed Anita where Tables’ discounts turn unprofitable with a 48-cell bubble grid (Segment × Region × Ship Mode). In Power BI, I would rebuild it as one scatter chart of discount against average profit per order, with conditional formatting coloring losses red and profits navy, a constant line labeled “20% cap,” and Segment and Region as slicers. Anita would read one panel instead of 48 cells, and each data refresh would automatically recolor any point that turns negative.
In Flex 4, I estimated net contribution for one fixed set of caps. In Power BI, the cap would be a what-if parameter and net contribution a measure so that Marcus could test other caps himself in the meeting.
I would divide the tools this way: Excel for quick, one-time exploration; Tableau for one-off explanatory charts needing custom design or public sharing; Power BI for scheduled-refresh reports that managers filter themselves.
My gap is experience with live company data, since my Flex projects used static exports and I have never managed scheduled refreshes or data that changes after publishing. To close it, I would first learn the team’s source systems and data dictionary, then shadow a teammate through a scheduled refresh, and rebuild one existing team report in a test workspace before sharing anything with managers.
I would welcome the chance to walk you through either rebuild.

Card Portfolio Review – Contactless Readiness | Which cards belong to the early replacement batch this quarter? (how many, what will it cost, evidence supporting the choice)
https://public.tableau.com/views/CardPortfolio/ExploratoryDash?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
If I were to redo this assignment, I would suggest alternatives according to budget ranges.

Card Growth Analysis – Wildcat Rewards Offer | Where/To whom should the first pilot go?
https://public.tableau.com/shared/83JKKRKG3?:display_count=n&:origin=viz_share_link
If I were to redo this assignment, I’d ask Compliance early whether a generation-based pilot is allowed. Millennials kept the largest eligible pool at higher cutoffs (80 at 700, 49 at 720), but I ruled them out over fair-lending concerns about targeting by age.
