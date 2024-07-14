# Market-Research-Analysis

Report Link : https://app.powerbi.com/groups/me/reports/612cd342-b7a4-4fea-bae9-e6cf4cf883b1?ctid=edc5c3bf-4ab5-4697-84fa-41b44eb08b5e&pbi_source=linkShare

Problem Statement
This report-cum-dashboard helps the company understand their customers better. It helps MarketMindz know if their customers are satisfied with their services. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area. It lets them know about their different campaigns' performances, buyer composition (who their customers are and what are their spending habits) and the different purchase drivers associated with what enhances or brings down performance in a particular campaign.

Thus arises the need to answer the following key questions for our analysis:

How are our 6 recent marketing campaigns performing?
How are our products performing?
Who are our customers?
What is driving campaign performance and buyer-decision making?


Steps followed

#Reviewing our Data

Step 1 : Load data into Power BI Desktop, dataset is a csv file.
Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
#Transforming our Data

Step 1 : Understand column names and meanings, using the marketing data dictionary for reference.
Step 2 : Identified and clarified unclear column names such as 'accepted CMP', 'num catalog purchases', and 'nt wines
Step 3 : Converted 'year birth' to 'age' using date transformations and age calculations, ensuring accurate age representation.
Step 4 : Corrected typos and standardized entries in 'education' and 'marital status' columns, merging infrequent values into an 'other' category.
Step 5 : Renamed columns for clarity, e.g., changing 'nt wines' to 'amount wine products', ensuring intuitive names for easier data understanding.
Step 6 : Set 'income' as a fixed decimal number for currency representation, ensuring correct data type handling in Power BI.
Step 7: Completed initial data transformations, ensuring cleaned and accurate data for effective data visualization and reporting.

#Evaluating Campaign Performance

Step 1 : Rename and reference the marketing dataset to isolate campaign-related columns. Unpivot campaign acceptance indicators into a single column for clarity.
Step 2 : Generate a bar chart displaying campaign acceptance rates. Ensure each campaign is clearly labeled on the X-axis with corresponding acceptance totals on the Y-axis.
Step 3 : Reference and consolidate product-related data from the marketing dataset. Unpivot product sales data to aggregate total sales in a single column.
Step 4 : Develop a bar chart illustrating sales figures across different product categories. Format total sales data as currency for improved readability and understanding.
Step 5 : Verify the accuracy of campaign and product performance charts. Save finalized visuals to ensure they accurately represent the dataset.
Step 6 : After pivoting product and campaign information into separate tables, we can now visualize total sales by product and campaign acceptance in a single chart.
Step 7 : Adjusted cross-filter direction between campaign and marketing data tables to accurately reflect total sales data by accepted campaigns.
Step 8 : Created a stacked 100% bar chart to analyze the sales composition of each campaign, highlighting product preferences among customers who accepted campaigns.
Step 9 : Utilized Power Query to pivot columns and create a platform table, showcasing purchase distribution across campaigns through catalogs, web, and in-store.
Step 10 : Developed another visual to display total purchases across different platforms, providing insights into customer preferences and purchase behaviors influenced by campaign efforts.

#Evaluating Buyer Composition

Step 1 : Understand customer demographics deeply relevant to campaign and product performance.
Step 2 : Avoid superficial demographics like average age or gender breakdowns; focus on how demographic attributes influence purchasing behaviors.
Step 3 : Divide page into halves - one for basic demographic insights (education, marital status, children at home) and the other for linking these demographics to campaign effectiveness.
Step 4 : Use bar charts for education levels, marital status, and donut charts for presence of kids and teens at home. Ensure clarity by renaming labels like "Kids at Home" and "Teens at Home" for better readability.
Step 5 : Employ bar charts to visualize campaign acceptance filtered by demographic attributes.Example: Use average income to show income variation across campaigns, enhancing with error bars for income range insights.
Step 6 : Utilize a stacked 100% bar chart to analyze purchasing habits by age groups. Enhance readability by grouping ages into bins (e.g., 5-year intervals) directly within the visual settings.
Step 7 : Avoid cluttering with excessive visuals; prioritize aesthetics and user comprehension. Utilize card visuals to succinctly display key metrics like user count, average income, average age, and platform preferences (e.g., deals, store, catalog, website visits).

#Uncovering Purchase drivers

Step 1 : The Key Influencers Visual was selected for its ability to identify and interpret influential factors within customer data.

Step 2 : Key variables were defined for analysis, including demographic attributes such as age, income, marital status, and behavioral metrics like website visits and campaign acceptance data.

Step 3 : The focus was on understanding the factors influencing customers to accept specific marketing campaigns. Variables like age, income levels, and household composition were analyzed to pinpoint significant influences on campaign success.

Step 4 : The scope expanded to analyze factors influencing total sales. This involved examining variables such as income levels, family demographics, and educational backgrounds to uncover trends driving overall sales figures.

Step 5 : A product slicer was introduced to enhance user interaction and deepen analysis. This feature allowed exploration of how different product categories—like wine or meat—were influenced by customer attributes, providing nuanced insights into purchasing behaviors.

Step 6 : The visual layout was refined to ensure clarity and usability. Side-by-side Key Influencers Visuals alongside the product slicer were presented to make complex data more accessible. Additionally, data storytelling techniques were incorporated to highlight key findings and actionable insights.

