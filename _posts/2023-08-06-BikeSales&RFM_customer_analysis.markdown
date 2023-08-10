---
layout: post
title: Bike Sales & RFM Customer Analysis
date: 2022-03-01
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: dashboard.png # Add image post (optional)
tags: [RFM_Scores,CustomerAnalysis,Excel,Tableau,KPMG,SalesData] # add tag
---
## Summary of Insights
For this project I analyzed 20,000 rows of transactional data in order to find top customers and the distribution of customers based on RFM (Recency Frequency Monetary) scores. I found that the top customers fell in the following groups: 40-49 years old, mass customers, female, from New South Whales, and from the "manufacturing" job industry. I also found that 40.14% customers fell into the 2nd and 3rd quartiles for recency. Such customers are a potential flight risk but haven't been lost yet. The recommendation is to look into why they these customers haven't bought in a while and likely target them with campaigns and incentives. 

- Used Excel to clean, mitigate, and prepare data for analysis
- Used Excel to calculate RFM scores and create pivot tables and charts 
- Used Tableau to create a dashboard displaying most important metrics
- [Here you can find the dashboard](https://public.tableau.com/app/profile/alice.giliarini/viz/KPMG_16465478819120/Dashboard1#1)

## Context
For this project KPMG provided three tables with data from a hypothetical company, Sprocket Central Pty Ltd:
- Transaction history: 20,000 rows of transactions
- Customer demographics: 4,001 customers
- Customer address: 4,000 customers
  
We were also given the following background information regarding the company:
> "Sprocket Central Pty Ltd is a long-standing KPMG client whom specializes in high-quality bikes and accessible cycling accessories to riders.” They have “given us a new list of 1000 potential customers with their demographics and attributes. However, these customers do not have prior transaction history with the organization."

> "Using the existing 3 datasets (Customer demographic, customer address and transactions) (…), please recommend which of these 1000 new customers should be targeted to drive the most value for the organization."

The project was broken down into three tasks:
1. Assess, clean, and mitigate the data. 
2. Explore the data and create a power point [presentation](https://github.com/agiliariniosm/Alice_Giliarini_Portfolio/blob/main/kpmg/KPMG%20virtual%20experience%20program.pdf) with your insights. 
3. Create a [dashboard](https://public.tableau.com/app/profile/alice.giliarini/viz/KPMG_16465478819120/Dashboard1#1) to present to the client. 

#### Data Assessment 
![data_assessment]({{site.baseurl}}/assets/img/KPMG/data_cleaning.png)

#### Data Exploration & Presentation

[Here you can find the presenatation](https://github.com/agiliariniosm/Alice_Giliarini_Portfolio/blob/main/kpmg/KPMG%20virtual%20experience%20program.pdf)
[![customertype]({{site.baseurl}}/assets/img/KPMG/customer_types.png)](https://github.com/agiliariniosm/Alice_Giliarini_Portfolio/blob/main/kpmg/KPMG%20virtual%20experience%20program.pdf)

#### Key Findings & Dashboard

[Here you can find the dashboard](https://public.tableau.com/app/profile/alice.giliarini/viz/KPMG_16465478819120/Dashboard1#1)
[![dashboard]({{site.baseurl}}/assets/img/KPMG/dashboard.png)](https://public.tableau.com/app/profile/alice.giliarini/viz/KPMG_16465478819120/Dashboard1#1)

I found the top customers to be:
- 40-49 years old
- Mass customers
- Female
- From New South Wales
- From the "manufacturing" job industry

Customers with these characteristics brought in the most profit. The recommendation is to look for these characteristics in the list of 1000 new customers when deciding who to target. Further more, I found that 40.14% of customers are in the "About to Dump You" segment and are at risk of leaving the company as they haven't bought for a while. It is a good idea to target these customers with campaigns and offers as well. 24% of our customers fall into either the "Soulmates" or "Lovers" segments, meaning they are good spenders, buy frequently, and have bought recently.

