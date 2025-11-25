# E-Commerce-Analysis
Analysis of E-Commerce Sales Dataset
In this Project, i analyzed an e-commerce sales dataset from a global software retailer that sells subscriptions and add-ons across analytics, design, collaboration, and AI. 

I leveraged my DAX skills to create measures and generate insightful visualizations. To finish off, I brought it all together in a sophisticated business dashboard to communicate insights to the Stakeholder.

**Project Steps**
1. Know the Objective
2. Understand the dataset
3. Data Cleaning
4. Data Modeling
5. Exploratory Data Analysis
6. Insight
7. Report Design

Lets dive in!

**Step 1: Know the Objective**

*Business Objective*:
The objective is to identify loyal customers (repeat buyers) and determine which channels and promotional campaigns drive their repeat purchases.

**Step 2: Understand the dataset**

The Dataset is a Global E-Commerce Transaction covering multiple products, plans, and customer segments. This Dataset was provided by Onyx Data.
The dataset has 3 Tables namely:-  Events, Products and Customers. Also the Data dictionary to the dataset was provided for easy understanding of the data.
After carefully going through the data, i loaded the data into the PowerBi desktop app for data cleaning.

**Step 3: Data Cleaning**

Data Cleaning is one of the most important process in data analysis. if you do not clean your data properly, your analysis wont be accurate and it will affect the insight you will generate.
i went through the ETL process which is, i extracted my data first then transform it before loading the data. The transformation of the data which also means cleaning of the data was done using power query.
The data is not that messy so i checked for the duplicate value, missing value and the data types of the column name to see if it really correspond with the column name.

**Step 4: Data Modelling**

The data model was done joined the Facts table  which is the (Events Table) to the Dimension Tables which are (Products and Customers Table) based on their relationship.
below is the data model of this project
![](https://github.com/phuad23/E-Commerce-Analysis/blob/main/model.PNG)

**Step 5: Exploratory Data Analysis**

After doing the data modeling, then i created some measures using DAX formular to answer some of the question asked.

1. 	How do total sales change by month?
   To answer this question, i created a line chart to visualize the month against the total revenue. By this, you can toggle among the month to see how sales changes on monthly basis.

2. 	Which channels bring in the most sales?
   To answer this question, i created a Clustered Bar chart to visualize the Total Revenue against the sales channel to see the channel that bring in more sales.

3. Which channels bring the most repeat (loyal) customers?
   To answer this question, i created a Stacked Bar chart to visualize the Sales Channel against the Loyal (repeat) Customers. mind you, i already use DAX formula to calculate the loyal customer. i based my loyal customers on customer who has patronized more than once.

4. What percent of monthly sales comes from loyal customers?
   To answer this question, i created a line chart to visualize Month against the Loyal Revenue in percentage. i used DAX formula to calcuate the Loyal Revenue %, to get this i Divided my Loyal Revenue by Total      Revenue to get the loyal revenue %.

5. Which products or plans sell the most?
   To answer this question, i created a Stacked Bar chart to visualize Total Revenue against the Product name to see the product that generated the highest revenue.

6. Which products are most popular with loyal customers?
   To answer this question, i created a Clustered Bar chart to visualize Product name against the Loyal Customers to see which product is more common or popular among the loyal (repeat) customers.

7. How long do customers wait before their second purchase?
   To answer this question, i created a Stacked Bar chart to visualize the Segment against Average Days to Second Purchase. This Avergae Days to Second Purcahse was calcluated using DAX formular, i first calcukated the first purchase and second purchase date, after which their difference is the days to second purchase, then i used AverageX function to calcuate the Average Days to Second Purchase and Values of the Events(customer_id).

All the question was answered and visualized with the necessary charts.

**Step 6: Insights**
1. in 2024, the total revenue generated was $14.57 million, while the total unit sold was 135,000 and the average selling price for 2024 was $108.1
2. From the Line Chart of the Revenue Trends, The month with the highest revenue is july which generated $3,685,397.24.
Also it was discovered that in the year 2024  the sales started from April, November is the month that generated the highest revenue of $1,794,931 while April generated the least revenue of $500,500.9 while in 2025 July is the month that generated the highest revenue of $1,930,917.34 and October generated the least revenue of $1,229,646.09.
4. Website is the channel that generated the highest revenue of about $14.4million  and also brought the highest loyal customer of 3851 while Partner generated the least reevenue of about $3.3million and also brought the least loyal customer of 1360.
5. The product with the highest revenue is Microsoft 365 Business Standard Annual which generate about $1,630,479.22 while AI Assistant Add-on monthly generated the lowest revenue of $27,306.57.
6. The top product that generated the highest revenue among loyal customers is Datadog Pro Annual which generated about $59,594.58 while FreshDeck Growth Monthly generated the least revenue of $64.48.
7. The Average days to second purchase of customer was categorized by Customer Segment. so, the average days to second purcahse of Consumer is 255 days, the average days to second purcahse of SOHO is 254 days, the average days to second purcahse of SMB is 251 days and the average days to second purcahse of Enterprise is 250 days.
8. Germany is the country with the highest average selling price of $125 while Australia is the country with the lowest average selling price of $107.
9. The billing cycle that generated the highest revenue per customer is Annual Subscription with revenue of $7,041.69 while Monthly Subscription generated the least revenue per customer of $698.86.
10. The Region that generated the highest revenue per customer is LATAM (Latin America) of about $8,679.12 while North America generated the least revenue per customer of $7,230.37.

**Step 7: Report Design**

I created some KPI's which are Card visuals, the following KPI's are created: Total Revenue, Loyal Customers, Unit Sold and Average Selling Price. 
A line chart of Revenue Trend was created, i added a parameter named KPI into the line chart so as to toggle between the following KPI, Total Revenue, Unit Sold and Total Order against the month column.

Conclusively, I put all the visuals of the question asked into a report template. The Report has 3 Pages, i created a “Overview” page which is the Home Page and provided users with quick access to navigate between pages in the report. The other 2 pages are Customer Page and Product & Channel Page.

Below are the images of the 3 Page Reports.
![](https://github.com/phuad23/E-Commerce-Analysis/blob/main/image.PNG)
![](https://github.com/phuad23/E-Commerce-Analysis/blob/main/Customer%20Analysis.PNG)
![](https://github.com/phuad23/E-Commerce-Analysis/blob/main/Product%20%26%20Channel%20Analysis.PNG)

Click [Here](https://app.powerbi.com/links/S-mZN2FIYa?ctid=d5bc17d2-4910-4403-86b9-672f3274f2f9&pbi_source=linkShare) to interact with the dashboard. You can also view the pdf of the final report [Here](https://github.com/phuad23/E-Commerce-Analysis/blob/main/E%20commerce%20Dashboard.pdf) 
