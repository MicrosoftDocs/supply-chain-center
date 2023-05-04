---
title: Create and use calculations
description: This article provides information about how to create and use calculations in Microsoft Supply Chain Center.
author: itayhi
ms.author: itayh
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: how-to
ms.date: 4/29/2023
ms.custom: bap-template
---

# Create and use calculations

Calculations are data tables that contain measures and dimensions. Calculations can be used to create KPIs.

## Create a new calculation

To create a new calculation, follow these steps.

1.	From ... select ...
1. Name the calculation.
1.	Select one or more data sources to use for the calculation. Ingested entities are marked as an **Application data** **Type**. Previously created calculations are marked as a **Calculation** **Type**. After you select the required data sources, select **Next**.
1.	The selected data sources to form into a **Power Query** screen. On the left side, you may see queries called as the data sources are used. You may transform the data in any of these queries, but make sure to include the data that would be used as a measure in the **Transformation** query. The Transformation query, by default, includes the same data as the top data source you selected. Once complete, select **Next**.
1.	Select the cadence for refreshing the Calculation. Select **Refresh manually** to refresh the data once. Select **Refresh automatically** to refresh the data on a recurring basis. 
1. Select **Submit** to create the Calculation.
 
## View Calculation details 

In the Calculations page, you may view the details of a calculation.
 
-	**Owner** shows the user who created the calculation. 
-	**Last run** shows the last time the data refresh was run for the given calculation. 
- **Status** shows the status of the latest data refresh of the calculation. The **Success** status means the data refresh was completed successfully. The **Idle** status means the last data refresh wasn't completed successfully.  

To view deails for a calcualtion, select its name.

-	In **Calculation**, you may find the underlying used queries.
-	In **Dependencies**, you may find the underlying data sources that the calculation is dependent on. You may also find any resources that are dependent on the calculation you're viewing. 

## Managing an existing calculation

Currently, editing an existing calculation isn't available. To manage an existing calculation, select on the **More actions** icon next to the calculation's name. The following actions can be performed on the calculation.
 
-	**Clone** creates a copy of an existing calculation and changes any underlying data transformation using **Power Query**. 
-	**Rename** changes the name of the selected calculation.
-	**Refresh** sets a one-time data refresh of the calculation.
-	**Delete** removes the selected calculation. 

## Best Practices

While working with calculations, please observer the following best practices.

1.	Include a measure and a date column in your calculation. 
2.	Sort date columns in descending order. To ensure that your KPI accurately reflects historical trends, it's important to sort your date columns in descending order. This way, the most recent data is displayed first to allow you to quickly see if there are any changes or trends over time. 
3.	Refresh calculations. Calculations used in KPIs should be successfully refreshed to ensure that they're up to date and accurate.  
4.	Use the appropriate level of aggregation. When creating calculations for use in KPIs, it's important to measure the smallest possible unit to a high level of aggregation. This means that you should create calculations that represent the data at different levels, from the most granular (such as individual transactions) to the most aggregated (such as total revenue). For example, if you want to track revenue growth for a company by region, you should create separate calculations for each region, and create a calculation for the company as a whole. The most aggregated calculation can be used in parent KPIs and most granular level in children KPIs. 


