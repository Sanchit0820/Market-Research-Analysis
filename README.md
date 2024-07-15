# Market-Research-Analysis

Report Link : https://app.powerbi.com/groups/me/reports/612cd342-b7a4-4fea-bae9-e6cf4cf883b1?ctid=edc5c3bf-4ab5-4697-84fa-41b44eb08b5e&pbi_source=linkShare

# Problem Statement

This report-cum-dashboard helps the company understand their customers better. It helps MarketMindz know if their customers are satisfied with their services. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area. It lets them know about their different campaigns' performances, buyer composition (who their customers are and what are their spending habits) and the different purchase drivers associated with what enhances or brings down performance in a particular campaign.

Thus arises the need to answer the following key questions for our analysis:

* How are our 6 recent marketing campaigns performing?
* How are our products performing?
* Who are our customers?
* What is driving campaign performance and buyer-decision making?


# Steps followed

### #Reviewing our Data

Step 1 : Load data into Power BI Desktop, dataset is a csv file.

Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.

Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".

### #Transforming our Data

Step 1 : Understand column names and meanings, using the marketing data dictionary for reference.

Step 2 : Identified and clarified unclear column names such as 'accepted CMP', 'num catalog purchases', and 'nt wines.

Step 3 : Converted 'year birth' to 'age' using date transformations and age calculations, ensuring accurate age representation.

Step 4 : Corrected typos and standardized entries in 'education' and 'marital status' columns, merging infrequent values into an 'other' category.

Step 5 : Renamed columns for clarity, e.g., changing 'nt wines' to 'amount wine products', ensuring intuitive names for easier data understanding.

Step 6 : Set 'income' as a fixed decimal number for currency representation, ensuring correct data type handling in Power BI.

Step 7: Completed initial data transformations, ensuring cleaned and accurate data for effective data visualization and reporting.

### #Evaluating Campaign Performance

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

### #Evaluating Buyer Composition

Step 1 : Understand customer demographics deeply relevant to campaign and product performance.

Step 2 : Avoid superficial demographics like average age or gender breakdowns; focus on how demographic attributes influence purchasing behaviors.

Step 3 : Divide page into halves - one for basic demographic insights (education, marital status, children at home) and the other for linking these demographics to campaign effectiveness.

Step 4 : Use bar charts for education levels, marital status, and donut charts for presence of kids and teens at home. Ensure clarity by renaming labels like "Kids at Home" and "Teens at Home" for better readability.

Step 5 : Employ bar charts to visualize campaign acceptance filtered by demographic attributes.Example: Use average income to show income variation across campaigns, enhancing with error bars for income range insights.

Step 6 : Utilize a stacked 100% bar chart to analyze purchasing habits by age groups. Enhance readability by grouping ages into bins (e.g., 5-year intervals) directly within the visual settings.

Step 7 : Avoid cluttering with excessive visuals; prioritize aesthetics and user comprehension. Utilize card visuals to succinctly display key metrics like user count, average income, average age, and platform preferences (e.g., deals, store, catalog, website visits).

### #Uncovering Purchase drivers

Step 1 : The Key Influencers Visual was selected for its ability to identify and interpret influential factors within customer data.

Step 2 : Key variables were defined for analysis, including demographic attributes such as age, income, marital status, and behavioral metrics like website visits and campaign acceptance data.

Step 3 : The focus was on understanding the factors influencing customers to accept specific marketing campaigns. Variables like age, income levels, and household composition were analyzed to pinpoint significant influences on campaign success.

Step 4 : The scope expanded to analyze factors influencing total sales. This involved examining variables such as income levels, family demographics, and educational backgrounds to uncover trends driving overall sales figures.

Step 5 : A product slicer was introduced to enhance user interaction and deepen analysis. This feature allowed exploration of how different product categories—like wine or meat—were influenced by customer attributes, providing nuanced insights into purchasing behaviors.

Step 6 : The visual layout was refined to ensure clarity and usability. Side-by-side Key Influencers Visuals alongside the product slicer were presented to make complex data more accessible. Additionally, data storytelling techniques were incorporated to highlight key findings and actionable insights.


# Findings

