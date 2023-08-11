---
layout: post
title: Measuring Row Health's Campaign Effectiveness
date: 2023-08-01
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: Row_Health_Screen.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CampaignEffectiviness,MarketingAnalytics,SQL,Excel] #add tags
---
## Summary of Insights

I examined the effectiveness of 57 campaigns by calculating and comparing metrics such as customer conversion rates and click through rates. I looked at overall cost, cost of acquiring a customer, and cost of acquiring an impression. What I found is that CAM005 had the lowest customer acquisition rates and lowest click-through-rates while it also had one of the highest customer acquisitions costs and is among more expensive campaigns for overall cost. For this reason I recommend to suspend this campaign. CAM018 achieved the highest success rate for customer acquisition with a 3.72% customer conversion rate while also having one of the cheapest costs per customer. CAM055 had the highest success rate for brand awareness with a click-through-rate of 65.74%. "Email" as a platform and "Health Awareness" as a campaign type, were both highest achieving for customer acquisiton and brand awareness.

- Used BigQuery to store, pull, and manipulate data in SQL
- Used SQL to calculate metrics such as number of sign ups per campaign, customer acquisition rates, click-through-rates, cost of customer acquisition, and cost per impression
- Used Excel to create pivot tables with conditional formatting in order to visualize seasonality and highlight cost differences
- Used Excel to present my findings and provide process documentation
- [Here you can find my Excel workbook](https://github.com/agiliariniosm/Row_Health/blob/b9e94fdbbf10c40bf8752fa83a322ac681a5b538/Row_Health_Project.xlsm)

## Context 

Row Health is a tech-forward insurance company with over 100,000 customers throughout the United States. In 2019 they launched a Wellness Reimbursement program that subsidizes the cost of popular wellbeing supplements for their users, in order to encourage patients to take well-rounded and daily care of their bodies. These products range from probiotics, to stress relief supplements, to digestive enzymes, which are marketed across various digital channels and campaigns. 

There were three tables I used for this project:
- Campaigns table: information for 57 campains on campaign type, campaign category, impressions, overall cost, and clicks
- Claims data: information for 48,000 claims on claim amount, product purchased, and covered amount
- Customer data: information for 16,400 customers such as the campaign that brought the customer and the state where customer is from

## Marketing Analysis of Row Health's Campaign and Claim Data

### Campaign Customer Acquisition Effectiveness

The top 12 campaigns with the highest customer acquisition rates also have lowest customer acquisiton costs. The success rate ranges from 3.72%-0.05% for these campaigns while cost per customer ranges from $0.36-$3.18. Campaigns CAM005, CAM026, CAM016 have some of the lowest sign up rates, but also have the highest cost per sign up and the overall cost is high. The recommendation is to investigate why these three campaigns did so poorly and to possibly discontinue these campaigns. CAM005 also had the lowest brand awareness success rate, making it a campaign to stay away from. 
![customer_acquisition]({{site.baseurl}}/assets/img/Row_Health/customer_acquisition.png)

Across campaigns run, "Email" as a platform and "Health Awareness" as a campaign type had the highest customer conversion rates. 
![platform&type]({{site.baseurl}}/assets/img/Row_Health/platform_customer_acquisition_1.png)

### Campaign Brand Awareness Effectiveness

The campaign with the highest clight-through-rate is CAM055 at 65.74%. It is also among the cheapest for overall money spent on the campaign so the recommendation is to continue running this campaign. Campaign CAM028 is 7th for highest click through rates and is also among the cheapest campaigns. However, not much money was dedicated to this campaign so it would be a good idea to explore CAM028 and possibly run this campaign for longer. The campaigns with 2nd and 6th highest success rates have above average costs for cost per impression. The recommendation is looking into how to reduce the costs of these campaigns. CAM005 has the lowest click through rate, but is among the more expensive campaigns. The recommendation is to explore CAM005 and likely suspend it. 
![brand_awareness]({{site.baseurl}}/assets/img/Row_Health/brand_awareness_1.png)

Across campaigns run, "Email" as a platform and "Health Awareness" as a campaign type had the highest click-through-rates.
![platform&type]({{site.baseurl}}/assets/img/Row_Health/platform_brand_awareness_1.png)

### Top Products and Seasonality 

The most popular poduct every year 2019-2023 was Hair Growth Supplements, so the recommendation is to always have these products in stock. The most profitable product, on the other hand, was the Detox + Debloat Vitamin. This product was top for profit every year as well. When looking at most products by state, the winners are Vitamin B+ Advanced Complex, Hair Grow Supplements, and the Detox + Debloat Vitamin. 
![platform&type]({{site.baseurl}}/assets/img/Row_Health/products.png)

An annual spike in March was found for both total claim counts and total claim amount.
![seasonality]({{site.baseurl}}/assets/img/Row_Health/seasonality_1.png)





