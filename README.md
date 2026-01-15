# Digital Marketing Spending Analysis Dashboard February 2021

## Project Overview

This repository contains information related to the analysis carried out on the digital marketing spending of a ficticious marketing brand across differebt campaigns in the month of February 2021. The data used reflects some facts about what happened - how much was spent, how much was earned, how customers behaved (who clicked on the ad banner, who signed up, who paid). This data is to calculate marketing metrics that would help to evaluate if a did a good job or not and also identify some parameters of the campaign that would be important for analysis. The project ends with a dashboard that visulizes various key metrics from this marketing campaign.

The project was carried out using **Power Query** for data transformation and **Power BI** for visualizing insights.  
It also involved the use of **DAX** for calculations and logical measures.

---

## Tools Used

- **Power Query** — data transformation and cleaning  
- **Power BI** — dashboard creation and visualization  
- **DAX** — calculated measures and analytics  

---

## Project Goal

The goal of this project is to analyse digital marketing spend, identify key marketing metrics that will allow us make more informed decision about the campaign and finally create an interactive Power BI dashboard

The key maketing metrics are:

- ROMI (return on marketing investments): How effective is marketing campaign, one metric that shows effectiveness of every rupee spent. It is calculated ( Total earning (Revenue) - Marketing cost ) / Marketing cost )
- Click-through rate(CTR): percentage of people who clicked at banner (Clicks/ Impressions)
- Conversion 1: conversion from visitors to leads for this campaign (Leads/Click)
- Conversion 2: conversion rate from leads to sales (Orders/Leads)
- Average order value (AOV): Average order value for this campaign (Revenue/Number of Orders)
- Cost per click (CPC): how much does it cost us to attract 1 click on average (Marketing spending/Clicks)
- Cost per lead (CPL): how much does it cost us to attract 1 lead on average (Marketing spending/Leads)
- Customer acquisition cost (CAC): how much does it cost us to attract 1 order on average (marketing spend/ orders)
- Gross profit Profit or loss after deducting marketing cost (Revenue-Marketing spending)

The final interactive dashboard will contain:

1. Revenue by Campaign: total amount of money generated that can be attributed to each marketing campaign.
2. Revenue by Campaign Category: total amount of money generated that can be attributed to each marketing campaign category.
3. Campaign performance overview: showing Campaign Name, Number of Impressions, Number of Clicks, Number of Leads, Number of Orders, Marketing Spend (₹), Revenue (₹), Gross Profit/Loss (₹)
4. Marketing performance trends over time: shows plot of Marketing spend, revenue, average order value (AOV), conversion rate, campaign performance trends over time
5. ROMI by Campaign
6. ROMI by campaign category



## Features

- Three-page **interactive Power BI dashboard**
- Slicers for:
  - Campaign ID
  - Day of month
- Separate file containing all **DAX formulas**

---

## Data

### Raw Dataset

Digital Marketing Dataset:  
https://github.com/ifioklee/Digital-Marketing-Spending-Analysis-Dashboard-February-2021/tree/main/Dataset
### Power BI Dashboard

Interactive Power BI file:  
https://github.com/ifioklee/Digital-Marketing-Spending-Analysis-Dashboard-February-2021/blob/main/Digital%20Marketing%20Spending%20Analysis%20Dashboard%20February%202021.pbix

###  – DAX Measures

File cotaining all DAX formulas: 

---

## Technical Details

### Data Preparation & Transformation (Power Query)

Transformations applied:
- Import marketing.csv file into Power Query
- Change data type of campaign_id column to text
- Create a column named Day by extracting Day from the c_date column
- Create new columns ROMI, CTR, CPC, CPL, CAC, Conversion 1, Conversion 2, AOV, Gross_Profit_loss using custom column fuction
- Remove all NULL entry in the CPL column
- Remove all empty rows from the CAC column
- Change data type of ID column to text

---

## Visualizations in Power BI

### Page 1
#### KPI cards:
- Number of category
- Number of impression
- Number of clicks
- Number of leads
- Number of orders
- Marketing spend
- Revenue
  #### Stacked bar chart:
  - Revenue by campaign
  #### Dornut chart:
  - Revenue by category
  #### Matrix Table:
  - Campaign performance overview
  #### Slicers:
  - Campaign ID
  - Day of the month

---

### Page 2
#### KPI cards:
- Number of category
- Number of impression
- Number of clicks
- Number of leads
- Number of orders
- Marketing spend
- Revenue
  #### Line chart:
  - Marketing performance trends over time
  #### Slicers:
  - Campaign ID
  - Day of the month

---

### Page 3
#### KPI cards:
- ROMI
- CTR
- CPC
- CPL
- CAC
- AOV
- Conversion 1
- Conversion 2
  #### Stacked bar chart:
  - ROMI by campaign
  - ROMI by campaign category
  #### Matrix Table:
  - Campaign ROI and efficiency metrics table
  - ROI by campaign category
  #### Slicers:
  - Campaign ID
  - Day of the month

---

## Results & Insights

A total of 289 campaigns were analysed, each grouped into 4 different categories.

These campaigns run in the month of February 2021 saw a total of 2 billion impressions, 3 million clicks, 66,000 leads generated and 8,043 orders confirmed.

₹30.57 Million was spent on marketing which drove in a revenue of ₹42.89 Million.

The campaign YouTube_blogger  stands out as the campaign with the highest revenue by campaign, generating a total of ₹15,311,433. Facebook_lal brought the least revenue by campaign, generating only ₹300,233.

Influencer campaign category brought in 49.24% of the total revenue while campaigns within the search category brought in the least revenue generating just 8.64% of the total revenue.

The overall Return on Marketing Investment is 40.30%, with click through rate of 0.19%, cost per click of ₹10.28, cost per lead of ₹466.61, customer acquisition cost of  ₹3,801, Average customer order value of ₹8,043.

The YouTube_blogger campaign is the campaign with the highest return on marketing investment while Facebook_lal campaign is the least return on marketing investment.

---