### Campaign Performance
![campaign performance](https://github.com/user-attachments/assets/cfa9e5b1-f48c-4c01-942b-883a3d2839b8)

1. Wine is the top-performing product in terms of both revenue ($681K) and number of purchases across all campaigns. Possible reasons for this could be high demand and popularity of wine as well as effective marketing strategies targeted towards wine. Also, wine generally has a higher price point compared to other categories, contributing to higher revenue.

2. Campaign 6 is the most successful in terms of both purchases (334) and revenue ($0.33M). This could be because Campaign 6 might have been launched during a peak buying period, such as holidays or special events. Another reason could be the introduction of attractive offers and discounts that resonated well with customers as well as effective targeting of the right audience segments.

3. In-store is the most preferred purchasing platform across all campaigns (13K). This could be primarily be due to customer experience where customers might prefer the tactile experience of shopping in-store. In-store purchases also allow customers to immediate gratification by providing their products on the spot. Some customers may also feel more secure purchasing in-store as compared to online.

4. Web (9.2K) and Catalog (6.0K) Purchases also contribute significantly. Web and catalog shopping offer convenience, especially for those who may not have easy access to physical stores. Wide reach can also be an example where online and catalog channels can reach a broader audience, including those in remote areas. Changes in shopping behaviour due to the pandemic may also have increased reliance on web and catalog shopping.

### Buyer Composition 
![buyer composition](https://github.com/user-attachments/assets/e6d5c29e-8825-4364-a50b-4b76b151cd0c)

1. The average age of our customers comes out to be approximately 55 years. This could be because the customer base might be skewed towards older adults due to product type or marketing strategies that appeal more to this demographic. Since wine was the highest selling product, it makes sense that middle aged people dabble more in wine as they grow older and their income rises.

2.  Education Level - The majority of customers have a college/university degree (Graduation: 1,127). One possible explanation could be because of higher education Levels, customers might be more informed and selective, preferring quality and value for money.

3. Marital Status - A larger chunk of our customers is married. This could be because marketing strategies or product offerings might appeal more to married individuals or families.

4. Household Composition - Kids at Home: 58% have no kids, 40% have 1 kid, 2% have 2 kids.

                           Teens at Home: 52% have no teens, 46% have 1 teen, 2% have 2 teens.

Possible Reasons:

Few Kids and Teens at Home: Indicates a trend towards smaller household sizes or older families with grown children.

### Purchase Drivers
![purchase drivers](https://github.com/user-attachments/assets/2825cd77-965d-40e0-83ed-f8082407cb4e)

1. This is a Key Insights dashboard that helps to find a determinant for success of each campaign or what factors influence income or total web visits, for example, to increase. It also helps in forecasting the same based on the present available data to understand what will work best in the future to further optimize our understanding of our market.

2. For example, in the measure set above, we can see when Campaign 6 is selected or the likelihood of accepted campaign being campaign 6 increases when income is $44,051 or less (1.93x), number of Kids at home is 1, web visits is more than 6 and marital status is single.


### Recommendations 

1. Targeted Marketing Campaigns:
   
* Demographic Focus: Given that the average customer age is 55.2 and many customers are married, create marketing campaigns that appeal to older adults and families. Highlight products that cater to their needs and preferences, such as health-focused items, convenience products, and family-sized packages.
  
* Income-Specific Offers: Tailor offers and promotions based on the income levels identified in the reports. For lower-income segments, emphasize affordability and value. For higher-income segments, focus on premium products and exclusive deals.
  
2. Enhanced Online Engagement:
   
* Web Activity Utilization: Leverage the insight that higher web activity correlates with campaign acceptance. Enhance the online shopping experience by improving website usability, offering personalized recommendations, and using targeted online ads and email campaigns to drive engagement and conversions.
  
* Frequent Web Visitor Retention: Implement strategies to retain and engage frequent web visitors. Consider loyalty programs, regular newsletters, and exclusive online offers to encourage repeat visits and larger purchases.
  
3. Product and Service Diversification:
   
* Age-Based Preferences: Recognize the distinct preferences of different age groups. For younger customers, promote meat and other fresh products. For older customers, emphasize wine and gourmet items. Tailor product recommendations and promotions to these preferences to boost sales.
  
* Household Composition Consideration: Offer products and promotions tailored to the household composition. For families with kids or teens, consider family-sized packages and child-friendly products. For single or child-free households, emphasize convenience and luxury items.
  
4. Channel-Specific Strategies:
   
* In-Store Dominance: Given the high number of in-store purchases, enhance the in-store shopping experience. Offer in-store exclusive promotions, loyalty programs, and personalized service to encourage repeat visits and higher spending.
  
* Multi-Channel Integration: Ensure a seamless omnichannel experience. Integrate online and offline channels to allow customers to easily switch between them. Use data from online interactions to inform in-store promotions and vice versa.
  
5. Campaign Design and Evaluation:
   
* Campaign-Specific Insights: Use the insights from successful campaigns (e.g., Campaign 6) to design future campaigns. Focus on the factors that increased acceptance, such as targeting lower-income segments, promoting through high web activity channels, and appealing to single customers.
  
* Continuous Improvement: Regularly evaluate the performance of each campaign. Use data analytics to understand what works and what doesn’t. Adjust future campaigns based on these insights to continuously improve effectiveness.
  
6. Personalized Customer Engagement:
    
* Personalization: Use customer data to offer personalized recommendations and promotions. Tailor marketing messages to individual preferences and purchasing behaviors to increase engagement and loyalty.
  
* Customer Feedback: Collect and analyze customer feedback to understand their needs and preferences better. Use this information to refine product offerings and marketing strategies.
  
7. Promotional and Discount Strategies:
   
* Discount Purchases: Given the significant number of discount purchases, strategically use discounts to attract price-sensitive customers without eroding overall profitability. Consider time-limited offers, bundle deals, and loyalty discounts.
  
* Seasonal and Event-Based Promotions: Plan promotions around key seasons and events that resonate with your target demographics. For example, offer special deals during holidays, family-focused events, and health awareness months to drive sales.

