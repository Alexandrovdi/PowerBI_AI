# Step 2 - Working with Data in Power BI

## Prerequisites

1. [Step 1 - Setup](https://github.com/Alexandrovdi/PowerBI_AI/blob/main/Challenge%20steps/Step%201%20-%20Setup.md) should be done successfully.


## Introduction

The purpose of this challenge is to introduce the participants to working with Power BI Dataflows which will be used in steps 2 - 4, and visualizing data with Power BI which will demonstrate the prepared data.


## Basic Steps to complete
1. Login to [powerbi.com](https://msit.powerbi.com/) and create a new workspace
   - Named your workspace
   - Click "Advanced" and choose "License mode" -> Embedded
   - Select capacity -> "pbi2aiembedded"
   - Click Save
3. In your workspace create a new "Dataflow" and choose "Define new tables"
4. Choose data source Azure SQL Database
5. Select the Products and Customers views, and the FactInternetSales and DimDate tables
6. Select Transform data
   - Rename "DimDate" to "OrderDate"
   - Rename "FactInternetSales" to "Sales"
8. Click "Save and close"
9. Name your dataflow "AdventureWorks"
10. Refresh the dataflow
11. Launch Power BI Desktop and start the "Get Data" process
12. Navigaite to the Power BI Dataflows data source
13. Select the Dataflows that we created earlier
14. Work with data model:
    - Disable relationship OrderDate (DateKey) and Sales (DueDateKey)
    - Make the relationship OrderDate (DateKey) and Sales (OrderDateKey) active
    - Create the relationship between Customers and Sales tables by "CustomerKey" key
    - Create the relationship between Products and Sales tables by "ProductKey" key
15. Create report with your coach 

## Potential pitfalls

1. Dataflows only are avaialble in workspaces, so a user has to create a workspace first.
1. App workspaces are only avaialble to Pro Users, so if the user doesn't have a pro license they must sign up for a 60 day pro trial.
1. If the users is working with a new account for this it is possible that there is a conflict between the credentials in Power BI desktop and the Power BI dataflow.  You may need to clear Power BI's credential cache.


[Next step (Working with Cognitive Services) -->](https://github.com/Alexandrovdi/PowerBI_AI/blob/main/Challenge%20steps/Step%203%20-%20CognitiveServices.md)
