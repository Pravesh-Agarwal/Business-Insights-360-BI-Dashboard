# 📊Business Insights 360📈

## 📑Project Overview

AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement Data Analytics using Power BI in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholders in terms of all aspects like Finance, Sales, Marketing and Supply Chain.

🔗[Live Report Link](https://app.powerbi.com/view?r=eyJrIjoiMWE1M2Q3ODctYzljZC00M2NjLTgwYmQtOWI0NWY5ZDY5MDU1IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9&embedImagePlaceholder=true)

## 👨‍💻Tech Stacks

- SQL
- Power BI Desktop
- Excel
- DAX language
- DAX Studio (for optimizing the report)
- Project charter file

## 🎓Power BI Techniques Learnt

- What all questions should be asked before staring the Project
- Creating calculated columns
- creating measures using DAX language
- Data modeling
- Using Bookmarks to switch between visuals
- Page navigation with buttons
- Using divide function to prevent zero division errors
- creating date table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting the values in visuals using icons or background color
- Data validation techniques
- Power BI Services
- Publishing reports to Power BI Services
- Setting up Personal Gateway to set up the auto refresh of data
- Power BI App creation
- Collaboration, workspace, access permissions in Power BI Services
- And more 😅

## 🌐GitHub 

- Uploading Large size files using GitHub LFS
- Tracking the particular type of file extensions for LFS

## 💼Business Related Terms

- Gross Price
- Pre-Invoice Deductions
- Post-Invoice Deductions
- Net Invoice Sale
- Gross Margin
- Net Sales
- Net Profit
- COGS - Cost Of Goods Sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer

## 🏬Company’s Background

AltiQ Hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells computer and computer accessories through three mediums/channel

- Retailers
- Direct
- Distributors

Recently the company has faced a unforeseen loss by opening store in America based on the surveys, intuition and some excel analysis. The company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ Hardware has no option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry. 

<br />Project Kick Off Session, where you should get clear picture of this project and all other questions you have with regards to the project:

### ❓Questions To Ask Before Starting With Dashboard

- What is the objective of building this Power BI Dashboard?
- In what terms the success of this project will be measured?
- What will be time dead-line of the project?
- Do the stakeholders expecting pre-view before the actual release?
- What are all the hopes stakeholders have out of this project?
- what are all the fears stakeholders have in terms of building this dashboard?
- Who all will be using this dashboard and for what purpose?
- what are the expectations of stakeholders, by the completion of this project?
- What can go wrong while building this project?
- what are all the resources/ data needed to build this dashboard?
- is there any inputs from stakeholders in terms of design and views of the dashboard?

<br />After the Project Kick Off Sessions, the data engineering team has given the data as per the request of data analytics team, let’s explore them.

### 🧐Dataset **Understanding**

Understanding what data is available will be more helpful while doing analysis. Before jumping on to the analysis get good understanding of what data are available.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions  

- gdb041:
    - dim_customer
        - **27** distinct markets (ex India, USA, Spain)
        - **75** distinct customers thorough out the market
        - **2** types of platforms
            - Brick & Mortar - Physical/offline store
            - E-commerce - Online Store (Amazon, flipkart)
        - Three channels
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - **27** distinct markets (ex India, USA, spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
    - dim_product
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - There are 14 different categories, Like Internal HDD, Keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
        - This table is used to forecast the customer’s need in advance, which can help in
            - Higher customer satisfaction
            - Reduced cost in warehouses for storage purpose
        - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
        - All the date of the month will be replaced by the start date of the month
        - It will have all the column names and in the end it will have the forecast quantity need of the customer
    - fact_sales_monthly
        - This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
- gdb056
    - freight_cost
        - This table has details of travel cost and other cost for each market with fiscal year
    - gross_price
        - Has the details of gross prices with product code
    - manufacturing_cost
        - Has the details of manufacturing cost with product code and year
    - Pre_invoice_dedutions
        - Has the details of pre invoice deductions percentage for each cutomer and year
    - Post_invoice_deductions
        - Post invoice deductions and other deductions details

## 📥Importing Data Into Power BI

- As the database is MySQL in this project, we need to import the datasets from Mysql database to Power BI by providing the Database access credential

## ✨Data Model

- Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
- Poor data modeling affects the over all performance of the report.
- Following good practices of data modeling is must. Refer this page to get to know the good practices [Blog](https://addendanalytics.com/blog/data-modelling-best-practices/)
- In this project, we have followed Snowflake data modeling method.

<img src="https://github.com/Pravesh-Agarwal/Business-Insights-360-BI-Dashboard/blob/main/Resources/Data_model.png" class="center">

### 🎨Dashboard designing

Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required

## 🏡Home view

In Home view, all the views button will be available. User will land on specific view page by clicking the button 

- Info
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Support

## 🌟Overall Report

![Overall Report.gif](https://github.com/Pravesh-Agarwal/Business-Insights-360-BI-Dashboard/blob/main/Resources/Overall.gif)

## 💵Finance View

![Finace.gif](https://github.com/Pravesh-Agarwal/Business-Insights-360-BI-Dashboard/blob/main/Resources/Finance%20View.gif)

## 🏷️Sales View

![Sales.gif](https://github.com/Pravesh-Agarwal/Business-Insights-360-BI-Dashboard/blob/main/Resources/Sales%20View.gif)

## 🛒Marketing View

![Marketing.gif](https://github.com/Pravesh-Agarwal/Business-Insights-360-BI-Dashboard/blob/main/Resources/Marketing%20View.gif)

## 🚚Supply Chain View

![Supply chain.gif](https://github.com/Pravesh-Agarwal/Business-Insights-360-BI-Dashboard/blob/main/Resources/Supply%20Chain%20View.gif)

## 👨🏻‍💼Executive View

![Executive.gif](https://github.com/Pravesh-Agarwal/Business-Insights-360-BI-Dashboard/blob/main/Resources/Executive%20View.gif)

🔗you can find the full report file here : [Report](https://github.com/Pravesh-Agarwal/Business-Insights-360-BI-Dashboard/blob/main/Report/business_insights_360.pbix)


## 🎯Project Outcome

By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
