---
title: Calculations
description: This article provides information about Microsoft Supply Chain Center's Calculations feature.
author: itayhi
ms.author: itayh
ms.reviewer: johnmichalak
ms.service: supply-chain-center
ms.topic: conceptual
ms.date: 4/29/2023
ms.custom: bap-template
---

# Calculations
Calculations are data tables which contain measures and dimensions. Calculations can be used to create KPIs.

## Create a new calculation
1.	First, name the calculation.
2.	Select one or more data sources which will be used for calculation. Ingested entities will be marked as **Application data** **Type**. Previously created calculations will be marked as **Calculation** **Type**. Once you selected the required data sources, select Next.
3.	The selected data sources will be formed into a Power Query screen. On the left hand side, you may see queries called as the data sources which were used. You may transform the data in any of these queries, but make sure to include the data that would be used as a measure in the **Transformation** query. The Transformation query will by default include the same data as the top data source you selected. Once complete, select Next.
4.	Select the refresh cadence of the Calculation. Select **Refresh manually** to refresh the data once. Select **Refresh automatically** to refresh the data on a recurring basis. Select **Submit** for the Calculation to be created.
 
## View Calculation details 
In the Calculations page, you may view the details of a calculation.
 
•	**Owner** shows the user who created the calculation. 
•	**Last run** shows the last time the data refresh was run for the given calculation. 
• **Status** shows the status of the latest data refresh of the calculation. **Success** value means the data refresh was completed successfully. **Idle** means the last data refresh was not completed successfully.  

Select a **Calculation**’s **Name** to view its details.
•	In **Calculation**, you may find the underlying used queries.
•	In **Dependencies**, you may find the underlying data sources that the calculation is dependent on. You may also find any resources that are dependent on the calculation you are viewing. 

## Managing an existing calculation
Currently, editing an existing calculation is unavailable. To manage the existing calculation, click on the **More actions** icon next to the calculation name.
 
•	**Clone** creates a copy of an existing calculation and to change any underlying data transformation using Power Query. 
•	**Rename** changes the name of the selected calculation.
•	**Refresh** sets a one-time data refresh of the calculation.
•	**Delete** deletes the selected calculation. 

## Best Practices
1.	Include a measure and date column in your calculation: 
When creating a calculation for use in a KPI, it's important to include both a measure (or an aggregation) and a date column. The measure should represent the data that you want to track, such as revenue or customer satisfaction. The date column should represent the time period over which you want to track the data, such as days, weeks, or months. 
2.	Sort date columns in descending order: 
To ensure that your KPI accurately reflects historical trends, it is important to sort your date columns in descending order. This way, the most recent data will be displayed first, allowing you to quickly see if there are any changes or trends over time. 
3.	Refresh calculations: 
Calculations used in KPIs should be successfully refreshed to ensure that they are up to date and accurate.  
4.	Use the appropriate level of aggregation: 
When creating calculations for use in KPIs, it is important to measure the smallest possible unit to a high level of aggregation. This means that you should create calculations that represent the data at different levels, from the most granular (such as individual transactions) to the most aggregated (such as total revenue). For example, if you want to track revenue growth for a company by region, you should create separate calculations for each region, as well as a calculation for the company as a whole. The most aggregated calculation can be used in parent KPIs and most granular level in children KPIs. 


